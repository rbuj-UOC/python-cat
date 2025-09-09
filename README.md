# UOC - Laboratori de Python i R

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/UOC%2Feimt%2Fdatascience%2FLAB%2Fpython-cat/HEAD?urlpath=%2Fdoc%2Ftree%2FPython%2FA1%2Finstalacio-programari-python.ipynb)

Aquest repositori conté materials educatius per al **Laboratori de Python i R** de la UOC (Universitat Oberta de Catalunya). El laboratori està estructurat com una col·lecció de notebooks de Jupyter organitzats per activitats que ensenyen progressivament conceptes de ciència de dades amb Python.

## Estructura del Repositori

```
Python/
├── A1/  # Instal·lació de programari Python i introducció als notebooks Jupyter
├── A2/  # Lectura i escriptura de fitxers de dades (CSV, Excel, JSON, ZIP)
├── A3/  # Manipulació de dades amb pandas
├── A4/  # Tècniques de neteja de dades
├── A5/  # Estadística descriptiva
├── A6/  # Visualització de dades
├── A7/  # Avaluació de models
└── A8/  # Exemple complet de flux de treball
```

## Configuració de l'Entorn Virtual

Hi ha dues opcions per configurar l'entorn de desenvolupament: **Conda** (recomanat) o **pip amb venv**.

### Opció 1: Conda (Recomanat)

#### Prerequisits
- Anaconda o Miniconda instal·lat al vostre sistema
- Descarregueu Anaconda des de: https://www.anaconda.com/products/distribution

#### Configuració
1. **Crear l'entorn des del fitxer environment.yml:**
   ```bash
   conda env create -f environment.yml
   ```

2. **Activar l'entorn:**
   ```bash
   conda activate uoc-dmlab
   ```

3. **Verificar la instal·lació:**
   ```bash
   conda list
   ```

4. **Iniciar Jupyter:**
   ```bash
   jupyter lab
   ```
   o
   ```bash
   jupyter notebook
   ```

#### Gestió de l'entorn Conda
- **Desactivar l'entorn:** `conda deactivate`
- **Eliminar l'entorn:** `conda env remove -n uoc-dmlab`
- **Actualitzar l'entorn:** `conda env update -f environment.yml`
- **Exportar l'entorn:** `conda env export > environment.yml`

### Opció 2: pip amb venv

#### Prerequisits
- Python 3.9 o superior instal·lat al vostre sistema

#### Configuració
1. **Crear un entorn virtual:**
   ```bash
   python -m venv uoc-dmlab-env
   ```

2. **Activar l'entorn virtual:**
   
   **En Windows:**
   ```bash
   uoc-dmlab-env\Scripts\activate
   ```
   
   **En macOS/Linux:**
   ```bash
   source uoc-dmlab-env/bin/activate
   ```

3. **Actualitzar pip:**
   ```bash
   pip install --upgrade pip
   ```

4. **Instal·lar les dependències:**
   ```bash
   pip install -r requirements.txt
   ```

5. **Instal·lar Jupyter (si no està inclòs):**
   ```bash
   pip install jupyter jupyterlab
   ```

6. **Iniciar Jupyter:**
   ```bash
   jupyter lab
   ```

#### Gestió de l'entorn pip
- **Desactivar l'entorn:** `deactivate`
- **Eliminar l'entorn:** Simplement elimineu la carpeta `uoc-dmlab-env`
- **Generar requirements.txt:** `pip freeze > requirements.txt`

## Llibreries Principals

El curs utilitza les següents llibreries clau:

- **pandas** - Manipulació i anàlisi de dades
- **numpy** - Computació numèrica
- **matplotlib** - Visualització bàsica
- **seaborn** - Visualització estadística
- **scikit-learn** - Algoritmes d'aprenentatge automàtic
- **jupyter** - Notebooks interactius

## Començar

### Opció 1: Binder (Recomanat per a proves ràpides)
La manera més ràpida de començar és utilitzant Binder. Feu clic al botó Binder de dalt per executar tots els notebooks al núvol sense necessitat d'instal·lació local.

### Opció 2: Entorn local
1. **Configureu l'entorn** seguint una de les opcions anteriors
2. **Navegueu fins a la carpeta Python:**
   ```bash
   cd Python
   ```
3. **Comenceu amb l'Activitat 1:**
   ```bash
   jupyter lab "A1/instalacio-programari-python.ipynb"
   ```

## Estructura de les Activitats

Cada carpeta d'activitat conté:
- Un notebook principal de Jupyter (.ipynb) amb exercicis i explicacions
- Carpeta `data/` amb conjunts de dades utilitzats en els exercicis
- Carpeta `images/` amb imatges i diagrames de suport

## Activitats del Laboratori

1. **Activitat 1**: Configuració de l'entorn amb Anaconda, introducció a Jupyter
2. **Activitat 2**: Operacions d'E/S de fitxers (formats CSV, Excel, JSON, ZIP)
3. **Activitat 3**: Tècniques de manipulació de dades amb pandas
4. **Activitat 4**: Neteja i preprocessament de dades
5. **Activitat 5**: Anàlisi estadística i estadística descriptiva
6. **Activitat 6**: Tècniques de visualització de dades
7. **Activitat 7**: Avaluació de models d'aprenentatge automàtic
8. **Activitat 8**: Exemple de flux de treball complet de ciència de dades

## Resolució de Problemes

### Problemes comuns amb Conda
- **Error "conda: command not found"**: Assegureu-vos que Anaconda/Miniconda estigui instal·lat i afegit al PATH
- **Conflictes de dependències**: Proveu `conda clean -a` i torneu a crear l'entorn

### Problemes comuns amb pip
- **Errors de permisos**: Utilitzeu `--user` flag o assegureu-vos que l'entorn virtual estigui activat
- **Versions incompatibles**: Assegureu-vos d'utilitzar Python 3.9+

### Problemes amb Jupyter
- **Kernel no trobat**: Instal·leu ipykernel: `pip install ipykernel` o `conda install ipykernel`
- **Port ja en ús**: Especifiqueu un port diferent: `jupyter lab --port=8889`
