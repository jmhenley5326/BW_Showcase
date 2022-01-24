# BusinessWorks Showcase
These projects contain various BusinessWorks examples showcasing functionality within the BusinessWorks 6 environment. There are many more examples available in the BusinessWorks 6 installation. These are intended to be more verbose and demo oriented.

# Projects
## Showcase_Basic
This project contains basic functionality that comes out of the box with BusinessWorks. Each example contains Notes and comments on what is happening. These are intended to show very simple reference implementations of various pieces of functionality that can then be used to create more complex business processes. For more information please look at the samples provided with the BW6 installation.

### Project Pre-Reqs
* BusinessWorks 6.4
* MySQL configured as described below (Other databases can be used. It is left to the user to adjust the JDBC Shared Resource and ensure all the required objects are available)
* SMTP Account- The SMTP Shared Resource must be configured for an account the user has access to
* EMS Instance- Currently configured for local instance but can be changed as needed

### showcase_basic.module.services
A simple Rest and SOAP implementation
![svc_produce](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/Rest_Service.png?raw=true)
### showcase_basic.module.consumers
Consumers of the Rest and SOAP services
![svc_consumer](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/Svc_Consumer.png?raw=true)
### showcase_basic.module.msg.producers
Basic JMS Queue and Topic message publishers
![msg_pub](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/Msg_Producer.png?raw=true)
### showcase_basic.module.msg.consumers
Queue and Topic listeners
![msg_sub](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/Msg_Consumer.png?raw=true)
### showcase_basic.module.mapping
Shows a simple mapping from one XSD to another as well as from an XSD to a Flat File format
![map](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/Mapper.png?raw=true)
### showcase_basic.module.files
Examples of writing files and listening for file events such as create, modify and delete
![files](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/File.png?raw=true)
### showcase_basic.module.exception
Very basic illustration of catching and handling exceptions within a process
![exception](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/Exception.png?raw=true)
### showcase_basic.module.choreography
A series of processes that combine many of the basic examples and combines them into a business choreography. This also shows how to encapsulate a set of activities into a subprocess for reuse.
![orch1](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/Orch1.png?raw=true)
![orch2](https://github.com/jmhenley5326/BW_Showcase/blob/master/screenshots/Orch2.png?raw=true)
### showcase_basic.module.sandbox
Use this module to create Processes live and show how they are built

### Database Configuration
Configure MySQL as follows:
* Create a user named bw_showcase
* Create the schema provided in the "db_schemas" folder at the root of this repository for this project
* Ensure the bw_showcase user has appropriate permissions for this new schema
* Test the JDBC Shared Resource and make adjustments to the JDBC URL and security credentials as required

## Showcase_Patterns
WORK-IN-PROGRESS -
This project contains sample implementation integration patterns

## Showcase_Social
WORK-IN-PROGRESS - 
This project covers interactions with social networks including Twitter and Facebook.
