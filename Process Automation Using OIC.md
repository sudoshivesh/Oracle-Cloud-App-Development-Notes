## Process Automation Using Oracle Integration Cloud


- Processes in Oracle Integration
  - Design (Composer), Automate, Manage (Workspace)
  - Composer -> Design Time Environment
  - Workspace -> Runtime Environment
  - | Design Time Environment | Run time Environment |
    |-|-|
    |Design| Automate , Manage|
    |Composer|Workspace|
    |Graphics tools, Quickstart apps, Test environment, process application|stay organised, share docs and collaborate,tool to track process, view complete reassign and delegate|
  - BPMN -> Business Process Model and Notation
  - WSDL - Web Service Description Language
  - REST -> Represenational State Transfer
- Process Role
  - | Process Role| Details | Note |
    |-|-|-|
    |Administrator|![image](https://github.com/user-attachments/assets/a50b68fa-f9e5-4249-babf-a2f1092d362c)||
    |Developer|![image](https://github.com/user-attachments/assets/36fd3cd5-1250-4b60-9eed-15f3d43b32aa) |Developer can't access the administration page in the design time or runtime environment. They Can't Create modify or deletes user for processes|
    |End User|![image](https://github.com/user-attachments/assets/4059c24d-452d-40c9-a38d-1c9aaa775474)|End user can't access any page in the design time environment and can't access administration pages in runtime. They Can't Create modify or deletes user for processes|
    |Oracle Content Management User|![image](https://github.com/user-attachments/assets/a683b0e1-682f-4066-b551-7d2357a79a83)|the integration user is assigned to this role|

- In Oracle Integration navigation pane, click my task, to work, monitor, troubleshoot ot administer process tasks.
- Process Application : In oracle Integration Navigation pane, click processes and then Process Application
  - Create application from scratch or importing
  - Manage your application, viewing, cloning, unlocking, downloading and deleting
- Application can be developed from scratch or using Sample, QuickStart
- Process Application made up of the following application component:
  - Processes. Forms, Business Types, Decision, Integrations, Indicators


### Create and Manage Application
- QuickStart Apps and Sample applicaion are located in the gallery. They are ready to use customizable and fully built
- Developers can easily build process application without any process knowledge
- Using the QuickStart Apps, developers can easily build process applications without any knowledge on BPMN. (Business Process Modeling Notation)
- On creating an application based on a QuickStart App, a copy of the pre-built application will be created with the name of the process application being created
- A process application can be created from the Process Application home page by clicking on Create button. It Shows THREE option
  - 1. To create an application based on **QuickStart App**, choose the option Start with a QuickStart.
    2. To create an application from scratch, choose the option Create an Application.
    3. To create an application based on already created application.
    Simply - Start with quickstart, import an application(.exp), create an application (scratch)

- SNAPSHOT : It is a read-only copy of an application at a particular moment. You can't open them for editing. You can Create a snapshot from the last published version of an application.
- You can view the content of snapshot
- Export an application based on snapshot - Deploy and application and Delete
- Participant with owner or editor permission can create a snapshot
- APPLICATION ROLES
- Use application roles to model the users, groups, or system that perform the work your business process represent. The predefined roles are: Process Owner, Reviewer, Analytics Viewer, Automatic Handler
- Application snapshots in Process can be exported to your local file system as .exp


### Develop Structured Process
- Structure Process
  - is a sequence of task, that after peformed, results in well defined outcome.
  - BPMN (Business Process Model and Notation, define the flow and behaviour
  - A process instance refer to a specific instance of a process.
  - new structure process are synchronous and after creating a new process you can change the type to Asynchronous, Manual or Resusable
  - Component of a Structured Process
  - Flow Element ( Tasks, Events, Gateways, Sequence Flows) and Data Objects are component
  - Data Object : used to define and store the information used by a process. Also DO are variables that are defined during the modelling and implemenatation of a process
- Steps to Create Structured Process:
  - Create -> Assign -> Design -> Configure -> Define -> Associate
- Application roles are defined for the entire application. They can be shared by all the processes in your application
- Swimlanes : Horizontal lines that run across the process editor canvass. All flow elements must be placed within a swimlane
- Elements : Elements are BPMN based. Used by dragging and dropping onto process editor canvas. After addign an element, you define its PROPERTIES, DATA ASSOCIATION, FORMS & SEQUENCE FLOW where they apply...
  - Elements are categorised into following types
  - Human, System, Events, Gateways, Insights, Integrations, Others
  - Human : Submit , Approve
  - System :  Data Mapper, Service, Call, Send, Notify
  - Event : Start, Form Start, Message Start, End, Error Boundary
  - Gateway : Exclusive, Inclusive, Parallel, Event Based
  - Integrations : Integration
  - Other : Note
- Communication Between Process
  - Processes can interact using Message start and message end event, send and recieve activities, or message throw message catch events. Process can also call other processes or include subprocesses

- Working with human task
- Three aspect define how humans interact with a business process:
  1. A HUMAN TASK in the process defines when an interaction occurs
  2. A HUMAN TASK IMPLEMENTATION define how the interaction occurs and who perform the task
  3. A WEB FORM defines the UI for task
- There are two type of HUMAN TASK :  Submit and Approve

### Develop Dynamic Process
- Dynamic Process are business process consisting of **STAGES & ACTIVITIES**
- Define the process flow at runtime i.e. Making real time decision; Carrying out relevent task
- In Process, you can design and develop ad hoc process called dynamic process. The business user work on following activities - Human Task and Structure Process
- Model a Dynamic process application with the required process artifacts :
  - Create a DP pattern such as From Scratch, To-Do List
  - Create activities that define the process
  - Segment or group activites into stages
  - Define input and output arguments for the process
  - Define data objects
- When you create an instance, the process engine ASSIGN NULL as the default values for all the data objects defined for that process.
- Model a Dynamic Process in Design Time
  - Create process roles to define responsibilities
  - Define the properties of each stage and activity
  - Finally define the condition for process completion or termination
- Use the process instance details page to view activities, start or force complete an activity. You can dorce complete an activity only if you are the process owner.


### Create and Use Micro Process
- You can divide a large complex business process into multiple reusable blocks called micro processes
- Micro processes are reusable blocks defined within seperate applications
- Smaller process with quick execution time, output feeding into the main process or parent process
- Can be invoked synchronously or asynchronously in the parent process
- To invoke a micro process from another application parent process, the micro process has to be deployed (activated) and a micro process link has to be created
- In dynamic processes, you can call only asynchronous micro process link
- You can edit the authetication and other settings for a micro process link while activating the main process

### Create Web Forms
- Web form editor is GUI based, where you can create forms, drags, drops and position various form controls in the form canvas.
- Web forms editor can be used to develop web forms in two modes: **i)Simple ii)Full**
- There are four types of **Form Controls** that can be added to the form canvas:
  - Basic Pa;ette, Advance Palette, Forms Palette and Business Types Palette
- Work with Presentation
  - presentation is a **single view of web form*
  - Presentation can be created : from Scratch, clone from previous presentation, customize from previous presentation
  - In web forms, data and controls are decoupled. You can define your control and data indeoendently

- Save Web FOrm Data
  - For every web form data object is created and associated
  - use I/O data association to create a snapshot
  - create simple expression that uses a **Form.getWebForm**
 
## Manage Application Data
- Managing data in Process Application includes defining, associating and manipulating data.
- Data is stored within a data object also called business object
- Business object are defined based on complex data types called business types reffered as business object and business exception
- A BO is a complex data type that groups together related data
- BO can be created using scratch using business object editor or automatically by importing an XSD.
- Business object are auto generated when designing forms using form-first design
- STEPS TO MANAGE DATA IN PROCESS APPLICATION
- Define business types->Create BO/ data objects-> Configure data association and transformation-> Define expression-> Create business indicators -> Define i/o arguments
- Define how data is stored and manipulated is part of the design and development of a Process Application
- Business types - such as Business objects, business exceptions, and Enum objects define the data structure used within your process application
- ---------------------------------------------------
- Business Object let you group related type sof data together to define data structure required for your process Application
- Either Create Business Object MANUALLY or base then on a XML Schema Definition (XSD).
- After defining Business Object, you can use them to define data object to store the data
- When Defining BO, the following element should be defined:
  - Modules : Modules are containers that enable you to create a hierarchical structure. Each BO must be conatined in a module. when you create a new BO, its automatically created within BusinessData modules
  - Business Objects : within a module you can define one or more BO. A BO can contain other BO 
  - Attributes : represents a characterstics of real-world concept. Attributes define particular piece of Process data that are stored and can be shared among process activities.
- DEFINE BUSINESS OBJECT USING XML SCHEMA
  - You can import business object that are based on an XML Schema (XSD) file. During the process you define the hierarchical relationship between modules and business objects.
- Data Object are the variable used to store the information used by your business processes defined during the design and implementation stage of a process
- Process -> Data Objects -> Add -> Enter name -> select type -> Create -> Close
- Business Exception and Enum objects can be defined based on complex or business data types
- Business Object defined : Based on XSD, based on FORMS, Business type explicitly
-  ASSOCIATE and MANIPULATE DATA
  - Data association and Transformation are done in Process Flow Elements such as -
  - Human task, Conditional, Timer catch events, Notification tasks, sub process tasks
  - You can use  **Expression Editor** to **evaluate and perform calculations** on data in data objects using **operator and functions**
- DATA ASSOCIATION AND TRANSFORMATION
  - Transformation is a special type of data association b/w input and output data types that don't match. Its simply maps thier type. it is reusable so configure once and use throughout.
  - You can control the execution of data association at runtime by adding condition to them in the data association editor. A data association that has been configured with conditional mapping executes at runtime only when the defined condition fulfils otherwise it fails.


### 8. Create Decision
- Decision Model in Process Application
  - Decision is a **container** in the process applications, in which **if/then rules or decision tables** are created along with other rule artifacts.When decisions are created, it is mandatory to define input and output data objects. These data objects **cannot be deleted or added after the decision is created.**
  - The data objects are used in the if/then rules and decision tables as input and output parameters, respectively.
 
  - Use the decision model framework to express a full range of automated decisions. Model your decisions as a tree of simple decisions, each automated using decision tables and simple expressions instead of production rules. Enter expressions in a simple standard expression language without worrying about quotation marks or special formatting. Then activate and use your decision models in one or more applications, and easily modify them as needed.

- Working with Decision Models
  - In a process, a Decision Model is used to determine **decision that automate** POLICY, COMPUTATIONS and REASONING
  - DM is consit of following elements:
  1. Decision and sub-Decision along with implementation logic
  2. Input data and types
  3. Associated Decision Services
  - It facilitates the modelling of complex decision as a hierarchy of simple decisions
- Steps to Create a Decision Model
  - Define a decision model which as a container holds various decision artifacts.
  - Add decisions and sub-decisions to the defined decision model.
  - Define the input data and its data type for the decisions.
  - Model the decision logic.
  - Test the decisions.
  - Create a decision service.
  - Create snapshots of the decision model and activate them.
- Creating a Decision Models
  - Processes -> Decision Models -> Create -> Create Decision Model -> Create
  - Some avaialble logic types in Decision:
  - Empty Decision, Decision Table, Expression, Context, if-then-else, function, context, relation, List
- Define EXPRESSION with Friendly Enough Expression Language (FEEL)
  - Decision Modelling and Notation (DMN) represents all decision in a Decision Model
  - FEEL is used in DMN which define expressions in a decision model
  - FEEL used in Decision Expresion has following language constructs
  - Data Type, Grammer Rule, Built-in Functions, Lists
- In process, FEEL is used to define expression within all notation of : **Decision Logic, Decision Tables**
- Data type in Decision : Text, Number, Boolean, Data and Time, Complex
- You can use bottom-up approach to define the logic within decision model
- TEST DECISION
  - Click test play icon -> Input data -> Start Test ->  View Result -> Click each green check mark -> Go Back and repeat step 1 to 3
- EXPOSE DECISION AS A SERVICE
   - To use your decision model in one or more Process Application, you must add atleast one decision service in the decision model before you deploy the decision model
   - Expand Service Pane -> Add new service -> Enter a name for decision service - > Ok -> Choose output decision and input data
- ACTIVATE DECISION AND CREATE SNAPSHOT
- DM Snapshots are read-only copies of a decision model at a particular moments
- You can -
  - Create a snapshot at any point, view the content, delete a snap, export a snap to your local file system
  - To Create and deploy a snapshot:
  - Activate-> enter name -> assign runtime version id -> select overwrite -> activate

- 
