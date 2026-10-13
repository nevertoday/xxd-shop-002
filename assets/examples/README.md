# XXD Shop 002 样张

每张都是本编号按 `references/sample-workflow.md` 一次生成、目视通过的原图，像素未改，只清理了元数据。商品是虚构的演示品牌，画面上的价格、规格等数字都是演示设定。

| 文件 | 用途 | 实际像素 | 输入 | 文字方式 | visual_review |
|---|---|---|---|---|---|
| `c01-category-1x1-1254x1254.png` | 外卖主图 | 1254x1254 | Logo `logo-laowan.png` | prompt zh-CN | passed |
| `c02-category-3x4-1086x1448.png` | 菜单主推 | 1086x1448 | Logo `logo-shanyu.png` | prompt zh-CN | passed |
| `c03-category-1x1-1254x1254.png` | 外卖主图 | 1254x1254 | Logo `logo-laowan.png` | prompt zh-CN | passed |
| `c04-category-4x5-1122x1402.png` | 电商主图 | 1122x1402 | Logo `logo-laowan.png` | prompt zh-CN | passed |
| `c05-category-16x9-1672x941.png` | 门头灯箱 | 1672x941 | Logo `logo-xiandao.png` | prompt zh-CN | passed |
| `c06-category-9x16-941x1672.png` | 门店竖屏 | 941x1672 | Logo `logo-shanyu.png` | plan zh-CN | passed |
| `s01-size-1x1-1254x1254.png` | 外卖主图 | 1254x1254 | 原图 `beef-noodle.jpg`、Logo `logo-laowan.png` | prompt zh-CN | passed |
| `s02-size-3x4-1086x1448.png` | 菜单主推 | 1086x1448 | 原图 `beef-noodle.jpg`、Logo `logo-laowan.png` | prompt zh-CN | passed |
| `s03-size-9x16-941x1672.png` | 门店竖屏 | 941x1672 | 原图 `beef-noodle.jpg`、Logo `logo-laowan.png` | prompt zh-CN | passed |
| `s04-size-16x9-1672x941.png` | 门头灯箱 | 1672x941 | 原图 `beef-noodle.jpg`、Logo `logo-laowan.png` | prompt zh-CN | passed |
| `s05-category-3x4-1086x1448.png` | 菜单主推 | 1086x1448 | 商品图 `product-shanyu-coldbrew.jpg`、Logo `logo-shanyu.png` | prompt zh-CN | passed |
| `s06-category-1x1-1254x1254.png` | 外卖主图 | 1254x1254 | 仅商品名称 | prompt zh-CN | passed |
| `s07-category-4x5-1122x1402.png` | 电商主图 | 1122x1402 | 仅商品名称 | prompt zh-CN | passed |
| `s08-special-1x1-1254x1254.png` | 外卖主图 | 1254x1254 | 原图 `beef-noodle.jpg`、Logo `logo-laowan.png` | prompt en-US | passed |
| `s09-special-1x1-1254x1254.png` | 外卖主图 | 1254x1254 | 原图 `beef-noodle.jpg`、Logo `logo-laowan.png` | prompt ja-JP | passed |

## 输入素材

`sources/` 里是生成时交给本编号的输入缩样，模拟商家手里的素材：带包装与 Logo 的商品图、品牌 Logo，个别为原图。
演示品牌、Logo 和商品图由本项目生成；其中以 Unsplash 照片为底的，署名如下，适用 [Unsplash License](https://unsplash.com/license)，**不属于**本仓库的 PolyForm Noncommercial 授权范围。

| 输入 | 说明 · 来源 |
|---|---|
| `sources/beef-noodle.jpg` | 原图 [WnPghXNUnZM](https://unsplash.com/photos/WnPghXNUnZM) · @jyredrose |
| `sources/logo-laowan.png` | 演示品牌 Logo，本项目生成 |
| `sources/logo-shanyu.png` | 演示品牌 Logo，本项目生成 |
| `sources/logo-xiandao.png` | 演示品牌 Logo，本项目生成 |
| `sources/product-shanyu-coldbrew.jpg` | 演示商品图，本项目生成；底图 [7moPg-okWAI](https://unsplash.com/photos/7moPg-okWAI) · @elozanov |
