# Setup ComfyUI with Manager

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

### To install ComfyUI manager go to
```bash
cd custom_nodes
```

### Clone ComfyUI manager repo
```bash
git clone https://github.com/ltdrdata/ComfyUI-Manager
```

### Back to main Folder
```bash
cd ..
````

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

### Install requirements
```bash
pip install -r requirements.txt
```

### Run ComfyUI local server with GPU
```bash
python3 main.py --gpu-only
```

### Run ComfyUI local server with CPU
```bash
python main.py --cpu-only
```

### Follow terminal link
```bash
http://127.0.0.1:8188/
```

#### Now you see ComfyUI over your browser with manager
- click on manager and click update all!

![Comfy UI + Manager](https://github.com/user-attachments/assets/5b780065-c578-4237-b55e-b9833b72ab2f)


- ALL DONE YOU ARE READY NOW
