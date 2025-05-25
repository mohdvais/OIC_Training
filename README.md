**Oracle Integration Cloud is a combination of 3 services:**

1. Integration Cloud Service (ICS/OIC)
It is a middleware which helps you application to connect with two or more system and helps in
design, monitor, and manage connections between your applications.
2. Process Cloud Service (PCS)
It helps to automate and manage business process.
It is just like Work-flow in EBS and BPM in Oracle Fusion Cloud.
3. Visual Builder Cloud Service (VBCS)
Build Mobile and Web Application visually. It can easily be merge with Oracle ERP application.


**2. Components in OIC**

. Adapters: Pre-built components that facilitate seamless connectivity between various applications and services, enabling data exchange without extensive coding.
· Agent: A lightweight service that runs on-premises to enable secure data transfer between cloud applications and on-premises systems.
. Connection: Defines the settings and credentials for connecting to various applications and services, acting as a bridge for data flow.
· Lookups: A way to manage and store reference data for use in integrations, allowing for dynamic value retrieval during data processing.
· Library: A collection of reusable components, functions, and assets that can be shared across different integrations, promoting efficiency and consistency.


**1. Adapter**


. Adapters are endpoints of any integration solution, so they can interact directly with the business applications.
· Adapters do the actual connections with application resources and manage application transactions, security, exceptions, and so on.
. It helps securely configured connection between Integration Cloud and other system using authentication with Username and password or other credentials.
· Some adapters are Oracle Cloud ERP Adapter, ATP, FTP, File, Oracle E-Business Suite, REST. SOAP. Oracle Data base. SAP etc.

**2. Agent**

· Agents are used by OIC to connect to on-prem entities such as a local database or
a local file server.
· For example, if you are using on-premise systems like EBS/SAP and also using Oracle
OIC in the same implementation, you would have to use an agent to connect to the OIC


**3. Connection**
· Connections are the various connectors that can be utilized to communicate with
external applications. Communication can be done with conventional systems like File,
FTP, etc., and also with new social media and other applications, like LinkedIn, Facebook,
Twitter, Gmail, WhatsApp etc.
· We need to create Connections by using the Adapters available.
. Connections are based on Adapters, If we want to connect with FTP server we
required FTP Adapter to make a connection with the application.


**4. Lookup**
It is used for providing mapping in integration.
We use lookups in the integration to create reusable tables that map the different terms used to describe the same item across your applications
E.g. Lookup for country code and country Name (US- United State, In - India, M- Male)


**5. Library**
In Oracle integration cloud OIC, JavaScript is used to enhance integration flows by adding custom logic and processing capabilities. It allows 
Developers to create reusable libraries for data transformations, invoke external services like APIs, Enforce business rules, and manage error
Handling. By using JavaScript, OIC integrations making complex workflows easier to manage and automate.

Here we can create functions which can be used in integration
Functions are configured in the Library editor page to be used in the orchestration canvas.

**6. Package**
Group Similar integrations: Packages allow you to group related integrations together improving organization and management.
Efficient Versioning : Packages help with managing different versions of integrations, ensuring that older versions can be maintained alongside newer ones.
Promotions Across Environments: Packages simplify the process of promoting integrations from one environment (e.g. development) to another (E.g. production)
Dependency Management: They ensure that all related components such as lookups , connections, and integrations are bundled together during migrations or updates
Streamlined Deployment : By using packages, users can deploy multiple integrations simultaneously, reducing the complexity of managing individual integration assets.



