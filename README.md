🎬 MovieBox Pro - 影视求片与媒体管理系统
![alt text](https://img.shields.io/docker/pulls/tbslantian/moviebox)

![alt text](https://img.shields.io/docker/v/tbslantian/moviebox/latest)

[
![alt text](https://img.shields.io/badge/Timezone-Asia%2FShanghai-red?style=flat&logo=clock)
](https:// time.is/Shanghai)
![alt text](https://img.shields.io/badge/Powered_By-Flask_&_Cython-blue)
MovieBox Pro 是一个现代化、轻量级且功能强大的影视求片管理系统。它无缝连接 TMDB、Emby 和 MoviePilot，为用户提供优雅的影片发现、状态查询及自动化订阅体验。
![alt text](https://via.placeholder.com/1200x600.png?text=MovieBox+Pro+Dashboard)

![alt text](image.png)  ![alt text](image-1.png) ![alt text](image-2.png) ![alt text](image-3.png)
✨ 核心特性
🎥 沉浸式发现：基于 TMDB 的热门趋势展示，每日自动更新，配合 Hero 大图背景，视觉体验极佳。
🔍 Emby 状态透视：在浏览或搜索影片时，自动检测 Emby 媒体库。如果库中已存在，直接显示 "Emby 已有" 绿色标签，拒绝重复求片。
🚀 无缝对接 MoviePilot：通过账号密码自动登录 MoviePilot 获取 Token，一键推送到 MoviePilot 进行下载。
⚡ 极致性能优化：
图片反代与缓存：内置 Emby 图片反向代理，自动缓存海报 3 小时，解决内网图片无法加载及浏览器请求频繁的问题。
后台异步更新：热门趋势与库存检测采用 "Stale-While-Revalidate" 策略，页面加载毫秒级响应。
📱 全端适配：完美适配移动端，支持侧边栏手势交互，手机管理更轻松。
📊 个人观影报告：基于 Emby 用户数据，生成个人观影统计与最近播放记录。

推荐使用 Docker Compose 进行部署


⚙️ 环境变量详解
变量名	必填	说明
MB_LICENSE_KEY	✅	商业授权码，用于激活系统
CFG_API_KEY	✅	TMDB API Key
CFG_MP_URL	✅	MoviePilot 地址 (http://IP:端口)
CFG_MP_USER	✅	MoviePilot 登录用户名
CFG_MP_PWD	✅	MoviePilot 登录密码
CFG_EMBY_URL	✅	Emby 地址 (http://IP:端口)
CFG_EMBY_KEY	✅	Emby API Key



📜 免责声明
本项目仅供个人学习与家庭媒体库管理使用。
所有元数据来自 TMDB，本项目不提供任何视听内容下载。
请勿将本项目用于商业盈利或非法用途。

