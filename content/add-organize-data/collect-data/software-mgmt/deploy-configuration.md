---
uid: DeployConfig
---

# Deploy a system configuration

After you export a system configuration, you have to manually deploy the configuration to the edge device in the field.

For details on how to deploy a configuration, see the specific system product documentation: 

 - [AVEVA Adapter for Azure Event Hubs](https://docs.aveva.com/bundle/pi-adapter-azure-event-hubs/page/configuration/configuration.html)
 
 - [AVEVA Adapter for BACnet](https://docs.aveva.com/bundle/pi-adapter-bacnet/page/configuration/configuration.html) 

 - [AVEVA Adapter for DNP3](https://docs.aveva.com/bundle/pi-adapter-dnp3/page/configuration/configuration.html)

 - [Edge Data Store](https://docs.aveva.com/bundle/edge-data-store/page/configuration/configuration.html)

 - [AVEVA Adapter for Modbus TCP](https://docs.aveva.com/bundle/pi-adapter-modbus/page/configuration/configuration.html)
 
 - [AVEVA Adapter for MQTT](https://docs.aveva.com/bundle/pi-adapter-mqtt/page/configuration/configuration.html)

 - [AVEVA Adapter for OPC UA](https://docs.aveva.com/bundle/pi-adapter-opc-ua/page/configuration/configuration.html)

 - [AVEVA Adapter for RDBMS](https://docs.aveva.com/bundle/pi-adapter-rdbms/page/configuration/configuration.html)

 - [AVEVA Adapter for Structured Data Files](https://docs.aveva.com/bundle/pi-adapter-structured-data-files/page/configuration/configuration.html)

After deploying the configuration, manually update the configuration file on the device to replace any mustache tokens used as place holders for secrets with the actual secrets. Then, to have an accurate record of the configuration, import the configuration file, including any modifications made in the field except secrets, to the corresponding system twin in AVEVA Data Hub.

## Data source scenarios

If you need to access multiple data sources on the same device, you need to differentiate the data sources. You can use the following options to identify the data sources:

 - Static IP address

 - Fully qualified device name

We recommend you review your specific scenario with your network administrator to determine the appropriate configuration for your use case.
