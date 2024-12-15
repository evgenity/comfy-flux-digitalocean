# comfy-flux-digitalocean

```
export DEBIAN_FRONTEND=noninteractive
apt-get update
apt install python3-pip -y
git clone https://github.com/comfyanonymous/ComfyUI
cd ComfyUI
pip install -r requirements.txt

cd custom_nodes
git clone https://github.com/ltdrdata/ComfyUI-Manager.git
cd ..
python3 main.py --listen
```

```
wget -O models/vae/ae.safetensors https://huggingface.co/second-state/FLUX.1-schnell-GGUF/resolve/main/ae.safetensors &
wget -O models/checkpoints/flux1-dev-fp8.safetensors https://huggingface.co/Comfy-Org/flux1-dev/resolve/main/flux1-dev-fp8.safetensors &
wget -O models/clip/clip_l.safetensors https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/main/clip_l.safetensors &
wget -O models/clip/t5xxl_fp8_e4m3fn.safetensors https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/main/t5xxl_fp8_e4m3fn.safetensors &

wget -O models/checkpoints/v1-5-pruned-emaonly.ckpt https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt &

mkdir models/controlnet/sdxl &
wget -O models/controlnet/sdxl/OpenPoseXL2.safetensors https://huggingface.co/thibaud/controlnet-openpose-sdxl-1.0/resolve/main/OpenPoseXL2.safetensors &

wget -O models/upscale_models/4x-ClearRealityV1.pth https://huggingface.co/skbhadra/ClearRealityV1/resolve/main/4x-ClearRealityV1.pth &

mkdir models/controlnet/FLUX.1/ &
wget -O models/controlnet/FLUX.1/diffusion_pytorch_model.safetensors https://huggingface.co/InstantX/FLUX.1-dev-Controlnet-Union/resolve/main/diffusion_pytorch_model.safetensors &

wget -O ./models/checkpoints/wildcardx-xl-turbo.safetensors https://civitai.com/api/download/models/329685?token=87b492a24c967ed812dbacc4a323c8bb&

wget -O models/checkpoints/flux1-dev.safetensors https://huggingface.co/black-forest-labs/FLUX.1-dev/resolve/main/flux1-dev.safetensors --header="Authorization: Bearer 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"
```

```
mkdir models/loras/flux
wget -O ./models/loras/flux/961155.safetensors https://civitai.com/api/download/models/961155?token=87b492a24c967ed812dbacc4a323c8bb
```

```
export GRADIO_SERVER_NAME="0.0.0.0"
git clone https://github.com/cocktailpeanut/fluxgym
cd fluxgym
git clone -b sd3 https://github.com/kohya-ss/sd-scripts

cd sd-scripts
pip install -r requirements.txt

cd ..
pip install -r requirements.txt

pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
```
