# Life skills

给 AI 助手使用的中文生活办事 Skill，包含香港手机号办理与美国汇丰申请辅助。

## 香港手机号办理与保号

[查看 Skill](skills/hk-mobile-number-guide/SKILL.md)

适用于首次办理带 +852 号码的 SIM / eSIM，以及后续充值、续费和保号。助手会根据所在地、设备和用途核对官方条件，区分号码到期、流量包到期和自动续购，并在具备任务工具时按真实到期日设置提醒。

不保证所有设备支持 eSIM，也不保证所有平台接受号码或验证码必达。实际浏览、开户和设置提醒能力取决于客户端提供的工具及用户授权。本项目与运营商无隶属关系。

## 美国汇丰申请辅助

[查看 Skill](skills/hsbc-us-application/SKILL.md) · [资料预检模板](skills/hsbc-us-application/references/intake.md) · [状态与计时规则](skills/hsbc-us-application/references/status-and-timing.md)

适用于境外申请人的材料准备、官网填写辅助、超时恢复、身份核验异常处理、回执核对和补件跟进。先核对实时官方要求，再使用本人确认的资料；电子月结单与正式水电账单的完整性、地址一致性是准备重点。

来自一次已提交、待审核的实操，不代表已获批，不保证申请资格、审批速度或费用豁免。护照拍摄、活体核验、法律声明和最终开户提交由申请人本人完成。本项目与汇丰无隶属关系。

## 安装

使用已安装 Node.js / npm 的终端运行：

```bash
npx skills add itsoso/life-skills --skill hk-mobile-number-guide
npx skills add itsoso/life-skills --skill hsbc-us-application
```

按提示选择客户端和安装范围。[skills CLI](https://github.com/vercel-labs/skills) 支持 Codex、Claude Code、Cursor 等客户端。

只查看可安装的 Skill：

```bash
npx skills add itsoso/life-skills --list
```

更新已安装的 Skill：

```bash
npx skills update
```

香港手机号 Skill 也可以从 [Releases](https://github.com/itsoso/life-skills/releases) 下载 ZIP，解压后按客户端的 Skill 安装说明放置整个 `hk-mobile-number-guide` 文件夹。支持 Skill 文件夹的客户端可读取其中的 `SKILL.md` 和相对引用。

## 使用示例

安装后在支持 Skill 的助手中发送：

> 使用 hk-mobile-number-guide 帮我办理香港手机号。我主要用来收短信，请先检查我的设备支持情况、能否在当前位置激活，以及保号费用。没有核实的信息请标明。

已有号码时可以说：

> 使用 hk-mobile-number-guide 帮我核对号码到期日、流量包到期日和自动续购设置，并提前 30 天和 7 天提醒我保号。请先确认实际到期日。

申请美国汇丰时可以说：

> 使用 hsbc-us-application 帮我准备美国汇丰申请。先核对当前官方条件和材料缺项，再协助填写；只使用我确认的信息。身份验证、声明和最终提交由我完成。已有提交回执时只跟进补件，不重复申请。

## 普通读者如何使用

无需安装也可以阅读 [办理步骤](skills/hk-mobile-number-guide/SKILL.md) 和 [SoSIM 官方核验入口](skills/hk-mobile-number-guide/references/sosim.md)。先确认设备和所在地条件，再核对官方套餐、实名、短信及续费规则。

## 隐私与反馈

发布内容仅包含通用流程和官方公开链接，不附个人订单、邮件、手机号、证件或激活二维码。Skill 不包含自动采集数据的脚本；用户在客户端输入的数据由所用客户端处理。

汇丰 Skill 仅包含通用步骤及空白模板，不附真实账单、身份证号、护照号、住址、账户或申请编号。填写后的预检表应保留在用户授权的私有目录，不能提交到此公开仓库。

通过 Issue 反馈失效链接或流程变化即可。请勿上传个人号码、证件、邮箱、验证码、订单、ICCID、EID、安装二维码或带令牌的链接。

## 维护与许可证

首次发布：v0.1.0，2026-10-09。美国汇丰申请辅助 Skill 加入于 2026-10-16。运营商和银行规则可能变化，执行时须重新核对官方页面。

采用 [MIT License](LICENSE)。
