## Build Visual Applications using Oracle Visual Builder Studio

### Unit 1 : Introduction to Visual Builder Studio and Visual Builder

- VBS is a robust application development platform that helps your team effectively plan and manage your work throughout all stages of the app dev life cycle; design build test and deploy
- With VBS, you get: Built in repositories, CI,CD Designer, Git, built and deploy different flavour of UI, agile board ans issue tracking system
- Project artifacts are stored in OCI Object Storage bucket
- Although VBS provides a Git repository for you, you can choose to use external repos, such as GitHub and BitBucket
- A project owner can create and configure a webhook to send notification to remote service and application about Oracle Visual Builder Studio  events. Ex: Slack, PagerDuty, Jenkins, Hudson, Genric Webhooks
- Project collects al the people; An environment lets you define and manage Oracle Cloud PaaS and SaaS; VBS uses hosted Git repositories to store source code and version contron; Create or edit apps in workspace; Use build page to create and configure builds jobs and pipeline
- In a project there is Projet Owner, Developer, Limited Developer, Contributor (can access the projet's component in read-only)
- From the Environment page you can: Create and delete environment, Add or remove service instances, Update the details, View the details, view deployment
- You can create, update and search issue from the ISSUES page or from Agile boards, You can also use REST APIs to create, retrive and update issues
- A workspace is a private Designer area with its own local Git repository and full remote git support built-in
- VB instances can be accessed from OIC or FA, or as a stand-alone instances via URL

### Unit 2 : Create Visual Application in Visual Builder

- Single Page Application (index.html) **header, flows & Pages and footer**
- Variant of single page application: FA v1 Application (Stand-alone) and FA v2 Application (App UI)
- |Unified App Defines|App UI comprises|
  |-|-|
  |Content and properties|Page and Page flows|
  |Redwood JS stripe| HTML,OJ, and OJ-SP|
  |Common VB service|Action chains|

- Fusion Application developed in VB are based on the technology stack known as **Redwood Stripe**
- **App UI** application are implemented as modules plugged into the Unified App; **Stand-alone App** are independent copies that are not sharing code
- Base Applications, which are produced by Oracle reffred as "factory extension"
- Visual Appliation Development Wokflow :
  - Create a new application or join an existing version -> Create a service connection-> Create business object -> Import real data and check the schema -> Develop the web or mobile app-> Secure the application -> Stage and test the application -> Publish the application
- Your work is not visible unless: a) merge it b) chose to share with other c) deploy
- An environment is also known as **pointer**, must be a seperate VB instance
- To develop an applicattion, you need to define its metadata (JSON) and create its pages and artifacts
- When you open an application in the Navigator, the structure of the application is displayed as nodes and subnodes
- Also the Designer has dedicated editors for each if the building blocks used to build your application
- In the diagram view : a) COLLAPSE or EXPAND flows for readability b) Properties pane displays page and subflow details c) Audits pane automatically show errors and warnings
- Also use LIVE mode to test code, DESIGN to add and configure components and CODE to edit the page's HTML
- Use COMMIT to snapshot your wirk as of a specific time. Commits document the process of saving files to the repository for AUDITs, ROLLBACK and EASIER CODE MANAGEMENT
- Web and Mobile apps created using Visual Builder can use the Oracle Identity Cloud Service (IDSC)


### Configure and Manage Service Connections in Visual Application
- Basic service information: Overvie, Servers, Endpoints, Headers, Tranform, Sources
- You can add edit or remove backend servers and you may have more than one server
- For static service connetion a list of service endpoint is display, for dynamic service connection read only view of all end point
- Headers are headers written in the REST call to the service
- Use transform scripts to change the REST API request and response to handle function such as Pagination, Filtering and Sorting
- The source tab show interlly stored service connection defintion in OpenAPI compliant JSON Format; connection setting, response, request defintion and other prarametre
- **Backend** is a collection of servers that your visual application uses to access REST endpoints in a known resources, such as Oracle Cloud Application or Integration
- Each backend is associated with one or more server, each server has different instance, backend instance are defined in tenant setting of VB
- You can choose to override the tenant-level defintion for a single application either to customize and existing backend
- Some backed service types are: Oracle Cloud Application, Integration, Process, Custom, Custom ADF Describe
- Only one type of backend can be added per backed in a visual application
- Multiple server can be added for every backend type, each associated with 1 app profile
- Creating a service connection: Using a Service catalog, Providing the Document Descriptor for the service and Using an Endpoint
- You can create a dynamic servie connetion whe nyour application is in development and then convert the dynamic connection to a static connection when your application is ready for prod.
- |service connedtion option|Advantages|Disadvantages|
  |-|-|-|
  |Copy full OpenAPI to your application(static)|Better performance|Application is out of sync|
  |Dynamically retrive metadata (Dynamic)|Provide most up to date service| Performance impacted|
  |Copy minimal OpenAPI to app (recommended)(Static+dynamic)|Optimal performance|Impacted|
- Supported service descriptor types:(Creating a External Service Connection(No Catalog)) Open API/Swagger, Oracle ADF Describe
- Create an External Service Connetion (No Descriptor): use a REST API endpoint if descriptor is not available
- Edit service connetion definition if swagger descriptor is missing or incomplete or to override existing service definition
- Pagination function that limits the number of records that are displayed on a page in REST
- You can modify the following when editing a service connection: ADD A SERVER, ADD MORE SERVICE ENDPOINTS, EDIT SERVICE ENDPOINTS, EDIT AUTHENTICATION DETAILS, ADD TRANSFORM
- Tokens are way of encoding the alling use identity into a string according to different specification such as SAML or JWT format
- Authentication mechanism that use the identity propagation type of mechanism are:
  - Oracle Cloud Account, User Assertion OAuth 2.0, Propagate Current User Identity (Delegate Authentication)
- Fixed Credential Authentication Mechanism : None (doesn't need any kind of authentiation), Basic, Client Credential OAuth 2.0, Resource Owner OAuth 2.0, Oracle Cloud Infrastructure API Signature 1.0
  - 
- 
