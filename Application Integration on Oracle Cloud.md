## Application Integration on Oracle Cloud

### 1. Introduction

**RESTfull Web Service**
- Represenataional State Transfer
- REST is an **architectural style**, not a protocol. It leverages standard HTTP methods (GET, POST, PUT, DELETE) for communication between client and server.
- The server does not store any session information between requests, so it's **stateless**
- Interactions are based on **CRUD** operation, typically uses **JSON** though XML can also be used.
- **Faster and more flexible** than SOAP; ideal for web service in Modern Appication. eg - Mobile App and web APIs

**SOAP Web Service** (Simple Object Access Protocol)
- Protocol that defines strict standards for messaging and communication.
- Messages are formatted in XML, rigid and complex than JSON
- Can maintain STATE if needed

**Platform as a Service (PaaS)**
- PaaS is ideal for developers who want to focus solely on application development without managing infrastructure, typically for building web apps, APIs, and microservices.
- Example: Google App Engine, Microsoft Azure

**Software as a Service (SaaS)**
- SaaS is used for software that’s accessed online, such as email, CRM, file storage, and collaboration tools. It offers easy scalability and accessibility, especially for businesses that don’t want to maintain their own software infrastructure.
- Example: Google Workspace, Microsoft 365


### 2. OIC Integration architectural Overview

- SaaS Application (Oracle Cloud, ERP, HCM, SCM) ko On-premises application (Custom Apps, people soft, e-business suite, Spreadsheet, SAP) ke saath quickly, cost efficteviely, and rapid innovation ke liye connect karna complex hai using traditional approaches
- Problems are : **Costly** to upgrade and maintain, **Incomplete view** of business, **Inconsistent experince** for customer and employees and **slow** to deliver and change
- Oracle ke bahut saare customer ke paas **Complex on-premises integration and automation investment** hai like - Service Oriented Architecture (SOA) or Enterprise Service Bus (ESB)
- **Oracle Integeration runs on Gen2 cloud infrastructure and includes 3 core - i) Application Integration using prebuilt Adapters  ii) Process Automation using example recipes  iii) Visual Builder using Business Accelerators**
- **Application Integration** connects all of SaaS and On-premises business application 6-10 times faster using prebuilt adapter to simplify the technical complexity of dealing with low level API
- **Process Automation** helps BA, App IT, and Integration Specialist collborate in parallel using prebuilt example recipe which combine source and target application adapter with a trigger and a example data map.
- **Visual Builder** - Gives you a quick way to extend SaaS and on-premises application with drag and drop tooling for mobile apps in minutes.
- Oracle Integration is available in mainly two edition - i)Standard ii)Enterprise

**Oracle Integration Cloud Services** - 
- Create and manage Integration(Integration) -> *Create the connection to the applications you want to share data with. Then set up the integration, which uses the connection you created and define how data is shared between your application*
- Build Automated Process Application(Process Builder) -> *Automate your business using process application: develop, test, publish, and activate. Repeat whenever changes are needed*
- Develop Web & Mobile Application(Visual Builder) -> *quicly create and publish custom web and mobile application using visual development tool. No setup and No coding is required. It leverage the Open Source Oracle javscript Extension Toolkit (Oracle JET) to create engaging web and mobile interface.*

- The basic component are visual application are mobile applications, web application, service connections, business objects, and pocesses.
- The basic building block of a mobile or web aapplication are user interface (UI) components, variables, action chains, page flows and page navigation, and data access through REST endpoints.
- Oracle Integration Cloud (OIC) is a complete, secure, but lightweight integration solution that enables you to connect your application in the cloud.
- OIC lookups maps the different codes or terms used by the application you are integrating to describe similar items
- Visual Data Mapper enables you to quickly create direct mappings between the trigger and invoke data structure
- From the mapper, you can also access lookups tables and use standard XPath function to map data b/w your application


### 3. Integrations Life Cycle & Packages

