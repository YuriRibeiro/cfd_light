# Traffic Vehicle Counter

This code is desgined to use object detection + tracking algorithms to track and count vehicles on videos.

Implemented Object Detectors:
- YOLOv5 (S, M, L, X)
- YOLOv3 (tiny, yv3, yv3-spp)

Implemented Tracking Algorithms:
- SORT


# Install
- Donwload this repo source code, via `git clone` or zip file (and unzip it).

- Download and install Python from [Python Official Website](https://www.python.org/) or [Anaconda](https://anaconda.org/), for example.

- Then, use your package manager to create a virtual environment *envname* with Python version greather or equal to 3.9.0, cd to the source code folder and pip install requirements.txt, such as:


```bash
conda create --name envname python=3.9.0

conda activate envname

cd source_code_folder_path

pip install -r requirements.txt
```

- Windows users: If you see an error like *'error: Microsoft Visual C++ 14.0 is required'* while pip is running, you'll have to install C++ Build Tools: download [Visual Studio Free](https://visualstudio.microsoft.com/downloads/), open the installer, select 'Individual Components', and check the following options to install:
  - Recursos principais das Ferramentas de Build do C++
  - Recursos principais do C++
  - Atualização do Pacote Redistribuível do C++ 2019
  - Ferramentas de build do MSVC v142 - VS 2019  C++ x64/86 (Mais recente)
  - Ferramentas do CMake do C++ para Windows
  - Transformação de Modelo de Texto
  - Runtime do Windows Universal C
  - SDK do Windows 10 (10.0.19041.0)


## Download Weights

Download the weights from my [Google Drive](https://drive.google.com/drive/folders/1UKGe3j5kFLnsjhHriimofuZX5dn3k3dY?usp=sharing).
Place them at `./Weights`.

# How to Use

The easy way: jupyter notebooks! Open yout terminal and:

```
conda activate envname

jupyter notebook
```

You should use the *envname* kernel on jupyter notebook. If it's necessary, "install" the kernel and restart the notebook:
```
python -m ipykernel install --user --name=envname
```

Then, navigate to the `interface_traffic_vehicle_counter.ipynb` and run it!

To define the counting barriers, there are two jupyter notebooks to help doing it: 

- `interface_define_barriers_jupyter`: Define barriers just via browser, it's nice if you use remote location server.

- `interface_define_barriers_opencv`: Define barrier using opencv package and works only for local machine. It's faster than the *interface_define_barriers_jupyter*.

*If yout want to use command line, please refer to the source code.*


# Extra
-  https://github.com/YuriRibeiro/cfd -- Research repository.

