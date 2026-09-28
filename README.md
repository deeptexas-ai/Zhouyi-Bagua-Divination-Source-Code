# 周易排盘与八字源码 | JavaScript Bazi & Chinese Metaphysics

[简体中文](README.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md) | [产品网站](https://deeptexas-ai.github.io/Zhouyi-Bagua-Divination-Source-Code/)

这是一个以浏览器 JavaScript 为主体的传统术数排盘源码仓库。公开代码覆盖四柱八字、干支与农历换算、十神与神煞、刑冲合害、五行、大运流年、时区与真太阳时相关计算，并包含七政四余、大六壬及紫微运势接口调用等产品组件。

> 范围说明：本页只描述公开代码与真实截图可以核实的内容。仓库没有 `package.json`、Docker 配置、Python 服务、SQLite 数据库或完整的 64 卦数据，因此不应宣传为已经验证的一键部署或完整三币六爻系统。部分界面调用 `/api`，实际部署前需要补齐对应服务。

## 产品界面

| 四柱八字与大运 | 七政四余排盘 |
| --- | --- |
| ![四柱八字、大运流年与真太阳时界面](docs/assets/screenshots/wujibazi.png) | ![七政四余星曜、时区与经纬度输入界面](docs/assets/screenshots/qizhengsiyu.png) |
| 大六壬盘式 | 五行趋势与排盘记录 |
| ![大六壬天地盘、四课三传排盘结果](docs/assets/screenshots/daliuren.png) | ![五行趋势图和排盘历史记录](docs/assets/screenshots/wuxing.png) |

## 主要功能

### 四柱八字与历法

- 根据公历时间生成干支、四柱与十神相关数据。
- 公历与农历转换，包含节气、生肖、儒略日等历法组件。
- 大运、流年、流月、流日、流时和换运时间展示。
- 支持时区、经纬度及真太阳时相关输入。

### 五行、十神与神煞

- 天干地支与木、火、土、金、水的映射和生克关系。
- 十神、藏干以及干支刑、冲、合、害关系。
- `shensha.js` 中的神煞规则、说明和按干支查询逻辑。
- 五行趋势参数、图表及历史排盘界面。

### 七政四余、大六壬与扩展组件

- 七政四余星曜选择、经纬度、时区与排盘结果界面。
- `kinliuren.js` 提供大六壬盘式计算组件。
- `index.js` 包含紫微运势图和反推功能的接口调用与图表渲染代码。
- 搜盘、拆补、宫位、九星、八门等筛选项可从截图界面核实。

## 代码结构

| 文件 | 可核实职责 |
| --- | --- |
| `index.html` / `index.js` | 排盘页面、输入流程、图表和 API 交互 |
| `lunar.js` / `nongli.js` | 公历、农历、干支与节气计算 |
| `paipan.js` | 天文历法、节气、真太阳时和排运基础 |
| `paipan.gx.js` | 十神、藏干、刑冲合害关系 |
| `shensha.js` | 神煞规则、说明与查询 |
| `kinliuren.js` | 大六壬相关计算 |
| `timezone.js` | 时区、经纬度与偏移数据 |

## 更多真实截图

| 搜盘条件 | 流年星盘 |
| --- | --- |
| ![八字搜盘条件与格局筛选](docs/assets/screenshots/baizhipaipan.png) | ![流年星体黄经与星盘数据](docs/assets/screenshots/liunian.png) |
| 七政四余综合盘 | 星曜组合结果 |
| ![七政四余综合排盘数据表](docs/assets/screenshots/paipan.png) | ![七政四余多组星曜结果](docs/assets/screenshots/qizheng2.png) |

## 使用与部署边界

公开页面可以直接阅读源文件，但完整运行环境可能依赖仓库外的样式、图表库和 `/api` 服务。上线前应核对依赖授权、接口实现、数据隐私和计算结果，并补充测试。命理与占卜内容只适合传统文化研究和娱乐参考，不应替代医疗、法律、投资或其他专业建议。

## 联系方式

- Telegram：[@xuzongbin001](https://t.me/xuzongbin001)
- Email：[masterai918@gmail.com](mailto:masterai918@gmail.com)

## License

以仓库中的 [License.md](License.md) 为准。第三方历法和算法代码可能保留各自署名及授权要求，商用前请逐项核实。
