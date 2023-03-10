
# 三分鐘搞定Stable Diffusion！不需要gpu
## 第一步 打開https://colab.research.google.com/

## 第二步 開始安裝 打开GPU选项
```python
!pip install --upgrade fastapi==0.90.1
!git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui
!git clone https://github.com/yfszzx/stable-diffusion-webui-images-browser /content/stable-diffusion-webui/extensions/stable-diffusion-webui-images-browser
!curl -Lo chilloutmixni.safetensors https://huggingface.co/nolanaatama/chomni/resolve/main/chomni.safetensors
!curl -Lo ulzzang-6500.pt https://huggingface.co/nolanaatama/chomni/resolve/main/ulzzang-6500.pt
!mv "/content/chilloutmixni.safetensors" "/content/stable-diffusion-webui/models/Stable-diffusion"
!mv "/content/ulzzang-6500.pt" "/content/stable-diffusion-webui/embeddings"
%cd /content/stable-diffusion-webui
!COMMANDLINE_ARGS="--share --disable-safe-unpickle --skip-torch-cuda-test --no-half-vae --xformers --reinstall-xformers --enable-insecure-extension-access" REQS_FILE="requirements.txt" python launch.py
```

## 第三步 打开生成链接算圖
```
**算圖參數(上面的框框)**
(8k, RAW photo, best quality, masterpiece:1.2), (realistic, photo-realistic:1.37), ultra-detailed,full body,1 girl, solo,beautiful detailed sky,detailed tokyo street,night,beautiful detailed eyes,beautiful detailed lips,professional lighting, photon mapping, radiosity, physically-based rendering,extremely detailed eyes and face, beautiful detailed eyes,light on face,cinematic lighting, short jacket,hoodie,school uniform,1girl,full body,full-body shot,see-through,looking at viewer,outdoors,((white hair)),
**算圖參數(下面的框框)**
EasyNegative, paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans,extra fingers,fewer fingers,strange fingers,bad hand,signature, watermark, username, blurry, bad feet,bad leg, duplicate, extra limb, ugly, disgusting, poorly drawn hands, missing limb, floating limbs, disconnected limbs, malformed hands, blurry,mutated hands and fingers,, EasyNegative, paintings, sketches, (worst quality:2), (low quality:2), (normal quality:2), lowres, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, glans,extra fingers,fewer fingers,strange fingers,bad hand,signature, watermark, username, blurry, bad feet,bad leg
```
