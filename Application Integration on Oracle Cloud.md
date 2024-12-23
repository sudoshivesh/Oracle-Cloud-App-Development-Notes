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
    - Delete : Removes the integration from this OIC environment (Only deactivated intergation                 can be deleted


