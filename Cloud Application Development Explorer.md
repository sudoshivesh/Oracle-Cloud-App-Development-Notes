# Cloud Application Development Explorer
    Introduction to Oracle's Cloud Application Development Platform
    Application Development Services
    Application Deployement Services
    Developer Productivity Services
    Become a Cloud App Developer

    Sir guidance: 

- Key Feature of Oracle Cloud Platform (Why to choose OCP)
    - Open: In term of choosing language/open source technology. Oracle Java SE, Python, Ruby, PHP, Oracle javascript Extension Tool (JET)
    - Modern: In tern of architectural styles/ tools (Agile/DevOps)
    - Easy: in terms of ease of integration
- it offers a **second genration cloud**

- ![image](https://github.com/user-attachments/assets/62b39ba7-ea79-412f-9ceb-1ce3396ca163)

- Machine Learning Models supported in Oracle cloud
    - Jupyter, Tensorflow, PyTorch, Plotly, Matplotlib
- Modern Application Development Platform supported by Oracle Cloud
    - Kubernetes, Docker, Terraform, Ansible, OCI, Oracle WebLogic Server
    - Kubernetes is an oracle managed container orchestration service that help to build modern application
    - OCI provide realtime elasticity for enterprise application
    - Docker is a set of PaaS products that uses OS level visualization to deliver software package
    - Terraform is a tool that allows the user to programmatically manage version and infrastructure
    - Ansible is the simples way to automate apps and infrastructure
    - Oracle WebLogic Server is a unified and extensible platform for developing, deploying and running enterprise applications such as Java for on premises and in the cloud
 
- Oracle Application Development Tools
    - Oracle Visual Builder Studio
    - Oracle Digital Assistant
    - Oracle REST Data Services
    - Oracle SQL Developer
    - Agile
- Oracle Cloud Application Development Platform Features
    - Continious Integration, Fast and Easy, Ease of Building Application, Migrating legacy Application
    - Continious Development, Faster time to market and higher productivity

- Type of Development
    - Enterprise Application Developer
    - Cloud Native Developer
    - Mobile Application Developer
    - API Developer
    - Blockchain Developer
    - Low-Code "Citizen" Developer

|App & Service Deployment|Application Development|Developer Productivity|
|-|-|-|
|WLS|Mobile Hub|API Gateway|
|Computer|Visual Builder|Visual Builder|
|Containers|Blockchain & Digital assistant||


### Application Development Services
- Four major application development cloud services
    - Visual Builder Studio
    - Oracle Mobile Hub
    - Oracle Digital Assistant
    - Oracle Blockchain

- Applicationn Deployment Services
    - Oracle Cloud Infrastructure (OCI)
    - WebLogic Server for OCI
    - Microservice and Containers
    - Container Engine for Kubernetes (OKE)
### ------------------------------------------------------------------------------------------
### Application Deployment Service

- Oracle Cloud Interface
    - It is a set of Complementary cloud services in Oracle Genration 2 Cloud. It can be used to configure many different components required for Oracle Cloud.
    - OCI also enables the user to build and run a wide range of applications and services in a highly available hosted environment.
    - OCI offers high-performance physical hardware and storage devices. It also offers a flexible overlay of virtual networks.
    - Using the resources available in OCI, a user can set up, configure and use various Cloud Services.
    - When you sign in to the OCI, you can see this OCI Console homepage.
    - Various categories of Cloud service accessible via the console: Core Infrastructure, Database, Platform, AI, Monitoring and diagnostics.
 
- More about OCI
    - OCI is hosted as region and availability domain. OCI is organised as region, domain, tenancy and compartment.
    - Sabse uper OCI, uske niche REGION (1...N), uske niche DOMAIN(1...N), uske nice TENANt(1..N), and sabse niche COMPARTMENT(1...N)
    - There is many domain in 1 region, and there is many Tenant in 1 Domain and there is many Compartment in 1 Tenant
    
    
    - A region is a localized geographical area composed of one or more availablity domains. Most OCI resources are either **region-specific** or **availability domain-specific**
    - There are **20+ region** available in the OCI. These region are in the US, UK, Canada and Japan
    - Availability Domains : An **availability domain** is one or more data centers located within a region. They are isolated from each other, fault tolerant, and very unlikely to fail simultaneously. They do not share infrastructure such as power or cooling or the internal availability domain network. Hence, a failure in one domain is unlikely to impact the availability of the others. All the domains in a region are connected to each other by a low-latency and high-bandwidth network.
    - Talking of **tenancy**, when a user signs up for OCI resources, Oracle creates a tenancy for the user organization. A tenancy is a secure and isolated partition within OCI where a user can create, organize, and administer the cloud resources. All the resources for hosting the client applications are created within the tenancy. The administrator can use the OCI console to manage the tenancy.
    - On compartments, a compartment is a logical group within a domain and not a physical container. When a user signs up for OCI, Oracle creates a tenancy, which is the group compartment that holds all the Cloud resources. The compartment contains a collection of related resources such as instances, virtual cloud, networks, log volumes, and many more. The compartment allows the user to organize and control access to cloud resources. It can be accessed only by certain groups who've been given permission assigned by an administrator. The administrator can control the compartment by setting up the policy. A user can create additional compartments within the tenancy and set up corresponding policies to control the access of resources in each compartment.

- OCI Compute
    - OCI Compute is one of the basic components that's needed for setting up the application containers and domain. OCI Compute enables us to choose the required hardware for the business application. OCI Compute lets the user provision and manage compute hosts, known as instances. A user can launch instances that are needed to meet the application computing power required for the application. An administrator can attach and detach volumes and can terminate the instance.
    - OCI offers both **bare metal and virtual machine instances** for setting up the Cloud environment for the client. **Bare metal** a bare metal compute instance gives the user dedicated physical server access for very high performance and strong isolation. **Virtual machine** a virtual machine is an independent computing environment that runs on top of physical bare metal hardware.
    - The virtualization makes it possible to run multiple virtual machines that are isolated from each other. Virtual machines are ideal for running applications that do not require the high performance and resources of an entire physical machine.

- Compute shapes (Standard, Dense IO, GPU, HPC)
    - Administrators can create a compute instance based on the most appropriate type of shape. The instance characteristics are based on the number of CPUs, amount of memory, and network resources. The shape-defined CPU, amount of memory, and related network resources.
    - **Standard shapes** are designed for general-purpose workloads. It is suitable for a *wide range of applications* and use cases. Standard shapes provide a balance of course, memory, and network resources. Standard shapes are available with Intel or AMD processors.
    - **Dense IO** shapes are designed for large databases, big data workloads, and applications that require high performance local storage. An example could be *share market data transaction.*
    - **GPU shapes** are designed for hardware-accelerated workloads. GPU shapes include Intel CPUs and Nvidia graphics processors. An example is a *graphic-intensive application like Google Maps.*
    - **High performance computing shapes** or HPC shapes are designed for high performance computing workloads that required high frequency processor calls and cluster networking for massively parallel HPC workloads. High performance computing shapes are available for bare metal instances only. Examples include data-intensive *banking transaction applications.*

- WebLogic Server
    - Oracle WebLogic Cloud is available as a set of applications in the OCI marketplace. WebLogic Server is configured by using OCI. The components required to create WebLogic server domain resources, like compute instances, networks, and load balancers, are configured by using the OCI interface.
    - Business applications created by using Java application can be deployed by using the WebLogic Server. The configured WebLogic Server stack with deployed business applications can be managed and monitored by using OCI.
    - WLS provides a modern development platform for building and deploying applications. It also provides a runtime platform for high-performance and availability
    - WLS implementation has many Oracle products, such as SOA, Identity Management, Grid Infrastructure, Business Intelligence, Web Center, and Enterprise Manager.

- WLS Edition
    - WLS OCI Marketplace supports three editions of Oracle WLS Server
    - Oracle WLS Standard Edition, Enterprise Edition, Oracle WebLogic Suite
    - WebLogic Server **Standard Edition** has a minimum of Oracle products required for configuring the WebLogic domain. It includes Enterprise Pack for Eclipse. WebLogic Server Standard Edition also has a license for SE edition of Java.
    - Oracle WebLogic Server **Enterprise Edition** includes all features and benefits of Oracle WLS Standard Edition, clustering for high-availability and scalability of Java resource and applications, and Oracle Java SE Advanced
    - The **most powerful and complete edition is Oracle's WebLogic Suite**, which includes all features and benefits of Oracle WLS Enterprise Edition plus Oracle Coherence for increased performance and scalability, Active GridLink for RAC, which enables advanced database connectivity.
 
    - ![image](https://github.com/user-attachments/assets/84b1aaac-7e16-49d1-b266-a19e94da5557)


- Component of WLS
    - Two Compute instance, Three WLS, One Admin Server, two managed server, one load balancer, key management is configured with a vault
    - The domain has a database with GRF schemas. As you see, the stack also has one bastion host. The bastion host is configured for WLS private subnets. The bastion host enables controlled access from public networks.
    - The Oracle WebLogic Server domain consists of one administration server and one or more managed servers to host the Java application deployments.
    - OCI Component comprise Oracle WL Cloud. they are : Oracle WLS, Marketplace, Resource manager, Compute, Virtual Cloud Network, Load balancer, Database, key management, Identity


- Microservice and Containers
    - Cloud native apps are created with microservices architecture. Each application is a collection of small services. Each runs on its own process and communicates with a lightweight mechanism, often as an HTTP resource API. The microservices are built around business requirements and can be deployed independently.
    - Each microservice can be deployed, upgraded, scaled, and restarted independent of other services in the application by using an automated system, enabling frequent updates to live applications without impacting any customers.
    - Five characteristics of microservices. They are highly **maintainable and testable, independently deployable, organized around business capabilities, loosely coupled, and owned by a small team.**

- Container
    - A container is a standard unit of software that packages up the code and all its dependencies. Containers hold components such as executables, binary code, libraries, and configuration files. Container hold all the component that are needed to run the application
    - Containerization of applications in cloud computing ensures reliability, consistency, and speed in the distributed platform environment. Applications are safer in containers, and they provide the strongest isolation capabilities. A single container can run small microservices or large software applications.

- Cloud Native Application
    - Container-based application packaging and deployment was initially started by Google
    - Container-based application deployment can be implemented using **Oracle Container Engine for Kubernetes, OKE.**
    - Cloud native applications are packaged as containers, a container in which is a lightweight, standalone, executable package of software that includes everything needed to run an application. That is code, runtime, system tools, system libraries, and settings.
    - Containers are for both efficiency and speed compared with standard virtual machines. They are highly accessible, scalable, easily portable from one environment to another and fast to create or tear down, making them ideal for building and learning applications composed of microservices.

- WHY THE NEED FOR CONTAINERIZED APPLICATION DEPLOYMENT
    - It implements environmental consistency across development, testing, and production. It is loosely coupled, distributed, and elastic liberated microservices.
    - Applications are broken into smaller independent pieces, and it can be deployed and managed dynamically. It enables clear demarcation of development and operational challenges.
    - It can be implemented on different operating systems like Ubuntu, RHEL, or OS on-premises, on major public clouds, and anywhere else
    - It increases ease and efficiency of container image creation compared to VM images.
    - It also enables application-centric management and resource isolation and utilization, predictable application performance with high efficiency and density.
    - Agile application creation and deployment

- ORACLE CONTAINER ENGINE FOR KUBERNETES (OKE)
    - This is a fully managed, scalable, and highly available service that you can use to deploy your containerised applications to the cloud.
    - Use OKE when your development team wants to reliably build, deploy, and manage cloud native applications.
    - You access the OKE cloud service to define and create Kubernetes clusters using the OCI Console with that or the REST API.
    - Then you can access the created cluster directly using the Kubernetes command line, the Kubernetes dashboard web app, or the Kubernetes API.
    - OKE is integrated with OCI Identity and Access Management, which provides easy authentication with the native US identity functionality.

- WHY TO USE OKE?
    - reducing complexity as well as the time involved
    - eliminating the need to integrate Kubernetes with a registry
    - built-in processes for container lifecycle management
    - OKE enables developers to get started and deploy containers quickly
    - It provide DevOps teams visibility and control for Kubernetes management.
    - OKE combines production-grade container orchestration of open Kubernetes with control, security, identity access management, and high predictable performance of Oracle's generation 2 Cloud Infrastructure.

### ------------------------------------------------------------------------------------------
### Developer Productivity Series (Cloud Services that will help enrich the development process)
- Key Component of Visual Builder Studio
    - Two Cloud Services that will help enhance developer productivity **Oracle Vision Builder Studio and Oracle API Gateway.**
    - Key Component of VBS (Visual Builder Studio) : Organization, Project, VB Studio Designer, WorkSpace, Git Repository, Maven Repository, Job, Visual Application, Data

    - Organization : the topmost entity in the project structure of VB Studio
    - Project: a collection of VB Studio features. You use a project to host source code files, track issues, collaborate on code, build and deploy your applications. A project can host multiple Git repositories.
    - VB Studio Designer: Browser based development environment
    - WorkSpace : all work in VB Studio is done in the context of WorkSpace, a private area where you can work on visual applications.
    - Git Repository: an open source code management and distributed motion control tool to host source code files.
    - Maven Repository : a hosted binary repository to store build artifacts, library files, and dependencies from Maven applications.
    - Job : a configuration that defines that application's builds. You can create a job to perform various actions, such as package artifacts, branch end commands, run unit test scripts, and deploy application artifacts.
    - Visual Application: a responsive web or native mobile application developed by using VB Studio's browser-based development environment.
    - Data: data for visual applications can come from a database in the form of business objects, Oracle REST services or external REST services.

- Manage the Application Development Cycle Part 1
    - Application Lifecycyle management : plan, develop, collaborate, build, integrate with external software, import-export project data, and project data
    - Plan : The plan activity in Visual Builder enables the user to manage environments, track issues, and manage Agile boards
    - ```
      - Environment : you can access and manage the project's environment, that is create and delete environments, add or remove service instances from existing environments, update the details of the environment, view the details of its service instances, and view deployments.
      - Issues : To track and manage tasks, defects, and features
      - Agile Board :  To manage and update issues and help plan your team's workflow.
      ```
    - Develop : 
    - ```
      - Git Repositories : a source code management and distributed version control tool the host source code files. A project can host multiple Git repositories
      - Designer : an editing and publishing environment that you use to create web or mobile applications or to customize your Oracle Cloud applications through application extensions.
      - Maven : a hosted binary repository to store build artifacts, library files, and dependencies for Maven applications. Use the project's Maven repository for managing binary files and dependencies.
      ```
    - Collaborate
    - ```
      - Merge Request : you may require team members to create a merge request for each branch of the Git repository and ask reviewers to review and approve the code
      - Wiki : This is a built in Wiki system to help your team alter and manage Wiki pages.
      - Snippets : Snippets to share reusable pieces of source code. A Snippet could include a small block of usable source code or text that could be incorporated into larger modules.
      ```
      
