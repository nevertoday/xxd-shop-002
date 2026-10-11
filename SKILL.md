---
name: xxd-shop-002
description: "Create XXD Shop 002 signature-dish main images (餐饮招牌产品主图) as finished PNGs from a dish photo, packaged-food shot, menu photo directory, or just a dish name, treating the bundled original brief as the sole aesthetic authority: the dish name becomes a bold signboard-grade title readable at thumbnail size, the food is the absolute centre with steam, gloss, sauce and layering, and a restrained recommendation-sticker system (招牌、必点、手作…) supports the buying decision. For restaurants, takeaway platforms, menus, light boxes and packaged food. Supports multiple ratios or exact sizes, several compositions per size, prompt-generated, user-exact or user-plan copy, and supplied facts only. Use when the user invokes xxd-shop-002 or asks for 招牌菜主图、外卖主图、餐饮爆品图、菜品海报、门店灯箱图."
---

# XXD Shop 002｜招牌菜主图

用本次的菜品图、产品包装图或菜名，生成“先记住名字，再产生食欲，再下单”的餐饮招牌主图，交付 PNG。

每次生成前，完整读取 `references/original-prompt/zh-CN.md`。这份中文原始提示词是唯一的创作与审美权威；不总结、不翻译、不混用，也不用本文件、README、样张或其他编号替代它。

每次构建生图请求前，完整读取 `references/shop-runtime.md`，它是唯一的家族运行合同。本 Skill 不另写第二套美术指导或运行规则。

所有成品直接写进 `~/Desktop/xxd/xxd-shop-002/` 下新建的一个任务目录（或 `--out` 指定的根目录），不建子目录，不自动拼总览。

## 本编号覆盖条款

**菜名是必需输入。** 原稿要求“产品名称必须成为第一视觉识别点”。菜名来自 `--product`、用户描述，或菜品图上清楚可读的招牌、包装；都没有就问，不替店家起菜名。

**“不要文字”与原稿冲突。** 选择 `--text none` 时，先说明这会去掉原稿的核心（菜名大字和推荐贴纸），用户仍坚持才执行。

**推荐贴纸按家族事实纪律的三级处理**，下表是本编号的餐饮版本，只比家族规则更严：

| 类型 | 例子 | 处理 |
|---|---|---|
| 店家自己的推荐语气 | 招牌、主推、必点、店长推荐、经典、手作、口味签（麻辣、鲜香、酸甜）、由菜名本身带出的地域风味（川味、潮汕） | 图像模型按原稿自行生成 |
| 需要店家确认的状态 | 新品、限定、季节限定、今日特供 | 只有用户说过才用 |
| 关于别人行为或可核查的事实 | 热销、人气、口碑、销量、排名、获奖、老字号年份、“XX 必吃榜” | 只来自“可用事实”，否则不出现 |

不确定某个词属于哪一级时，按更严格的一级处理。

**食物要像这道菜本身。** 有菜品图时，摆盘、器皿、主料与配料的种类和比例以图为准，不额外加肉、加料、加份量；热气、油润、酱汁光泽可以按原稿强化。没有菜品图时，主料配料只从菜名、用户描述和品类常识推出，不加用户没提到的招牌食材。

**适用范围：** 堂食菜品、饮品、小吃、预制菜和速食包装，也包括单个烘焙品的招牌图。要做一套烘焙系列，或想重点放大酥皮、气孔这类烘焙质感时，推荐 `xxd-shop-004`。

**追加验收：** 菜名在缩略图尺寸下第一眼可读；菜名先于食物被注意到，再把视线引向食物；贴纸数量克制、主次分明，没有满屏促销；没有出现上表第三级里无来源的词。

## 参考文件

- `references/shop-runtime.md`：家族运行合同
- `references/original-prompt/zh-CN.md`：运行时使用的原始提示词
- `references/original-prompt/README.md`：译文索引与权威说明
- `references/runtime-preferences.md`：交付偏好沿用
- `references/sample-workflow.md`：仅用于维护样张
- `scripts/configured_imagegen.py`、`scripts/shop_preferences.py`
