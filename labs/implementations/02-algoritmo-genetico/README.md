# cc66m-grupo5-lab2

## integrantes

- Paola Rioseco
- José Sanz
- Guillermo Barriga
- Guillermo Pinto
- Manuel Bórquez

## hardware

- **Model**: MacBook Pro 14" (2023)  
- **Chip**: Apple M2 Max (12-core CPU, 38-core GPU, 16-core Neural Engine)  
- **Architecture**: arm64 (Apple Silicon)  
- **Memory**: 32 GB unified RAM  
- **Graphics**: Integrated Apple GPU with full Metal 4 support  
- **OS**: macOS 26.0 (Build 25A354)  

## conda environment setup

```bash
# definición de entorno conda
conda env create -f environment.yml

# activación del entorno
conda activate cc66m-grupo5-lab2

# registro del kernel
python -m ipykernel install --user --name cc66m-grupo5-lab2 --display-name "Python (cc66m-grupo5-lab2)"

# actualizar el entorno
conda env update --file environment.yml --prune 

# reinicio / limpieza
conda deactivate
conda clean --all --yes
conda remove -n cc66m-grupo5-lab2 --all

```

## gpu

```bash
# verificación de acceso a GPU integrada al mac
python -c "import torch; print('PyTorch:', torch.__version__); print('Torchvision:', __import__('torchvision').__version__); print('MPS available:', torch.backends.mps.is_available())"
```