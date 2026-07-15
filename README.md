# PIT WALL — F1 车迷仪表盘

三页静态站点，无需构建，直接部署到 GitHub Pages 即可。

## 页面

- `index.html` — 计时台：OpenF1 实时/历史计时塔（基础/专业/战斗三种模式 + 战斗组分组 + 新手术语解释）、车手圈速、轮胎策略、遥测
- `analysis.html` — 分析：按圈回放、事件时间线（Race Control/进站/无线电可播放）、全场轮胎策略图、多车手圈速对比
- `compare.html` — 对比：任意两位车手赛季对决（积分/交手/平均名次，可只算双方完赛场次）
- `profile.html` — 档案：车手/车队详情页（赛季 KPI、每站结果、历年战绩），从积分榜点击进入
- `index.html` 顶部会按赛事阶段（非比赛周/比赛周/进行中/赛后）显示动态横幅
- `schedule.html` — 赛程：下一场倒计时、周末各节时间（北京时间 + 本地时间）、全年赛历
- `standings.html` — 积分榜：车手 & 车队积分

## 数据源

- [OpenF1 API](https://openf1.org)（计时 / 遥测）
- [Jolpica-F1 API](https://jolpi.ca)（赛历 / 积分，Ergast 继任者）

均为免费公开 API，纯前端 fetch，无需后端和密钥。

## 部署到 GitHub Pages

1. 把本目录推到 GitHub 仓库
2. Settings → Pages → Source 选 `main` 分支根目录
3. 访问 `https://<用户名>.github.io/<仓库名>/`
