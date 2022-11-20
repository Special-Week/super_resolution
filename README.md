# super_resolution
## 本地的超分辨率工具

重要的依赖:

    pytorch                  pip install torch torchvision torchaudio    (如果想要能调用显卡的cuda, 请好好安装pytorch, 验证方法见下) 
    realesrgan               pip install realesrgan                      (先安装好torch)
    basicsr                  pip install basicsr
    
    
```python
import torch
print(torch.cuda.is_available()) 
```
 
其他依赖项

    imageio                    pip install imageio
    numpy                      pip install numpy    
    loguru                     pip install loguru      
    PIL                        pip install pillow    
    httpx                      pip install httpx    
    nonebot2                   pip install nonebot2    
    nonebot.adapters.onebot    pip install nonebot-adapter-onebot


我认为你应该有的依赖:

    io    
    time    
    asyncio    
    json    
    pathlib    
    typing
    
    
    
导包部分:
```python
import io
import time
import json
import asyncio
import imageio
import numpy as np
from io import BytesIO
from pathlib import Path
from loguru import logger
from PIL import Image as IMG
from PIL import ImageSequence
from httpx import AsyncClient
from typing import Union, List
from nonebot import on_command
from nonebot.typing import T_State
from realesrgan import RealESRGANer
from nonebot.params import Arg, Depends
from basicsr.archs.rrdbnet_arch import RRDBNet
from nonebot.adapters.onebot.v11 import Message, MessageEvent, MessageSegment
```
    
    
 注释已补全, 详细运行逻辑请看注释
