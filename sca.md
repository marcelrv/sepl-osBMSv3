# SCA table

FET and onther status & setting

| **"ID"** | **rtuAddress** | **description zh-CN** | **description en-US**  | **byte** | **value** | **Index** | **unit** | **scale** | **hasSign** | **isDisplay** | **datatype** | **attribute** |
|----------|----------------|-----------------------|------------------------|----------|-----------|-----------|----------|-----------|-------------|---------------|--------------|---------------|
| 1        | 150D           | 零点校准                  | Calibration Zero       | 2        | 0         | 0         | A        | 0.01      | 1           | 1             | AdjustInfo   | Other         |
| 2        | 150E           | 电流校准                  | Calibration Current    | 2        | -50       | 1         | A        | 0.01      | 1           | 1             | AdjustInfo   | Normal        |
| 3        | 150F           | 电芯电压校准                | Calibration Voltage    | 2        | 3.3       | 2         | V        | 0.001     | 0           | 1             | AdjustInfo   | Normal        |
| 4        | 1510           | 放电管关闭                 | Discharing FETs Off    | 2        | 0         | 0         | -        | 1         | 0           | 1             | ControlInfo  | OnOff         |
| 5        | 1510           | 放电管取消关闭               | Discharing FETs On     | 2        | 0         | 0         | -        | 1         | 0           | 1             | ControlInfo  | OffOn         |
| 6        | 1511           | 充电管关闭                 | Charing FETs Off       | 2        | 0         | 1         | -        | 1         | 0           | 1             | ControlInfo  | OnOff         |
| 7        | 1512           | 限流管关闭                 | Current Limit FETs Off | 2        | 0         | 2         | -        | 1         | 0           | 1             | ControlInfo  | OnOff         |
| 8        | 1513           | 预充管开启                 | Precharging FETs On    | 2        | 0         | 3         | -        | 1         | 0           | 0             | ControlInfo  | OffOn         |
| 9        | 1514           | 加热管开启                 | Heater FETs On         | 2        | 0         | 4         | -        | 1         | 0           | 1             | ControlInfo  | OffOn         |
| 10       | 1515           | 充电管开启                 | Charing FETs On        | 2        | 0         | 5         | -        | 1         | 0           | 1             | ControlInfo  | OffOn         |
| 11       | 1516           | 恢复出厂                  | Parameter Reset        | 2        | 0         | 6         | -        | 1         | 0           | 1             | ControlInfo  | Simple        |
| 12       | 1517           | 系统关机                  | System Power Off       | 2        | 0         | 7         | -        | 1         | 0           | 1             | ControlInfo  | Simple        |
| 13       | 1518           | 系统复位                  | System Reset           | 2        | 0         | 8         | -        | 1         | 0           | 1             | ControlInfo  | Simple        |
