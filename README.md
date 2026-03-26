# 🧧 美团红包助手（meituan-coupon）

> 一个 AI Agent Skill，帮你一键领取美团优惠券，并查询历史领券记录。支持主流 AI Agent 平台（Claude、OpenClaw 等）。

---

## ✨ 功能介绍

- **一键领券**：通过自然语言指令，自动为你的美团账号发放优惠券
- **历史查询**：查询指定日期或日期区间内的历史领券记录
- **内置认证**：无需额外安装其他 Skill，内置美团账号短信验证码登录流程
- **多平台支持**：兼容 macOS、Windows（Git Bash）、Linux 及其他 Agent 环境

---

## 🚀 快速开始

### 安装

将本仓库克隆到你的 Skill 目录：

```bash
# macOS / Linux
git clone https://github.com/<your-org>/meituan-coupon \
  ~/.claude/skills/meituan-coupon-get-tool

# 或使用自定义 Skill 目录
git clone https://github.com/<your-org>/meituan-coupon \
  $CLAUDE_CONFIG_DIR/skills/meituan-coupon-get-tool
```

### 触发词

在对话框中输入以下任意关键词即可激活本 Skill：

> 领取美团权益、领美团券、我要领券、领优惠券、美团发券、美团优惠、美团红包、外卖红包、外卖优惠、美团外卖券、美团外卖神券

---

## 📖 使用示例

**领取今日优惠券：**
```
用户：领美团券
助手：🎉 美团权益领取成功！共为您发放 3 张优惠券：
      🎫 外卖满减券
      💰 面额：15 元（满 50 元可用）
      📅 有效期：2026-03-25 至 2026-04-01
      🔗 立即使用
      ...
```
---


## 🛡️ 安全说明

- 所有核心参数（渠道码、接口域名等）均由 Skill 内部维护，外部不可覆盖
- 每天每个账号仅可领取一次，服务端有防重保护
- Token 仅存储在本地，不会上传至任何服务器
