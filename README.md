# Node-RED flow for EbecoConnect
The flow is used in order to integrate EbecoConnect floor-heating thermostats into Home Assistant through Node-RED.

**Pre-reqs:**

 - Home Assistant variant of choice
 - Node-RED configured for connecting to Home Assistant
 - MQTT broker
	 - Configured as an integration in Home Assistant with discovery
	 - Configured as a configuration node in Node-RED

**Other notes:**

 - It's a work in progress. This initial version is functioning although ugly. 
 - In this example flow I have integrated two thermostats. Copy or remove nodes as needed. 
