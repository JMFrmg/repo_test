# Lancement des modèles Rank_IQA, hyperUQA et ava_mlsp

## Instrcutions pour les modèles rank_IQA et ava_mlsp :
En console se positionner dans le répertoire du modèle à tester (ex : /home/matthieu/Documents/projets/adas_decisional_system/model_testing/ava_mlsp)

Créer un environnement virtuel avec Conda : 
```console
conda create --name nom_de_l_environnement python=3.7.10 
```
Charger l'environnement virtuel :  
```console
source nom_de_l_environnement/bin/activate  
```
Installer les dépendances :  
```console
pip install -r requirements.txt 
```
Lancer le modèle :  
```console
python main.py path_absolu_de_l_image  
```  
La prédiction sera affichée en console.
  
## Instructions pour hyper_IQA :
En console se positionner dans le répertoire du modèle à tester (ex : /home/matthieu/Documents/projets/adas_decisional_system/model_testing/ava_mlsp)  

Créer un environnement virtuel avec Conda :  
```console
conda create --name nom_de_l_environnement python=3.7.10  
```
Charger l'environnement virtuel :  
```console
conda activate nom_de_l_environnement  
```
Le Github de référence du modèle hyperIQA utilise la version 0.4 de pytorch.  
Cette dernière n'est pas compatible avec les dernières versions de cuda.  
Vérifier la présence de cuda dans les paquest installés :  
```console
conda list  
```
Désinstaller cuda :  
```console
conda uninstall cuda  
```
Installer les dépendances :  
```console
pip install -r requirements.txt  
```
Lancer le modèle :  
```console
python main.py path_absolu_de_l_image  
```

# Papiers et Githubs sources des modèles  
### Rank_IQA  
Papier : https://paperswithcode.com/paper/rankiqa-learning-from-rankings-for-no  
Github : https://github.com/YunanZhu/Pytorch-TestRankIQA  
### Hyper_IQA  
Papier : https://paperswithcode.com/paper/blindly-assess-image-quality-in-the-wild  
Github : https://github.com/SSL92/hyperIQA  
### ava_mlsp  
Papier : https://paperswithcode.com/paper/effective-aesthetics-prediction-with-multi  
Github : https://github.com/subpic/ava-mlsp  
