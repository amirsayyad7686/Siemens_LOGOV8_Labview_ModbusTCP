# Siemens_LOGOV8_Labview_ModbusTCP
Connection between LOGOV8 with Labview over modbust TCP/IP protocol

![siemens-logo](https://github.com/amirsayyad7686/Siemens_LOGOV8_Labview_ModbusTCP/assets/78236642/c8f0b8e8-e270-4fba-b75c-2bf68d6bd732)

Program LOGO (FBD) at first here is an example with 2 output coils & 2 inputs & 2 memories and 1 analog input

![logosoft](https://github.com/amirsayyad7686/Siemens_LOGOV8_Labview_ModbusTCP/assets/78236642/1aa94516-9e92-4653-9922-378435bcfc26)

at first we should give the LOGO permission to accept LAN connection for using Labview over Modbus for accepting permission in ethernet connection page and general tab we can define one or several acceptable connection for using further

![logosoft2](https://github.com/amirsayyad7686/Siemens_LOGOV8_Labview_ModbusTCP/assets/78236642/a5b0288b-694f-4fd6-b475-0d8a0e99db88)

every FBD blocks in program have a unic address in modbus connection here we can access the list in ethernet connection 

![logosoft3](https://github.com/amirsayyad7686/Siemens_LOGOV8_Labview_ModbusTCP/assets/78236642/bb78cc01-f625-402f-a84e-cced2fe8c51c)

now every things are ready we should download FBD on LOGO and then making a connection on Labview using Modbus lib (NI Modbus Library)

![labview](https://github.com/amirsayyad7686/Siemens_LOGOV8_Labview_ModbusTCP/assets/78236642/0229fab4-98df-4f56-b121-4110484960ff)

1- at first create modbus instance and point the ip address of LOGO and also point port (default is 502)

2- write single coil block is for trigger a coil(Q) on LOGO by sending coil address like Q1 start with 8192 & Q2 = 8193 &...
for example if write 8192 on write single coil input then toggle the button coil Q1 will ON

3- read dicrite 

