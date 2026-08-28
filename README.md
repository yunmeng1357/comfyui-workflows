ComfyUI 工作流合集

个人常用的 ComfyUI 批量生图工作流，支持在本地 ComfyUI 或 RunningHub 等云端平台运行。


工作流列表

1. 女侠批量生图（古风主题）
   模型：Krea2-turbo-White_Marble-AIO_V1_BF16
   参数：512x512，batch_size=3，euler采样器，20步，CFG=8
   用途：批量生成统一风格的古风女侠图片
   文件：空白工作流_api.json

2. 赛博城市批量生图（科幻主题）
   模型：epicrealism_pureEvolutionV5-inpainting
   参数：512x512，batch_size=3，euler采样器，20步，CFG=8
   用途：批量生成赛博朋克风格科幻场景
   文件：工作流_api.json


使用说明

1. 下载对应的 JSON 文件
2. 拖入 ComfyUI 界面 或 上传至 RunningHub
3. 修改正向提示词中的主题描述，更换生成内容
4. 调整 batch_size 控制单次生成数量
5. 点击 Queue Prompt 运行


参数说明

width / height：生成图片分辨率
batch_size：单次生成数量
steps：采样步数（20步平衡速度与质量）
CFG：提示词引导强度（推荐值8）
sampler_name：euler / scheduler：simple
