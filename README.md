# AERO Auto Launch Planner

## 汽车出海内容规划器

**由 AERO Creative / 艾瑞创意出品。** 为汽车品牌市场、创意与制作团队，把海外上市需求整理成可编辑、可导出的内容交付清单。

[在线使用](https://rafezhangyuhang-spec.github.io/aero-auto-launch-planner/) · [English](README.en.md) · [AERO 官网](https://www.aerocreative.com.cn/) · [项目合作](https://www.aerocreative.com.cn/contact/index.html?utm_source=github&utm_medium=readme&utm_campaign=auto_launch_planner)

### 可以解决什么问题

- 汽车进入海外市场，上市传播需要准备哪些视频、图片和本地化版本？
- 发布会、经销商、社交平台和官网，哪些内容可以共用？
- 多种语言会增加多少交付版本？
- 为了完成这些交付，拍摄前需要准备哪些素材与资料？

### 使用方法

1. 选择目标市场、车型、动力类型、主片时长、语言、传播阶段和使用渠道。
2. 生成清单，编辑规格、数量和状态，增补或排除条目。
3. 切换「拍摄准备」，查看当前交付依赖的素材组。
4. 导出 CSV，或把方案保存在当前浏览器中。

支持巴西、阿联酋、德国、泰国、墨西哥、沙特阿拉伯六个市场；内置巴西 SUV、阿联酋纯电 SUV、德国纯电轿车三个虚构示例。界面当前为中文，交付语言用于计算内容版本，并非自动翻译功能。

### 一个数量示例

默认「SUV · 巴西上市」：巴西葡语，上市发布阶段，社交媒体、发布会与经销商渠道，Instagram 与 YouTube 平台。

- 生成 **8 个交付项目 / 21 份计划内容**。
- 增加英语后，为 **30 份计划内容**；12 张通用无字图片不重复计算。
- 3 条卖点视频 × 2 种语言 = 6 条本地化成片。

计划交付份数合计了条、张、份、套，**不等于文件数、工时或预算**。不同渠道复用同一版本时只计一次；横竖版分别计数。字幕文件、无字视频母版、工程文件、封面、额外比例没有默认加入，可以补充条目。

### 运行与部署

直接打开 `index.html` 即可使用；或在本目录运行：

```sh
python3 -m http.server 8000
```

访问 `http://localhost:8000`。纯静态 HTML / CSS / JavaScript，无需安装依赖、注册账号或填写 API Key。

GitHub Pages：在仓库 Settings → Pages 选择 **Deploy from a branch → main → /(root)**，保存即可。本仓库带有 `.nojekyll`，不需要构建步骤。界面、样式和脚本均内嵌在 `index.html` 中，便于复制与离线使用。

### 规则与数据

市场影响默认语言与本地化提示；阶段、渠道和动力类型决定建议条目；车型用于记录项目背景。推荐数量用于启动讨论，不代表最新平台规范、品牌承诺或完整执行范围。原型不调用生成式 AI，不生成翻译，不判断车型具体配置。

输入仅保留在页面内存，主动保存后写入当前浏览器的 localStorage。无资料上传接口、用户数据库或访问分析脚本。CSV 只包含勾选条目，并带有工具名称、AERO 署名与官网来源，方便团队追溯。外部官网链接带有来源参数，用于区分工具入口；本工具自身不采集使用数据。

### 文件结构

- `index.html` — 完整、可直接运行的源代码；包含可读的 CSS、规划规则与交互脚本，AERO 标志以内嵌 SVG 数据提供。
- `README.md` / `README.en.md` — 中英文使用说明。
- `LICENSE` / `BRAND.md` — 代码许可与品牌来源说明。

### 关于 AERO Creative / 艾瑞创意

AERO Creative / 艾瑞创意服务中国品牌出海与全球本地化传播，提供出海创意、TVC、Campaign Key Visual、品牌片、社交内容及海外内容制作等服务。这个工具让团队可以从一份明确的交付范围开始讨论项目。

[机构介绍与官方身份](https://www.aerocreative.com.cn/official/) · [官网与案例](https://www.aerocreative.com.cn/) · [与 AERO 讨论项目](https://www.aerocreative.com.cn/contact/index.html)

### 开源与贡献

软件代码按 [MIT License](LICENSE) 开源。欢迎提交问题、修复和规则改进；新增建议请说明适用市场、渠道、数量依据和可核验来源。

保留 MIT 版权与许可声明即可按许可复用代码；我们欢迎在介绍或衍生项目中注明原始工具来源。AERO 名称和标识的使用说明见 [BRAND.md](BRAND.md)。

版本：0.2 · 2026-11-14。