- Prebuilt Integration help users accelerate their integration projects. **Types - i) Oracle Created ii) Third Party or User Created**
- Integration ko development se test me leke aane ke liye (ek environment se dushre environment) me use krne ke liye hume package bananna hota hai jisse test kerne me easiness ho;
- Empty package can't be created; Package have no scope; All integration are still visible to one another regardless of package designation. .par & .iar are the extension
- Exported Integration include all of thier dependent connection resources but Inported Integration will NOT include the importof their dependent connection.
- **Life Cycle Operation for Integration**
    - View : Open the Integration design canvas in view only mode
    - Edit : Open the Integration design canvas in edit mode. Only deactivated Integration can 
             be edited and modified
    - Clone : Create a new Integration that can be edited seperately
    - Create Version : Require you to specify a new version number. Same as clone.
    - Export : Downloads an Integration (.iar) archieve file
    - Delete : Removes the integration from this OIC environment (Only deactivated intergation can be deleted)
- **Integeration Versioning**
    - Integration are uniquely identified by a unique identifier and a version number (format xx.yy.zzzz where xx is major version and yy.zzzz is minor version. You can create additional version.
    - Integration with same major version but a different minor version follow the rule. Only one activation can be active. Dushra active hoga to pehla deactivate ho jayegaa
    - Integration with different major version, can be active at same time
 

### 4. Fundamental of Creating Integration

- What is an OIC Integration
    - Define the flow of message and it's the main ingredient of Oracle Integration
    - An Integration includes 
          - Atleast a Trigger (source) connection for request sent TO OIC
          - One or more Invoke (target) connection for request sent FROM OIC
          - Data Mapping or Field Mapping b/w two connecton (both request and response)
- OIC Integration Style
    - Basic Routing (deprecated)
    - Publish to OIC : Fire and Forget Integration pattern are handled by Public to OIC and Subscribe to OIC
    - Subscribe to OIC
    - App Driven Orchestration (Oracle Recommendation) : Allow all four interaction pattern or message exchange pattern (1. Synchronous Interface {request-response} 2. Asynchronous Interface {one-way} 3. w/ callback 4. event based)
      .Switch expression, looping construct, robust fault handling are included.
    - Schedule Orchestration : use cases that need to be triggered on a recurring schedule and/or on demand
    - File Transfer : identical to Schedule Orchestration

- Integration Development and Management Workflow
    - Define Connection -> Build Integration Flow Logic -> Map Data -> Activate Integration -> Monitor Integration
    - Basic Integration Development Workflows Steps
      
          1. If necessary, create new connection (select adapter and define connection)
          2. Create a new integration (Select the App Driven Orchestration Style and optionally you add it to a pkg
          3. Add and configure the trigger (source) connection
          4. Add and configure the invoke (target) connection
          5. Map data for the invoke connection request
          6. Map data for the response to be returned to the source (if applicable)
          7. Define the key business identifier for monitoring purpose
          8. Activate and test
    - The map you create are called transformation maps and use the eXtensible Style Sheet (XSL). A visual mapper enable you to map fields between appliction by dragging source field into targer field.
 
### 5. Creating OIC Adapter Connection....

- Oracle Cloud Adapter : Benifits
    - Adapter simplyfy and accelrate integration with SaaS and on-premises application
    - Improve developer productivity by allowing an interface, which is user driven
    - Provide runtime benifit by session management and security
    - With adapter, everything is packaged, covered and transparent to end user
    - Adapter allow you to generate normalized, integration-friendly web services, thereby making the mapping much faster
- Feature of Oracle Cloud Adapter
    - Provide both design time and runtime features for implementing and depploying specific integration use case
    - Session Management, Simple to configure, Standard error-handling capabilities, Native Suport
    - High availability, scalability, and reliability
- Available OIC Adapter
    - Oracle Cloud SaaS Application
    - Third-Party Cloud SaaS Application
    - On-Premises Enterprise Application
    - Social/Productivity Application
    - Generic Technology Adapters : Databases, FTP/File Servers, REST, SOAP
- What is a Connection?
    - Connection define INFORMATION about the instance o each configuration you are integrating.
    - A connection is based on adapter
    - Connection are used in one of two roles: - trigger (inbound) & Invoke (Outbound)
    - Trigger (inbound) : Define a SOAP or REST interface allowing client to invoke integration flow
    - Invoke (outbound) : Used to define an external service or system that can be called from an integration
- Creating a connection
    - Select a Adapter -> Provide Basic Info -> Configure Connection Properties -> Configure Security -> Test the Connection
    - **Configure Connection Properties AND Configure Security** : Are specific to the chosen adapter
    - 60+ Adapters defined in OIC
    - Oracle Servce Cloud (RightNow), Oracle Engagement Cloud, Oracle ERP Cloud, Oracle HCM Cloud, salesforce etc.
    - The defined 11 adapters in the guide is from page 115-137


### 6. Configuring Trigger Connections

- Integration Development
    - To tell OIC how to map data between your application use *Graphical Mapper*
    - To see how well your integration are running & monitor error use *Monitoring dashboard*
    - Define Connection -> Build Integration Flow Logic -> Map Data -> Activate Integration -> Monitor Integration
- Message Exchange Pattern between Client Apps & OIC Integrations
    - Synchronous request/response
    - Asynchronous request/callback
    - Asynchronous request (one-way) - aka "fire and forget"
    - Event-based
- These 27 adapter can be used in the trigger role for an integration flow (page -168)
    - File Adapter, FTP Adapter, REST Adapter, SOAP Adapter, MySQL, SAP Adapter etc.
- Getting Started - Trigger Connections
    - Allowed while naming : English Alphabet, number, underscore, and dashes
    - Not Allowed: Blank Spaces, Special Character, Multibyte Character
- Using the Adapter Endpoint Configuration Wizard (Refer 171-200) for given 6 Wizard

### 7. Configuration Invoke Connections
- Integration Development Phases
    - Define Connection -> Build Integration flow logic -> Map Data (Use OIC Data Mapper) -> Activate Integration -> Monitor Integration (track payload & manage error)
    - Over 60 adapters are pre-installed in your OIC environemnt. Almost every adapter type is used in the invoke role for an integration flow
    - Read about the 8 configuration wizard from page(211-260)

### 8. Data Mapping
- OIC Data Mapping
    - A VISUAL MAPPER enables you to define data mapping b/w d/f data structure by using drag and drop
    - Transformation is supported between XML and XML (XSLT, XPath, OIC Lookups, Expression Builder). It create for-each statement automatically.
    - Transaformation maps use XSL. Required field are identified by a blue asterisk
    - Mapping supports both *qualified and unqualified schemas*
- Creating Transformation Outside of OIC
    - Some task can't be performed in the OIC mapper. We will use **JDeveloper.**
    - The XSLT Map Editor provides the following edit views under the design view :  Map View and XSLT View
    - When using Custom javascript function: Two option are offered in OIC- a) Register as a custom XPath function b) Register as a Javascript function call
