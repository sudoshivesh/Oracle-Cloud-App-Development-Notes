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
