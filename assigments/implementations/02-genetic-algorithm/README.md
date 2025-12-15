# cc6mm-grupo5-assigment-2

## integrantes

- Paola Rioseco
- José Sanz
- Guillermo Barriga
- Guillermo Pinto
- Manuel Bórquez

## conda environment setup

```bash
# definición de entorno conda
conda env create -f environment.yml

# activación del entorno
conda activate cc6mm-grupo5-assigment-2

# registro del kernel
python -m ipykernel install --user --name cc6mm-grupo5-assigment-2 --display-name "Python (cc6mm-grupo5-assigment-2)"

# actualizar el entorno
conda env update --file environment.yml --prune 

# reinicio / limpieza
conda deactivate
conda clean --all --yes
conda remove -n cc6mm-grupo5-assigment-2 --all

```

## gpu

```bash
# verificación de acceso a GPU integrada al mac
python -c "import torch; print('PyTorch:', torch.__version__); print('Torchvision:', __import__('torchvision').__version__); print('MPS available:', torch.backends.mps.is_available())"
```