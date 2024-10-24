---
title: Cable Test Procedure
category: procedure
owner: george.russ@forfusion.com
created: "2024-10-18"
---

This guide explains how to carry out a cable test. A cable test is carried out to test the condition of the cable remotely. These tests are useful for troubleshooting ethernet ports for a physical layer problem with the cabling, patching or RJ45 connections.

## Before you start

Before you begin, ensure:

* You have Command Line Interface (CLI) access to the switch that the cable is connected to.
  * i.e. Catalyst Center or SecureCRT

* You are only testing ports using Ethernet cabling.
  * This will not work on Fibre ports.

* You know the Switch and port you would like to test (Obviously)

## Cable test

1. Navigate to the switch's CLI

   note: If you do not have SecureCRT, you can find the switch in Catalyst Center and navigate to either Device360 or Device Details. From there, you can access the CLI via "Run Commands".

   ![](../../../assets/images/image-20241016120235746.png)

2. Once in the CLI, run the following command to start the cable test:

   ```txt
   test cable-diagnostic tdr interface {interface of your choice}
   # This command can be shortened to "test cab tdr int {gx/x/x}".
   ```

3. Wait for about 5 to 7 seconds for the test to run.

   ![](../../../assets/images/image-20241016121610991.png)

4. Run the command the following command to show the result of the TDR test:

   ```txt
   show cable-diagnostic tdr interface {interface of your choice}
   # Can be shortened to "show cab tdr int {gx/x/x}".
   ```

   ![](../../../assets/images/image-20241016121641018.png)

5. Read results and send to client if necessary.

   Note: A guide on reading cable test results will be created and link pasted in the "See also" section. For now, I'll post a brief description of the results and copper pair functions below:

   ![](../../../assets/images/image-20241016122756217.png)

   ![](../../../assets/images/image-20241016122859385.png)

## See also

* An explanation on TDR cable test will created in the Knowledge Base. A link will be shown here once complete.
* <https://community.cisco.com/t5/networking-knowledge-base/how-to-use-time-domain-reflectometer-tdr/ta-p/3119327> - This is a great forum explaining the TDR cable test on Cisco switches
