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

Agenda : OIC Session :Day 2


Available integration patterns



When you begin creating an integration, the first step is selecting the appropriate pattern based on the integration requirements. 
These patterns help streamline development and ensure that integrations are built efficiently to handle specific use cases.

In Gen2, Oracle integration cloud (OIC) offers six (6) integration patterns.

	1. Basic Routing
	2. Publish to OIC
	3. Subscribe to OIC
	4. File Transfer
	5. Scheduled Orchestration
	6. App Driven Orchestration

In Gen 3, Oracle Integration Cloud offers three integration patterns

	1. Application
	2. Schedule
	3. Event

Basic Routing integration: Basic Routing integration is created initially with empty trigger and invoke connections.
This design is adopted with the use case, when we have a requirement of integration business entity of one system to another,
with their mapping data structure for request and response.

We can create only single routing expressions in basic routing integration, In case we have a requirement for creating multiple routing expressions,
We should use the Orchestration Design pattern (App Driven Or Schedule).

Schedule Orchestration integration

This pattern is ideal for use cases where integrations need to be run on a scheduled basis, such as batch processing at a specific time.
By leveraging the scheduled orchestration pattern, you can build robust and reliable integration that operate seamlessly according to  your organizations
Scheduling needs.
Scheduled orchestration pattern allows you to develop an integration that can run on the pre-defined frequency and can be executed on an ad-hoc basis

App driven Orchestration integration

App driven Orchestration pattern is a multi-step pattern, allows invoking multiple applications in a single flow, doing a for-each loop, if else logic, apply complex logic, etc,
Integrations are triggered by an event or a business object change, such as a Salesforce outbound message.
Supports decision making, loops, parallel processing, and state management for handling complex business scenarios.


Event (Publish/Subscribe) Integration

	· In Gen3, event are are used to Publish message.
	· Using  this, Systems can publish events and other integrations can subscribe to these events to execute specific actions.
	· Event pattern allows you to subscribe to an event that is published by a producer.
	· The subscribing integration event is triggered when the integration Publishing the event is run.
	· Multiple integrations can subscribe to the same published event.
	
	

Schedule Integration

Scheduled Integration in Oracle integration cloud (OIC) is a type of integration that runs at predefined intervals or on ad-hoc basis.
Oracle integration Cloud (OIC) allows up to five scheduled parameters in scheduled integrations. These parameters can be used to dynamically control the behavior of the integration when it runs.
Schedule parameters can have value length upto 256 characters.
A scheduled integration can run for a maximum duration of 6 hours.
Scheduled integration is asynchronous integration and it doesn't returns any value.
We cannot schedule integration recurrence less than 10 minutes using scheduler.
iCall expression will be used to schedule integration below 10 minutes.

![image](https://github.com/user-attachments/assets/97f82beb-15ae-4400-a594-d8224db7ee2c)




