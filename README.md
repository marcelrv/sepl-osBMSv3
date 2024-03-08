# Seplos BMSv3

Description of Seplos BMS v3 protocol

## Modbus RTU
Seplos BMS v3 uses modbus RTU protocol for reading and writing the values and settings as seen in the BMSSudio app
The individual BMSses can be addressed by the modbus Client Id. (minus 1: Client 1 in software = client id 0 in modbus)

Writing to the SPA & SCA registers will change the settings of the BMS

Settings:
speed: 19200 8N1

## Main blocks
| Block           | Adres  | Length | len(hex) | Type       | Description                                  |
|-----------------|--------|--------|----------|------------|----------------------------------------------|
| [PIA](pia.md)   | 0x1000 | 18     | 0x12     | registers  | Basic status info                            |
| [PIB](pib.md)   | 0x1100 | 26     | 0x1A     | registers  | Cell voltage and temperatures                |
| [PIC](pic.md)   | 0x1200 | 144    | 0x90     | bits/coils | Cell & other Alarms                          |
| [SPA](spa.md)   | 0x1300 | 106    | 0x6A     | registers  | Settings                                     |
| [SFA](sfa.md)   | 0x1400 | 80     | 0x50     | bits/coils | Overall alarms                               |
| [SCA](sca.md)   | 0x150D | 13     | 0x0D     | registers  | FET and onther status & setting              |
| info            | 0x1700 | 51     | 0x33     | registers  | Manufacturer, product and serialnumber info  |


## Request made by Seplos software and example response

```
client.read_input_registers(0x1700, 0x33, slave=0):
response: [22618, 18477, 17772, 25955, 21605, 25448, 8259, 28462, 11340, 29796, 16973, 21297, 13907, 12848, 12353, 11603, 20528, 13634, 0, 0, 12595, 21328, 12341, 16946, 13105, 12594, 13872, 12342, 12546, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
response (hex): 585a482d456c65635465636820436f2e2c4c7464424d53313653323030412d5350303542003133535030354232333131323630303633000000000000000000000000
string: XZH-ElecTech Co.,LtdBMS16S200A-SP05B13SP05B2311260063

client.read_input_registers(0x1301, 0x01, slave=0):
response: [16]
response (hex): 10

client.read_input_registers(0x1000, 0x12, slave=0):
response: [5236, 1301, 3800, 30400, 64, 125, 1000, 2, 3272, 2837, 3275, 3268, 2845, 2831, 0, 180, 180, 1000]
response (hex): 1474515ed876c0407d3e82cc8b15ccbcc4b1db0f0b4b43e8

client.read_input_registers(0x1100, 0x1a, slave=0):
response: [3273, 3273, 3268, 3272, 3274, 3274, 3275, 3275, 3274, 3273, 3273, 3270, 3271, 3271, 3270, 3272, 2842, 2833, 2831, 2845, 2731, 2731, 2731, 2731, 2833, 2829]
response (hex): cc9cc9cc4cc8ccaccaccbccbccacc9cc9cc6cc7cc7cc6cc8b1ab11b0fb1daabaabaabaabb11b0d

client.read_input_registers(0x1300, 0x6a, slave=0):
response: [4, 16, 5400, 5600, 5400, 5760, 4800, 4640, 4800, 4320, 3400, 3500, 3400, 3650, 3100, 2900, 3100, 2700, 2000, 1000, 500, 203, 205, 210, 100, 300, 300, 65333, 65331, 65326, 100, 65186, 300, 65236, 106, 600, 5, 3000, 205, 10, 3500, 3400, 1500, 1000, 800, 200, 30, 3201, 3231, 3231, 3281, 2781, 2751, 2731, 2631, 3231, 3281, 3281, 3331, 2761, 2631, 2731, 2581, 3201, 3231, 3281, 3331, 2761, 2731, 2731, 2631, 3581, 3681, 3581, 3831, 2831, 2731, 3231, 2731, 10, 3400, 50, 30, 960, 150, 100, 70, 50, 30400, 30400, 3800, 48, 60, 240, 10, 7, 0, 13, 0, 500, 300, 5760, 180, 65356, 5, 8]
response (hex): 410151815e01518168012c0122012c010e0d48dacd48e42c1cb54c1ca8c7d03e81f4cbcdd26412c12cff35ff33ff2e64fea212cfed46a2585bb8cdadacd485dc3e8320c81ec81c9fc9fcd1addabfaaba47c9fcd1cd1d03ac9a47aaba15c81c9fcd1d03ac9aabaaba47dfde61dfdef7b0faabc9faabad48321e3c09664463276c076c0ed8303cf0a70d01f412c1680b4ff4c58

client.read_input_registers(0x1500, 0x04, slave=0):
response: [59399, 776, 4141, 7710]
response (hex): e807308102d1e1e

client.read_coils(0x1200, 0x90, slave=0):
response: [False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, True, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, True, True, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False, False]

client.read_coils(0x1400, 0x50, slave=0):
response: [True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, True, False, False, True, False, False, False, False, False, False, False, True, True, True, True, True, True, True, False, True, True, True, True, False, True, False, False, True, True, True, True, True, False, False, True, True, True, True, True, False, False, False, False, True, True, False, False, False, True, True, False, True, True, True, True, False, True, True, False]
```
## Excel
Excel file with the tables available here [Seplos BMS v3 modbus registers.xlsx](https://github.com/marcelrv/seplosBMSv3/blob/main/Seplos%20BMS%20v3%20modbus%20registers.xlsx)

## Warning

Note: **I'm not affiliated to Seplos in any way!**

This info is explicitly provided “AS IS” without express or implied warranties, guarantees, or guarantees of correctness. 
So USE THEM AT YOUR OWN RISK! Don't complain if you broke your BMS.

This content © 2024 is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)] ![img/svg/by-nc.eu.svg](https://github.com/marcelrv/seplosBMSv3/blob/main/img/by-nc.eu.svg)


