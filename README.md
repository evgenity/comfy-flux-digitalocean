# comfy-flux-digitalocean

```
cd ../home
apt install python3-pip -y
git clone https://github.com/comfyanonymous/ComfyUI
cd ComfyUI
pip install -r requirements.txt

wget -O models/vae/ae.safetensors https://huggingface.co/second-state/FLUX.1-schnell-GGUF/resolve/main/ae.safetensors
wget -O models/diffusion_models/flux1-dev-fp8.safetensors https://huggingface.co/Comfy-Org/flux1-dev/resolve/main/flux1-dev-fp8.safetensors
wget -O models/clip/clip_l.safetensors https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/main/clip_l.safetensors
wget -O models/clip/t5xxl_fp8_e4m3fn.safetensors https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/main/t5xxl_fp8_e4m3fn.safetensors

wget -O models/checkpoints/v1-5-pruned-emaonly.ckpt https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt
```
