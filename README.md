# super_resolution
## 本地的超分辨率工具

重要的依赖:

    pytorch                  pip install torch torchvision torchaudio    (如果想要能调用显卡的cuda, 请好好安装pytorch, 验证方法见下) 
    realesrgan
    basicsr
    
    
```python
import torch
print(torch.cuda.is_available()) 
```
 
其他依赖项
    imageio
    numpy
    loguru
    PIL
    httpx
    typing


我认为你应该有的依赖:
    io
    time
    json
    asyncio
    pathlib
    nonebot2
    nonebot-adapter-onebot
    
    
 注释已补全, 详细运行逻辑请看注释
