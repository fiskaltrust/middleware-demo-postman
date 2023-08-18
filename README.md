# fiskaltrust.Middleware demo (Postman collection)
A Postman collection containing examples that demonstrate how to call the fiskaltrust.Middleware via HTTP.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://middleware-samples.docs.fiskaltrust.cloud/)

## Getting Started

### Prerequisites
In order to use this demo collection, the following prerequisites are required:
- *Postman with the imported collection*: [Download Postman](https://www.postman.com/), an API testing tool, and install it on your machine. Then click on "Run in Postman" on the [middleware API docs](https://middleware-samples.docs.fiskaltrust.cloud/) to import the collection.
- *The fiskaltrust.Middleware* running on your machine, which can be configured and downloaded via the fiskaltrust.Portal ([AT](https://portal.fiskaltrust.at), [DE](https://portal.fiskaltrust.de), [FR](https://portal.fiskaltrust.fr)). Start it (either by running it as a service, or with the `test.cmd` file), and let it run in the background to handle your requests.
- *Your Cashbox Id* is visible in the portal. It is also displayed in the startup console log of the Middleware. 

### Executing the demo requests
After importing the Postman collection, you first need to set the required variables:
- Right-click on the collection and select _Edit_
- Open the _Variables_ tab, and enter the values for `cashbox_id` and `base_url` 
   - **cashbox_id** is a GUID and shown either in the Portal or in the log of the Middleware itself
   - **base_url** is the URL of the Middleware's HTTP endpoint, **without a trailing slash**. This could e.g. look like this: `http://localhost:1500/bda7742e-fb7e-4eb6-b3ee-27e0c48fc316`. Again, this URL is both displayed in the Portal and in the Middleware log.

After you configured these two variables, you can easily run the examples by double-clicking them in the "Collections" menu.

For more information about how to use Postman collections, please refer to [their extensive documentation](https://learning.postman.com/docs/postman/collections/intro-to-collections/).

## Documentation
The full documentation for the interface can be found on https://docs.fiskaltrust.cloud. It is actively maintained and developed in our [interface-doc repository](https://github.com/fiskaltrust/interface-doc). 

More information is also available after logging into the portal with a user that has the _PosCreator_ role assigned.

### Communication
The fiskaltrust.Middleware supports different communication protocols, effectively giving our customers the possibility to use it on all platforms. Hence, different protocols are recommended for different platforms. Given that HTTP is one of the most generally used network communication protocols, it should be supported on all required platforms. Please have a look into our other demo repositories for alternatives, e.g. via gRPC or SOAP.

#### User specific protocols
With the helper topology, it is possible to solve every scenario. Please contact our support if you required assistance for a special case scenario.

## Contributions
We welcome all kinds of contributions and feedback, e.g. via Issues or Pull Requests. 

## Related resources
Our latest samples are available for the following programming languages and tools:
<p align="center">
  <a href="https://github.com/fiskaltrust/middleware-demo-dotnet"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0d/C_Sharp_wordmark.svg/100px-C_Sharp_wordmark.svg.png" alt="csharp"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/fiskaltrust/middleware-demo-java"><img src="https://upload.wikimedia.org/wikiversity/de/thumb/b/b8/Java_cup.svg/100px-Java_cup.svg.png" alt="java"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/fiskaltrust/middleware-demo-node"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/100px-Node.js_logo.svg.png" alt="node"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/fiskaltrust/middleware-demo-android"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d7/Android_robot.svg/100px-Android_robot.svg.png" alt="android"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/fiskaltrust/middleware-demo-postman"><img src="https://avatars3.githubusercontent.com/u/10251060?s=100&v=4" alt="node"></a>
</p>

Additionally, other samples (including legacy ones) can be found in our [demo repository](https://github.com/fiskaltrust/demo).
