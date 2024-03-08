# PIA Table
Basic status info


| **"ID"** | **rtuAddress** | **description zh-CN** | **description en-US**      | **byte** | **byteIndex** | **unit** | **scale** | **hasSign** | **isDisplay** | **datatype** | **inHistory** |
|----------|----------------|-----------------------|----------------------------|----------|---------------|----------|-----------|-------------|---------------|--------------|---------------|
| 1        | 1000           | 总电压                   | Battery voltage            | 2        | 0             | V        | 0.01      | 0           | 1             | MainInfo     | 1             |
| 2        | 1001           | 总电流                   | Current                    | 2        | 2             | A        | 0.01      | 1           | 1             | MainInfo     | 1             |
| 3        | 1002           | 剩余容量                  | Remaining capacity         | 2        | 4             | Ah       | 0.01      | 0           | 1             | OtherInfo    | 1             |
| 4        | 1003           | 总容量                   | Total capacity             | 2        | 6             | Ah       | 0.01      | 0           | 1             | OtherInfo    | 0             |
| 5        | 1004           | 总放电容量                 | Total discharge capacity   | 2        | 8             | Ah       | 10        | 0           | 1             | OtherInfo    | 0             |
| 6        | 1005           | SOC                   | SOC                        | 2        | 10            | %        | 0.1       | 0           | 1             | MainInfo     | 0             |
| 7        | 1006           | SOH                   | SOH                        | 2        | 12            | %        | 0.1       | 0           | 1             | OtherInfo    | 0             |
| 8        | 1007           | 循环次数                  | Cycle                      | 2        | 14            | times    | 1         | 0           | 1             | OtherInfo    | 0             |
| 9        | 1008           | 平均电芯电压                | Averag of cell votage      | 2        | 16            | V        | 0.001     | 0           | 1             | MainInfo     | 0             |
| 10       | 1009           | 平均电芯温度                | Averag of cell temperature | 2        | 18            | ℃        | 0.1       | 0           | 1             | OtherInfo    | 0             |
| 11       | 100A           | 最高电芯电压                | Max cell voltage           | 2        | 20            | V        | 0.001     | 0           | 1             | MainInfo     | 0             |
| 12       | 100B           | 最低电芯电压                | Min cell voltage           | 2        | 22            | V        | 0.001     | 0           | 1             | MainInfo     | 0             |
| 13       | 100C           | 最高电芯温度                | Max cell temperature       | 2        | 24            | ℃        | 0.1       | 0           | 1             | OtherInfo    | 0             |
| 14       | 100D           | 最低电芯温度                | Min cell temperature       | 2        | 26            | ℃        | 0.1       | 0           | 1             | OtherInfo    | 0             |
| 15       | 100E           | 系统事件概要                | System events              | 2        | 28            |          | 1         | 0           | 0             | OtherInfo    | 0             |
| 16       | 100F           | 建议最大放电电流              | Max discharge current      | 2        | 30            | A        | 1         | 0           | 1             | OtherInfo    | 0             |
| 17       | 1010           | 建议最大充电电流              | Max charge current         | 2        | 32            | A        | 1         | 0           | 1             | OtherInfo    | 0             |
| 18       | 1011           | 母线电压                  | Extern voltage             | 2        | 34            | V        | 0.001     | 0           | 0             | OtherInfo    | 0             |
