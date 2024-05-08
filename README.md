<div align="center">
  <h1>𝐕𝐌𝐀𝐈𝐋.𝐃𝐄𝐕</h1>
  <p><a href="https://discord.gg/d68kWCBDEs">Discord</a> · <a href="https://github.com/oiov/vmail/blob/main/README_en.md">English</a> | 简体中文</p>
  <p>使用 Cloudflare email worker 实现的临时电子邮件服务</p>
  <!-- <img src="https://img.inke.app/file/beb0212f96c6cd37eaeb8.jpg"/> -->
</div>

## 🌈 特点

- 🎯 隐私友好，无需注册，开箱即用
- ✈️ 支持邮件收发
- ✨ 支持保存密码，找回邮箱
- 😄 支持多域名后缀
- 🚀 快速部署，无需服务器

原理：

- Email worker 接收电子邮件
- 前端显示电子邮件（remix）
- 邮件存储（sqlite）
- 发信使用 MailChannel API

## 👋 自部署教程

### 准备工作

- [Cloudflare](https://dash.cloudflare.com/) 账户与托管在 Cloudflare 上的域名
- [turso](https://turso.tech) sqlite 数据库（个人免费计划足够）
- [Vercel](https://vercel.com) 或 [fly.io](https://fly.io) 账号部署前端用户界面
- 本地安装 [Nodejs](https://nodejs.org) 环境 (版本 >= 18.x)

### 接收邮件教程

查看 [receive-tutorial.md](/docs/receive-tutorial.md)

### 发送邮件教程

查看 [send-tutorial.md](/docs/send-tutorial.md)

## 🔨 本地运行调试

```bash
git clone https://github.com/oiov/vmail
cd vmail
# 安装依赖
pnpm install

# 运行端口 localhost:3000
pnpm run remix:dev
```

运行前复制 `apps/remix/.env.example` 文件并重命名为 `apps/remix/.env`，填写必要的环境变量。

## ❤️ 交流群

有任何问题或意见，欢迎加入交流群讨论。

- 添加微信 `yesmore_cc` (**备注你的职业**) 拉讨论群或[扫码进群](https://img.inke.app/file/494a7126352427a3b34d8.jpg) 
- Discord: https://discord.gg/d68kWCBDEs

## 🎨 Inspired By

Please check out these previous works that helped inspire the creation of vmail. 🙏

- [akazwz/smail](https://github.com/akazwz/smail)
- [email.ml](email.ml)

## 📝 License

GNU General Public License v3.0

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=oiov/vmail&type=Date)](https://star-history.com/#oiov/vmail&Date)
