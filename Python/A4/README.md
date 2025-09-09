# Activitat 4: Neteja de dades

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/UOC%2Feimt%2Fdatascience%2FLAB%2Fpython-cat/HEAD?urlpath=%2Fdoc%2Ftree%2FPython%2FA4%2Fneteja-dades.ipynb)

## Descripció

Aquesta activitat ensenya les tècniques essencials de neteja i preprocessament de dades, incloent la gestió de valors perduts, detecció d'outliers i normalització de dades.

## Contingut

- **Notebook principal**: `neteja-dades.ipynb`
- **Dades**: Dataset de metadades de pel·lícules per a exercicis de neteja

## Com executar

### Opció 1: Binder (Recomanat per a proves ràpides)
Feu clic al botó Binder de dalt per executar l'activitat al núvol sense necessitat d'instal·lació local.

### Opció 2: Entorn local
1. Assegureu-vos que teniu l'entorn `uoc-dmlab` configurat seguint les instruccions del [README principal](../../README.md)
2. Activeu l'entorn:
   ```bash
   conda activate uoc-dmlab
   ```
3. Navegueu a aquesta carpeta:
   ```bash
   cd Python/A4
   ```
4. Obriu el notebook:
   ```bash
   jupyter lab neteja-dades.ipynb
   ```

## Objectius d'aprenentatge

- Identificar i gestionar valors perduts (NaN, NULL)
- Detectar i tractar valors outliers
- Normalitzar i estandarditzar dades numèriques
- Netejar i reformatar dades de text
- Validar la qualitat de les dades després de la neteja
