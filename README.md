GitHub 已开源部分
- SOSOVE X 日文发帖 Skill：每天生成 5 条日文 X 文案，支持按星期/季节/日本生活场景选角度；可生成配图 prompt；可接收 5 张图片并按顺序匹配文案；支持使用已登录的 X 浏览器批量发帖。核心在 [SKILL.md](D:/Backup/Documents/New project/skills/sosove-x-posts/SKILL.md)。
- Meta 广告资料库下载器：Chrome MV3 扩展，自动加载广告、捕获最高源视频、按 CDN 去重、保留广告编号和广告文案、检测分辨率、筛选画质、批量下载、暂停/继续/取消、失败重试、导出 CSV、按“唯一视频”或“按资料库编号”命名。见 [README.md](D:/Backup/Documents/New project/meta-ad-library-hd-downloader/README.md)。
- Cloudflare 批量域名工具：cf_add_zones.py 批量把域名添加为 Cloudflare Zone；cf_dns_upsert.py 批量新增或更新根域名 A 记录和 www CNAME 记录，走环境变量读取 Token。
- X 发帖示例数据：data/x-platform/2026-05-27/ 里有 5 张图、压缩版 JPG 和对应日文文案。
- Facebook 广告报表样例：仓库里还提交了 reports/facebook_bm_ads* 的历史 CSV/JSON 报表样例。
本地工作区还有、但这次没有全部开源的能力
- SOSOVE SKU Board：商品、卖点、设计进度、广告花费、任务、复盘、AI 生图、日本落地页 10 图、Amazon A+ 9 图、乐天 9 图、COD 30 图等一体化运营面板。见 [README.md](D:/Backup/Documents/New project/sosove-sku-board/README.md)。
- Shopline Monitor：独立站订单/GA4/渠道归因监控、UTM 诊断、异常提醒、飞书/Slack webhook、利润估算和运营摘要。
- TikTok Ads Monitor：多广告账户同步、CTR/CPC/CVR 重算、异常识别、预算建议、素材动作表、视频内容诊断、AI 调户助手、操作审计。见 [README.md](D:/Backup/Documents/New project/tiktok_ads_monitor/README.md)。
- Seedance Video Web：本地 Web 工作台，支持 Ark/Seedance 视频任务提交、状态轮询、模型配置、图片/视频/音频上传、ffprobe 元数据、AI prompt 生成、1–4 条批量任务。
- Creator Outreach：Instagram/TikTok 达人筛选、CSV 导入导出、公开搜索连接器、官方 Graph API 补资料、日文 DM 草稿、回复助手、合作/寄样/发布/优惠码/ROI 跟踪。
- Universal Video Downloader / Image Crawler：Chrome 扩展，前者识别网页视频直链和 Instagram 视频；后者递归采集当前站点图片并导出 CSV。
- AI Product Agent：目前主要是脚手架，规划 1688 选品 → 日本市场评估 → Shopline 上架 → 广告反馈；真实爬虫、AI 评分、Shopline 同步还没完成。见 [README.md](D:/Backup/Documents/New project/ai-product-agent/README.md)。
- Open Image Prompts：图片提示词库 + img-gen-taste / img-gen-prompts 两个 Skill，支持本地检索和画廊。
- ChatCut / HyperFrames 广告视频工作流：AI 素材分析、混剪候选、剪映草稿、ChatCut 同步、视频文案库和商品提示词。
