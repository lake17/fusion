---
title: Adding a device port into PRTG Monitoring
category: procedure
owner: george.russ@forfusion.com
created: '2024-10-21'
---

This guide explains how to add a device port into PRTG monitoring. As PRTG administrators, we are responsible for adding these sensors into monitoring. Once these sensors have been configured, we will receive alerts to the desk, and our customers will be able to check the sensors from their read-only accounts. There are many types of sensors that can be added, but for this procedure, we're only going to be focussing on switchport sensors. This is because it's the most common sensor type that we add.

## Before you start

Before you can add sensors into PRTG monitoring, ensure:

* You have a PRTG admin account.

## Adding a Port Sensor

1. Navigate to the relevant switch using the search bar in the top right of the page. You can also find the device in the "Devices" section.

   ![image-20241018135213841](../../../assets/images/image-20241018135213841.png)  ![image-20241018135424427](../../../assets/images/image-20241018135424427.png)

2. Once you've found the device, you'll be greeted with the main device page. Here you will find all the sensors that are being monitored on the device.   ![image-20241018135830685](../../../assets/images/image-20241018135830685.png)

3. Click the "add Sensor" button on the left of the page.

   This will open the "add sensor type" page where we can add many different types of sensors.

   ![image-20241018140544050](../../../assets/images/image-20241018140544050.png)

4. Choose the sensor type "SNMP traffic" by clicking the title of the sensor, or the small addition symbol.

   ![image-20241018141030980](../../../assets/images/image-20241018141030980.png)

5. Once the page has loaded, locate and click on the port you want to add to monitoring.

   There are multiple pages that you can flick through.

   ![image-20241018141602364](../../../assets/images/image-20241018141602364.png)

6. Set the Connection Status Handling option to "Show down status for all disconnected states".

   **<u>This is important as we don't want to ignore disconnected states or ports that have been deactivated manually.</u>**

   Additional channels are optional. If a port is needed to be closely monitored, adding channels for discards and errors can be useful. Most of the time, these can be left alone.

   ![image-20241018142145098](../../../assets/images/image-20241018142145098.png)

7. Create the sensor by clicking the "Create" button. This will take you back to the device overview page.

   ![image-20241018142349232](../../../assets/images/image-20241018142349232.png)

8. Locate the new sensor which will appear at the bottom of the sensor list.

   For housekeeping reasons, the sensor should be moved to it's correct numerical position based on the port number. Use the multi-directional arrow on the sensor to drag it to it's correct position.

   ![image-20241018142532482](../../../assets/images/image-20241018142532482.png)

9. Confirm the sensor is green and passing traffic by clicking the Sensor description. This will open the Sensor overview page where you can check live and historic data on the sensor.

   ![image-20241018143027204](../../../assets/images/image-20241018143027204.png)  

10. Email the customer back confirming that you've added the sensor into PRTG monitoring.
11. Give yourself a pat on the back and grab a brew.

## See also

* PRTG Manual: Add a Sensor

  * <https://www.paessler.com/manuals/prtg/add_a_sensor>

* YouTube tutorial on manually adding a sensor

  <iframe src="https://www.youtube.com/embed/03gWnhgq20s" title="PRTG Tutorial - How to Add a Sensor Manually" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
