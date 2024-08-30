# Setup ComfyUI with Manager

### [Follow to install git and python](https://github.com/zohaibtariq/youtube-guides/blob/main/setup-git-python.md)

### Navigate to the folder where you want to install ComfyUI
```bash
mkdir ComfyUI
```

### Move Inside Created Directory
```bash
cd ComfyUI
```

### Clone ComfyUI repo
```bash
git clone https://github.com/comfyanonymous/ComfyUI .
```

---

### IMPORTANT NOTE

###### If you have two python versions installed on your OS python 2 and 3 then execute all python commands with python3 if you have only one python version with any version that is >= 3 you can use python as well

---

### Create new virtual environment
```bash
python -m venv ai
```

### Activate newly created virtual environment
```bash
source ai/bin/activate
```

### Install pytorch Nightly (Recommended) or take it from https://pytorch.org/
```bash
pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/whl/nightly/cpu
```

### Install ComfyUI requirements
```bash
pip install -r requirements.txt
```

### To install ComfyUI manager go to
```bash
cd custom_nodes
```

### Clone ComfyUI manager repo
```bash
git clone https://github.com/ltdrdata/ComfyUI-Manager
```

### Go to ComfyUI-Manager Folder
```bash
cd ComfyUI-Manager
````

### Install requirements
```bash
pip install -r requirements.txt
```

---
## IMPORTANT NOTE: If you want to use GGUF models for low vram or low specs hardware follow this

Make sure you are in the custom_nodes folder
```
cd ..
pip install --upgrade gguf
git clone git clone https://github.com/city96/ComfyUI-GGUF
cd ComfyUI-GGUF
pip install -r requirements.txt
```

---

### Go back to ComfyUI Folder
```bash
cd ../..
````

### Run ComfyUI local server with GPU

For non mac OS

```bash
python main.py --gpu-only
```

For mac

```bash
PYTORCH_ENABLE_MPS_FALLBACK=1 python main.py --gpu-only
```

### Run ComfyUI local server with CPU

For non mac OS

```bash
PYTORCH_ENABLE_MPS_FALLBACK=1 python main.py --cpu-only
```

For mac

```bash
PYTORCH_ENABLE_MPS_FALLBACK=1 python main.py --cpu-only
```

### Follow terminal link
```bash
http://127.0.0.1:8188/
```

#### Now you see ComfyUI over your browser with manager
- click on manager and click update all!

![Comfy UI + Manager](https://github.com/user-attachments/assets/5b780065-c578-4237-b55e-b9833b72ab2f)


- ALL DONE YOU ARE READY NOW
