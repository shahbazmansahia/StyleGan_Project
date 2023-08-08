-- FOR Google Cloud Host VM INSTANCE:
- "pip install gdown"
- "pip install -q condacolab"
- "wget https://repo.anaconda.com/archive/Anaconda3-2023.07-1-Linux-x86_64.sh"
- "pwd" ## make note of the output as it is the place where the installer file is downloaded
-  NOTE: HOME DIRECTORY WAS FULL SO WE INSTALLED IT IN BIN!
- "cd /bin"
- "bash <prefix: apply the directory path we got as output to pwd above>Anaconda3-2023.07-1-Linux-x86_64.sh"
- NOTE: if it creates the directory and crashes for some reason, try "bash <prefix: apply the directory path we got as output to pwd above>Anaconda3-2023.07-1-Linux-x86_64.sh -u"
- STEP: SPECIFY THE FILE DIRECTORY AFTER TERMS OF SERVICE 'yes' COMMAND TO '/BIN/'


-- ONCE YOU HAVE CONDA (LOCAL OR VM) 
- Install Nvidia CUDA drivers and setup Nvidia CuDNN on your machine [tested using CUDA 11.8 on a 4090: NOT RUNNING; 11.0 needed for cards below 3090/3000 series]
- create anaconda environment with python 3.7
- activate created anaconda environment
- run command: pip install notebook
- install pytorch-Cuda version 1.7.1 + 11.0 (tested) [IMPORTANT: USE PIP INSTALL VERSION; we used: "pip install torch==1.7.1+cu110 torchvision==0.8.2+cu110 torchaudio==0.7.2 -f https://download.pytorch.org/whl/torch_stable.html"]
- run command: pip install click requests tqdm pyspng ninja imageio-ffmpeg==0.4.3
- run command: pip install scipy

OPTIONAL: 
- install windows 10 SDK tools