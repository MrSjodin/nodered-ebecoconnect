# Node-RED flow for EbecoConnect
The flow is used in order to integrate EbecoConnect floor-heating thermostats into Home Assistant through Node-RED.

**Pre-reqs:**

 - An active EbecoConnect account with access to username (e-mail) and password. 
 - Home Assistant variant of choice
 - Node-RED configured for connecting to Home Assistant
 - MQTT broker
	 - Configured as an integration in Home Assistant with discovery
	 - Configured as a configuration node in Node-RED

**Edits needed:**

 - Set the username and password in the node 'Set Auth Parameters' under the Authentication part
 - In the Change nodes under the "Check if climate devices are already set" section, modify the ID with the correct one fetched from EbecoConnect API
 - In the Funcion nodes "BaseParameters...." under the "Update the Thermostat...." sections, modify the ID with the correct one fetched from EbecoConnect API
 - ..and probably someplace else I forgot about..
 

**Other notes:**

 - It's a work in progress. This initial version is functioning although pretty ugly - I'm aware of that. 
 - You set the username and password in the node 'Set Auth Parameters' under the Authentication part. 
 - In this example flow I have integrated two thermostats. Copy or remove nodes as needed. 
