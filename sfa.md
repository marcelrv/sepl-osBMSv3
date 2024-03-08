# SFA table

Alarms

| **"ID"** | **rtuAddress** | **description zh-CN** | **description en-US**                       | **bit** | **bitIndex** | **byteIndex** | **isDisplay** | **datatype**        |
|----------|----------------|-----------------------|---------------------------------------------|---------|--------------|---------------|---------------|---------------------|
| 1        | 1400           | 单体高压告警                | Cell high voltage alarm                     | 1       | 0            | 0             | 1             | SwitchParameterInfo |
| 2        | 1401           | 单体过压保护                | Cell over voltage protection                | 1       | 1            | 0             | 1             | SwitchParameterInfo |
| 3        | 1402           | 单体低压告警                | Cell low voltage alarm                      | 1       | 2            | 0             | 1             | SwitchParameterInfo |
| 4        | 1403           | 单体欠压保护                | Cell under voltage protection               | 1       | 3            | 0             | 1             | SwitchParameterInfo |
| 5        | 1404           | 总压高压告警                | Battery high voltage alarm                  | 1       | 4            | 0             | 1             | SwitchParameterInfo |
| 6        | 1405           | 总压过压保护                | Battery over voltage protection             | 1       | 5            | 0             | 1             | SwitchParameterInfo |
| 7        | 1406           | 总压低压告警                | Battery low voltage alarm                   | 1       | 6            | 0             | 1             | SwitchParameterInfo |
| 8        | 1407           | 总压欠压保护                | Battery under voltage protection            | 1       | 7            | 0             | 1             | SwitchParameterInfo |
| 9        | 1408           | 充电高温告警                | Charge high temperature alarm               | 1       | 0            | 1             | 1             | SwitchParameterInfo |
| 10       | 1409           | 充电过温保护                | Charge over temperature protection          | 1       | 1            | 1             | 1             | SwitchParameterInfo |
| 11       | 140A           | 充电低温告警                | Charge low temperature alarm                | 1       | 2            | 1             | 1             | SwitchParameterInfo |
| 12       | 140B           | 充电欠温保护                | Charge under temperature protection         | 1       | 3            | 1             | 1             | SwitchParameterInfo |
| 13       | 140C           | 放电高温告警                | Discharge high temperature alarm            | 1       | 4            | 1             | 1             | SwitchParameterInfo |
| 14       | 140D           | 放电过温保护                | Discharge over temperature protection       | 1       | 5            | 1             | 1             | SwitchParameterInfo |
| 15       | 140E           | 放电低温告警                | Discharge low temperature alarm             | 1       | 6            | 1             | 1             | SwitchParameterInfo |
| 16       | 140F           | 放电欠温保护                | Discharge under temperature protection      | 1       | 7            | 1             | 1             | SwitchParameterInfo |
| 17       | 1410           | 环境高温告警                | High ambient temperature alarm              | 1       | 0            | 2             | 1             | SwitchParameterInfo |
| 18       | 1411           | 环境过温保护                | Over ambient temperature protection         | 1       | 1            | 2             | 1             | SwitchParameterInfo |
| 19       | 1412           | 环境低温告警                | Low ambient temperature alarm               | 1       | 2            | 2             | 1             | SwitchParameterInfo |
| 20       | 1413           | 环境欠温保护                | Under ambient temperature protection        | 1       | 3            | 2             | 1             | SwitchParameterInfo |
| 21       | 1414           | 功率高温告警                | Power high temperature alarm                | 1       | 4            | 2             | 1             | SwitchParameterInfo |
| 22       | 1415           | 功率过温保护                | Power over temperature protection           | 1       | 5            | 2             | 1             | SwitchParameterInfo |
| 23       | 1416           | 电芯低温加热                | Cell temperature low heating                | 1       | 6            | 2             | 1             | SwitchParameterInfo |
| 24       | 1417           | 电芯电压失效                | Cell voltage fault                          | 1       | 7            | 2             | 0             | SwitchParameterInfo |
| 25       | 1418           | 强制输出功能                | Forced output                               | 1       | 0            | 3             | 1             | SwitchParameterInfo |
| 26       | 1419           | 散热开启                  | Heat dissipation turned on                  | 1       | 1            | 3             | 1             | SwitchParameterInfo |
| 27       | 141A           | 容量灯常亮                 | CapLeds idle display                        | 1       | 2            | 3             | 1             | SwitchParameterInfo |
| 28       | 141B           | 保留                    | Reservation                                 | 1       | 3            | 3             | 0             | SwitchParameterInfo |
| 29       | 141C           | 保留                    | Reservation                                 | 1       | 4            | 3             | 0             | SwitchParameterInfo |
| 30       | 141D           | 保留                    | Reservation                                 | 1       | 5            | 3             | 0             | SwitchParameterInfo |
| 31       | 141E           | 保留                    | Reservation                                 | 1       | 6            | 3             | 0             | SwitchParameterInfo |
| 32       | 141F           | 保留                    | Reservation                                 | 1       | 7            | 3             | 0             | SwitchParameterInfo |
| 33       | 1420           | 充电电流告警                | Charge current alarm                        | 1       | 0            | 4             | 1             | SwitchParameterInfo |
| 34       | 1421           | 充电过流保护                | Charge over current protection              | 1       | 1            | 4             | 1             | SwitchParameterInfo |
| 35       | 1422           | 充电过流二级保护              | Secondary charge over current protection    | 1       | 2            | 4             | 1             | SwitchParameterInfo |
| 36       | 1423           | 放电电流告警                | Discharge current alarm                     | 1       | 3            | 4             | 1             | SwitchParameterInfo |
| 37       | 1424           | 放电过流保护                | Discharge over current protection           | 1       | 4            | 4             | 1             | SwitchParameterInfo |
| 38       | 1425           | 放电二级过流保护              | Secondary discharge over current protection | 1       | 5            | 4             | 1             | SwitchParameterInfo |
| 39       | 1426           | 输出短路保护                | Output short-circuit protection             | 1       | 6            | 4             | 1             | SwitchParameterInfo |
| 40       | 1427           | 保留                    | Reservation                                 | 1       | 7            | 4             | 0             | SwitchParameterInfo |
| 41       | 1428           | 输出短路锁定                | Output short-circuit lock                   | 1       | 0            | 5             | 1             | SwitchParameterInfo |
| 42       | 1429           | 反接保护                  | Inverse current protection                  | 1       | 1            | 5             | 0             | SwitchParameterInfo |
| 43       | 142A           | 充电二级过流锁定              | Secondary charge over current lock          | 1       | 2            | 5             | 1             | SwitchParameterInfo |
| 44       | 142B           | 放电二级过流锁定              | Secondary discharge over current lock       | 1       | 3            | 5             | 1             | SwitchParameterInfo |
| 45       | 142C           | 保留                    | Reservation                                 | 1       | 4            | 5             | 0             | SwitchParameterInfo |
| 46       | 142D           | 保留                    | Reservation                                 | 1       | 5            | 5             | 0             | SwitchParameterInfo |
| 47       | 142E           | 保留                    | Reservation                                 | 1       | 6            | 5             | 0             | SwitchParameterInfo |
| 48       | 142F           | 保留                    | Reservation                                 | 1       | 7            | 5             | 0             | SwitchParameterInfo |
| 49       | 1430           | SOC低告警                | Low SOC alarm                               | 1       | 0            | 6             | 1             | SwitchParameterInfo |
| 50       | 1431           | 间歇式的充电                | Intermittent charge                         | 1       | 1            | 6             | 1             | SwitchParameterInfo |
| 51       | 1432           | 外部开关控制                | External switch control                     | 1       | 2            | 6             | 1             | SwitchParameterInfo |
| 52       | 1433           | 静态待机休眠                | Static stand-by sleep                       | 1       | 3            | 6             | 1             | SwitchParameterInfo |
| 53       | 1434           | 历史数据记录                | History data recording                      | 1       | 4            | 6             | 1             | SwitchParameterInfo |
| 54       | 1435           | SOC低保护                | Under SOC protect                           | 1       | 5            | 6             | 1             | SwitchParameterInfo |
| 55       | 1436           | 主动限流                  | Active-limited current                      | 1       | 6            | 6             | 1             | SwitchParameterInfo |
| 56       | 1437           | 被动限流                  | Passive-limited current                     | 1       | 7            | 6             | 1             | SwitchParameterInfo |
| 57       | 1438           | 均衡模块开启                | Equilibrium module to open                  | 1       | 0            | 7             | 1             | SwitchParameterInfo |
| 58       | 1439           | 静态均衡指示                | Static equilibrium indicate                 | 1       | 1            | 7             | 1             | SwitchParameterInfo |
| 59       | 143A           | 静态均衡超时                | Static equilibrium overtime                 | 1       | 2            | 7             | 1             | SwitchParameterInfo |
| 60       | 143B           | 超温禁止均衡                | Equalization temperature limit              | 1       | 3            | 7             | 1             | SwitchParameterInfo |
| 61       | 143C           | 保留                    | Reservation                                 | 1       | 4            | 7             | 0             | SwitchParameterInfo |
| 62       | 143D           | 保留                    | Reservation                                 | 1       | 5            | 7             | 0             | SwitchParameterInfo |
| 63       | 143E           | 保留                    | Reservation                                 | 1       | 6            | 7             | 0             | SwitchParameterInfo |
| 64       | 143F           | 保留                    | Reservation                                 | 1       | 7            | 7             | 0             | SwitchParameterInfo |
| 65       | 1440           | 蜂鸣器声指示                | Buzzer indicator                            | 1       | 0            | 8             | 0             | SwitchParameterInfo |
| 66       | 1441           | LCD显示功能               | LCD display                                 | 1       | 1            | 8             | 1             | SwitchParameterInfo |
| 67       | 1442           | 手动强制输出                | Manual forced output                        | 1       | 2            | 8             | 0             | SwitchParameterInfo |
| 68       | 1443           | 自动强制输出                | Auto forced output                          | 1       | 3            | 8             | 0             | SwitchParameterInfo |
| 69       | 1444           | 欠压恢复功能                | Under voltage recover                       | 1       | 4            | 8             | 0             | SwitchParameterInfo |
| 70       | 1445           | 气溶胶检测功能               | Aerosol detection function                  | 1       | 5            | 8             | 1             | SwitchParameterInfo |
| 71       | 1446           | 气溶胶常断模式               | Aerosol normally disconnected mode          | 1       | 6            | 8             | 1             | SwitchParameterInfo |
| 72       | 1447           | 检流器温度补偿               | Current detector temperature compensation   | 1       | 7            | 8             | 1             | SwitchParameterInfo |
| 73       | 1448           | NTC失效                 | NTC failure                                 | 1       | 0            | 9             | 1             | SwitchParameterInfo |
| 74       | 1449           | AFE失效                 | AFE failure                                 | 1       | 1            | 9             | 1             | SwitchParameterInfo |
| 75       | 144A           | 充电管失效                 | Charge mosfets failure                      | 1       | 2            | 9             | 1             | SwitchParameterInfo |
| 76       | 144B           | 放电管失效                 | Discharge mosfets failure                   | 1       | 3            | 9             | 1             | SwitchParameterInfo |
| 77       | 144C           | 电芯压差失效                | Cell diff failure                           | 1       | 4            | 9             | 1             | SwitchParameterInfo |
| 78       | 144D           | 断线                    | Cell break                                  | 1       | 5            | 9             | 1             | SwitchParameterInfo |
| 79       | 144E           | 按键失效                  | Key failure                                 | 1       | 6            | 9             | 1             | SwitchParameterInfo |
| 80       | 144F           | 保留                    | Reservation                                 | 1       | 7            | 9             | 0             | SwitchParameterInfo |
