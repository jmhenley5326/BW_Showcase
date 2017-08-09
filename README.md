# BW_Showcase
These projects contain various BusinessWorks examples showcasing functionality within the BusinessWorks 6 environment.

# Projects
## Showcase_Basic
This project contains basic functionality that comes out of the box with BusinessWorks. Each example contains Notes and comments on what is happening. These are intended to show very simply reference implementation of various pieces of functionality that can then be used to create more complex business processes

### Project Pre-Reqs
* BusinessWorks 6.4
* MySQL configured as described below (Other databases can be used. It is left to the user to adjust the JDBC Shared Resource and ensure all the required objects are available)
* SMTP Account- The SMTP Shared Resource must be configured for an account the user has access to

### showcase_basic.module.services
A simple Rest and SOAP implementation
### showcase_basic.module.consumers
Consumers of the Rest and SOAP services
### showcase_basic.module.msg.producers
Basic JMS Queue and Topic message publishers
### showcase_basic.module.msg.consumers
Queue and Topic listeners
### showcase_basic.module.mapping
Shows a simple mapping from one XSD to another as well as from an XSD to a Flat File format
### showcase_basic.module.files
Examples of writing files and listening for file events such as create, modify and delete
### showcase_basic.module.exception
Very basic illustration of catching and handling exceptions within a process
### showcase_basic.module.choreography
A series of processes that combine many of the basic examples and combines them into a business choreography. This also shows how to encapsulate a set of activities into a subprocess for reuse.

### Database Configuration
Configure MySQL as follows:
* Create a user named bw_showcase
* Create the schema provided in the "db_schemas" folder at the root of this repository for this project
* Test the JDBC Shared Resource and make adjustments to the JDBC URL and security credentials as required
