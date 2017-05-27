# OPCModbusUAServer
An open source OPC UA server for Modbus TCP devices. The project makes use of the powerful open source NodeOPCUA (http://node-opcua.github.io/) package, combined with the jsmodbus (https://github.com/Cloud-Automation/node-modbus) package to build the OPC server.


----------

Main files in the project:

 - server.js => The entry point for the application, creates the OPC UA server, initializes the address space, and links to Modbus actions
 - modbushandler.js => Contains the Modbus communication code needed to provide Modbus actions like reads and writes for the OPC server
 - config.json => Configuration file for the application, this is how we get to know the TCP addresses of the Modbus devices, the registers we'd like to read...etc

