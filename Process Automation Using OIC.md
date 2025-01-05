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
- Using the QuickStart Apps, developers can easily build process applications without any knowledge on BPMN. (Business Process Modeling Notation)
- On creating an application based on a QuickStart App, a copy of the pre-built application will be created with the name of the process application being created
- A process application can be created from the Process Application home page by clicking on Create button. It Shows THREE option
  - 1. To create an application based on QuickStart App, choose the option Start with a QuickStart.
    2. To create an application from scratch, choose the option Create an Application.
    3. To create an application based on already created application
- SNAPSHOT : It is a read-only copy of an application at a particular moment. You can't open them for editing. You can Create a snapshot from the last published version of an application.
- You can view the content of snapshot
- Export an application based on snapshot - Deploy and application and Delete
- Participant with owner or editor permission can create a snapshot
- APPLICATION ROLES
- Use application roles to model the users, groups, or system that perform the work your business process represent. The predefined roles are: Process Owner, Reviewer, Analytics Viewer, Automatic Handler


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
