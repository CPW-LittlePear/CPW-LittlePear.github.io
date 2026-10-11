# MEMORY.md

## 用户信息
- 姓名：曹培文，昵称小梨
- 学校：南京大学
- 邮箱：xiaoningmeng1934@qq.com
- 微信号：xiaoningmeng1934
- 个人主页：https://cpw-littlepear.github.io/
- 仓库本地路径：e:\Mine\Homepage\CPW-LittlePear.github.io

## 个人主页结构（截至 2026-04-11）
- 框架：纯 HTML + Marked.js 渲染 Markdown，部署在 GitHub Pages
- 布局：左侧固定侧边栏（260px）+ 右侧主内容
- 侧边栏：头像（photo.png）+ 小梨/曹培文-南京大学 + 导航 + 联系方式
- 联系方式：邮箱文字 + wechat: 文字 + 微信二维码图片（static/assets/img/wechat-qrcode.jpg）

## 当前导航顺序
教育背景(home.md) → 实习经历(Work.md) → 项目经历(Project.md) → GameJam(GameJam.md) → 作品集(artwork.md) → 游戏经历(Game.md) → 相关技能(Skill.md) → 校园经历(campus.md)

## 项目约定
- Markdown 图片路径统一用相对路径，如 contents/images/xxx.png
- 图片在 main.css 中统一设为 width:50%
- 加粗用 <strong> 标签（marked.js 对某些中文符号组合解析不稳定）
- **index.html 严禁引入外部 CDN**：polyfill.io / jsdelivr / Google Fonts / MathJax 在国内均被墙，会导致页面白屏/打不开。相关资源已全部本地化：bootstrap-icons.css 在 static/css/、字体在 static/fonts/（woff2/woff）。新增图标资源时务必本地化，不要加新 CDN 链接。
- git push 需要代理：git config --global http.proxy http://127.0.0.1:7890
- **直连 GitHub 注意**：大文件传输（完整 clone 50MB pack / push 大 diff）常遇 `Connection was reset`（GFW 干扰）。可靠做法：① 用浅克隆 `git clone --depth 1` 规避大包；② 或开代理 127.0.0.1:7890；③ push 增量（小 commit）通常能成功，不必重传全量
- Windows 下被 IDE/资源管理器占用的目录无法 `mv`/`rm` 整目录（busy），但可写入 → 可用 `cp -a` 覆盖内部文件来"替换"仓库内容

## GameJam 记录（6条）
- 第二届 034 GameJam 程序 2026.3
- 2026Global GameJam 美术 2026.1
- 第九届 雷火makers 策划 2025.10
- 2025Taptap聚光灯GameJam 杭州站 策划 2025.8
- 2025Ciga GameJam 策划 2025.6
- 2025Taptap聚光灯GameJam 上海站 策划 2025.6
