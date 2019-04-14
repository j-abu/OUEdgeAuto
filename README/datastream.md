# EdgeAuto-datastream

## Objective 
  The datastream handles the data collection from the carloop connected to the vehicle, all the way to the node. This will handle the direction of the output for the carloop to a specific node based on the carloop's GPS position. 

## Design Scheme
  The carloop performs a handshake with the mapping node with a TCP/IP connection. Once the mapping node receives the request, it creates a unique ID for the carloop and its current session. The carloop receives this information, then process to wait for the GPS module to begin data collection. 
  After the GPS data has been ascertained, it is sent to the mapping server for evaluation. The mapping node will 
