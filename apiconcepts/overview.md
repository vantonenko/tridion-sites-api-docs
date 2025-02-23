# Tridion Sites API Documentation #
Tridion Sites is an enterprise-class web content management system that lets you manage complex global web, mobile and other digital touchpoints. Together with Tridion Docs, it forms the Tridion suite of products.

## [Content Delivery Public Content API](https://docs.rws.com/956379/888888/) ##
Content Delivery exposes its content through the Public Content API, in the GraphQL query language. To interact with the API and the published content, use an in-browser GraphQL IDE such as GraphiQL.

Select [this link](https://docs.rws.com/binary/956379/955694/) to download the Public Content API reference documentation.

## [Extension points in the .NET Content Interaction Libraries](https://docs.rws.com/956379/631159/) ##
Various interfaces in the .NET CIL enable you to override various default implementations. You can use Microsoft Unity to inject any new dependencies you create.

## [Content Deployer extensions](https://docs.rws.com/956379/695273/) ##
When a user publishes content, the Content Deployer unpacks the incoming Transport Package and processes its transport instructions. You can extend the default behavior of the Content Deployer by creating a custom Module and adding it to a Step, or by extending an existing Module.

By default, the Content Deployer runs through a list of item types (Pages, Components and so on) in the package. For each type, it then deploys all the items in the package (that is, it sends the items to the Storage Layer). The deployment process as a whole is called a Pipeline, and each step of the deployment process is called a Step. If a Step performs a deployment or undeployment, it can contain a Module. You can extend existing Modules, or build a new one and add it to a Step.

To add your extension to Content Deployer, run the microservice startup or installation script with the extensions switch pointing to your extension.

## [Implementing Add-ons](https://docs.rws.com/956379/771360/) ##
To extend the functionality of Tridion Sites with custom functionality, create or obtain one or more Add-ons.

An Add-on takes the form of a ZIP file. The ZIP file must contain one or more Extensions, which together represent your custom feature. If you want, you can combine multiple custom features in a single package as well.

The package must also contain a manifest file, which explains where each Extension is located, and may include custom configuration for each Extension.

## [Implementing Connectors](https://docs.rws.com/956379/919091/) ##
A Connector is a specific type of Add-on that is specifically used to integrate Tridion Sites with other systems, either other RWS products or third-party systems. RWS provides a number of Connectors built on Tridion Integration Framework, which you can optionally purchase and implement, plus you can use the framework and SDK to build additional, custom Connectors. The SDK is available for .NET Core and Java.

## [Content Manager extension points](https://docs.rws.com/956379/480866/) ##
Content Manager extension points are the APIs you can use to implement Content Manager functionality: you can use the TOM.NET API for developing templating and Event Handler and Workflow, the Content Manager Explorer extension API to add custom controls and behavior to the GUI, and the Core Service API to interact with the Content Manager from a third-party application or third-party GUI.

If you use 32-bit COM components inside your .NET extensions (e.g. .NET event handlers), your code will fail on a 64-bit operating system. To prevent this, put your COM component in a COM+ app.

## [Translation Manager API and Plugin System](https://docs.rws.com/956379/690092/) ##
You can customize the functionality provided by the Translation Manager using the Translation Manager API. The API provides classes that you can use to access and extend the Translation Manager. For example the Plugin System allows you to load custom DLLs created using this API into the Translation Manager and you can trigger translations from the Event System and Workflow.

## [API reference documentation downloads](https://docs.rws.com/956379/884682/) ##
Links to download the API reference documentation for Tridion Sites. The ASP.NET APIs are available as .chm files and the Java APIs as Javadoc.

The following documentation is available:

### Content Manager APIs (.chm files) ###
- [TOM.NET API reference](https://docs.rws.com/binary/956379/952141/)
- [GUI API reference](https://docs.rws.com/binary/956379/955707/)
- [Core Service API reference](https://docs.rws.com/binary/956379/952144/)
- [ECL API reference](https://docs.rws.com/binary/956379/955810/)
- [Translation Manager API reference](https://docs.rws.com/binary/956379/955807/)

### Content Delivery Content API (GraphQL Schema) ###
- [Content Delivery Public Content API (GraphQL Schema)](https://docs.rws.com/binary/956379/955694/)


### Content Delivery .NET APIs (.chm files) ###
- [Content Delivery RESTful API (.NET)](https://docs.rws.com/binary/956407/955697/)
- [Experience Optimization Content Delivery (ASP.NET)](https://docs.rws.com/binary/956379/955964/)


### Content Delivery Java APIs (Javadoc) ###
- [Content Delivery RESTful API (Java)](https://docs.rws.com/binary/956407/955700/)
- [Experience Optimization Content Delivery (JSP)](https://docs.rws.com/binary/956379/955704/)


### Tridion Integration Framework APIs ###
- [Tridion Integration Framework API (.NET)](https://docs.rws.com/binary/956379/955804/)
- [Tridion Integration Framework API (Java)](https://docs.rws.com/binary/956379/955798/)
- [Tridion Integration Framework SDK (Java)](https://docs.rws.com/binary/956379/955801/)

## Tridion DXA ##
This section is intended for developers wanting to extend DXA functionality using its open-source .NET and Java APIs.

### Customizing and extending DXA ###
[Development prerequisites](https://docs.rws.com/784837/720093/sdl-digital-experience-accelerator-2-2/development-prerequisites)
Developing custom Tridion Sites web applications/sites requires a full development environment. The necessary third-party software differs depending on whether you are developing a .NET or Java application.

[.NET web application development](https://docs.rws.com/784837/682805/sdl-digital-experience-accelerator-2-2/-net-web-application-development)
Set up a .NET development environment to customize or extend the DXA .NET web application.

[Java web application development](https://docs.rws.com/784837/720545/sdl-digital-experience-accelerator-2-2/java-web-application-development)
Set up a Java development environment to customize or extend the DXA Java web application.

[Using SDL's public APIs](https://docs.rws.com/784837/679912/sdl-digital-experience-accelerator-2-2/using-sdl-s-public-apis)
Use the available public APIs to extend and customize the behavior DXA.

[Creating the folder structure for a custom module](https://docs.rws.com/784837/651695/sdl-digital-experience-accelerator-2-2/creating-the-folder-structure-for-a-custom-module)
A custom module implements a distinct piece of functionality that is only relevant to some implementations. When you want to add a module to RWS Digital Experience Accelerator, you need to create a folder structure in Content Manager.

[Model mapping and semantics](https://docs.rws.com/784837/695734/sdl-digital-experience-accelerator-2-2/model-mapping-and-semantics)
Domain (Content Manager) Models are mapped to the Presentation (View) Models using Model Semantics so that web developers can work with data structures optimized for the Views they are creating without having to have a deep understanding of the underlying content model.

### API reference documentation downloads ###
Links to download the API reference documentation for RWS Digital Experience Accelerator.
- [DXA API for .NET](https://docs.sdl.com/DXA/DotNET/2.2/APIDOC/)
- [DXA API for Java](https://docs.sdl.com/DXA/Java/2.2/APIDOC/)
- [Content Delivery's Public Content API](https://docs.rws.com/binary/956379/955694/)