- Using OIC Lookups
    - Use Lookups to create in-memory "tables"
    - It maps different terms used to describe the same item across your application
    - Lookups are **resusable**
    - Lookups associate value used by one application for a specific field to the values used by other application for the same field
    - For Example: Country Code, city codes, currency codes and so on...
 

### 9. Orchestration Integration Actions
- Define Connection -> **Build Integration Flow Logic (action for facilitating orchestration inegration flow logic)** -> Map Data -> Activate Integration -> Monitor Integration
- Orchestration Styles : App Driven & Scheduled
    - App Driven : Interface invoked by a client application or API. It create an integration tht uses *an event or business object* to trigger the integration. **CallBack activities** (to end a process and respond back to sender) and **end activities** (to end a process without responding back to the sender) are included in the asynchronous activation
    - Scheduled : Excecutes automatically or on-demand for batch bulk, integration or file processing. Create an integration that uses a *schedule* to trigger the integration instead of an adapter
- Editing view option
    - Canvas View: Display the default view of integration canvas
    - Psedu View : Display the integration vertically with child nodes indented.
 
- invokes can be placed within (this is same for **action**)
    - The main flow path
    - The golbal fault handler
    - For-each loops
    - while loops
    - branch of a switch activity
    - Scopes
    - Scope fault handlers
- You cannot **Delete** a trigger connection connection in an integration (Delete option isn't available)
- Action are organized into five sections: (with thier functionality)
    - Data: Assign, EDI Translate, Map, Stage File
    - Call: Integration, javascript, Process
    - Collection: For Each, Scope, Switch, While
    - Genral: Logger, Note, Notification, Wait
    - End: Re-throw fault, Throw new Fault, Fault Return, Return, Callback, Stop






