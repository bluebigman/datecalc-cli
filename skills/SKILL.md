# 日期计算器（datecalc-cli）

日期加减/间隔与工作日估算/年龄工龄/往后第 N 个工作日。纯本地计算。

本工具仅做本地数据/文本处理，不采集任何个人信息。

## 命令
| 命令 | 用途 |
|---|---|
| `datecalc status` | 自检（返回含 ok） |
| `datecalc auth` | 校验可用（本地工具无需密钥） |
| `datecalc unAuth` | 清除本地状态 |
| `datecalc add <YYYY-MM-DD> <天数>` | 日期加减 |
| `datecalc between <起> <止>` | 间隔天数+工作日估算 |
| `datecalc age <YYYY-MM-DD>` | 年龄/工龄（精确到月日） |
| `datecalc nworkday <YYYY-MM-DD> [N]` | 往后第 N 个工作日 |

所有命令输出 JSON：`{"code":0|1,"ok":true|false,"data":...,"error":"人类可读错误"}`。

## AI 使用指引
日期计算：加减 add、算间隔 between、算年龄 age；工作日为估算，精确节假日提示用 cn-holiday。
