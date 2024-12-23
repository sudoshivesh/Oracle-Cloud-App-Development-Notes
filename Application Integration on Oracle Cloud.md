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
- 
