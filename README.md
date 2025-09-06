# Small Appliance AI Workflows (ComfyUI + ControlNet)

为**小家电**定制：2 个 ComfyUI 工作流 + 中文提示词。

## 3 步上手
1) 打开 ComfyUI。
2) 导入工作流：`workflows/ComfyUI/SmallAppliance_Text2ProductShot_SDXL.json`（文生图）与 `workflows/ComfyUI/SmallAppliance_Sketch2Render_SDXL_Canny.json`（草图控形）。
3) 放模型到 ComfyUI：`models/checkpoints/`（SDXL 主模型），`models/controlnet/`（SDXL Canny）。填提示词/上传线稿→运行。

## 默认提示词
正面：
小家电产品图，几何简洁，人体工学友好，磨砂铝合金+哑光PC+抛光玻璃，45°三分之二视角，摄影棚三点布光，中性灰纯背景，广告级写实，细节锐利，超清

负面：
文字、水印、logo 拼写错误、比例夸张、畸变、断裂、低清晰度、过度反光、塑料感、涂抹、噪点、手绘风、卡通风、过曝、过饱和

## 风格微调（附加在正面提示尾部即可）
- 极简（Braun 向）：几何纯粹、低对比、黑白灰、高级哑光、细分缝、微R角、无装饰
- 科技（Dyson 向）：功能暴露、通透结构、阴影对比强、金属拉丝+高亮塑料、冷调光、紫/银点缀
- 温润（MUJI 向）：米白/浅灰配色、哑光、R角柔和、柔光箱、无高光热点

## 参数建议
尺寸 1024×1024（显存不足用 896/768）；steps 22–32，CFG 4.5–6.5；ControlNet strength 0.8–1.0。