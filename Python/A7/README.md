# Activitat 7: Avaluació de models

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/UOC%2Feimt%2Fdatascience%2FLAB%2Fpython-cat/HEAD?urlpath=%2Fdoc%2Ftree%2FPython%2FA7%2Favaluacio-model.ipynb)

## Descripció

Aquesta activitat se centra en l'avaluació de models d'aprenentatge automàtic, incloent mètriques de rendiment, validació creuada i tècniques de selecció de models.

## Contingut

- **Notebook principal**: `avaluacio-model.ipynb`
- **Dades**: Dataset del Titanic net per a exercicis de modelització
- **Imatges**: Diagrames sobre precisió vs accuracy i algoritmes de ML

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
   cd Python/A7
   ```
4. Obriu el notebook:
   ```bash
   jupyter lab avaluacio-model.ipynb
   ```

## Objectius d'aprenentatge

- Entendre mètriques d'avaluació (precisió, recall, F1-score)
- Implementar validació creuada
- Crear matrius de confusió
- Comparar diferents models d'aprenentatge automàtic
- Interpretar resultats i seleccionar el millor model
