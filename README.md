# 🏆 KilnHackathon - Programme de Points 🎯

__KilnHackathon__ est un projet visant à améliorer la fidélisation des utilisateurs de vaults Defi sur Kiln. En utilisant un modèle "Points as a Service", notre solution récompense la fidélité des utilisateurs en attribuant des points basés sur leur participation au staking et à d'autres activités.

## Sommaire

- [Structure du projet](#structure-du-projet)
- [Fonctionnalités](#fonctionnalités)
- [Langages utilisées](#langages-utilisées)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Auteurs](#auteurs)

## Structure du projet

Le projet est organisé comme suit :

```
KilnHackathon/
├── src/
│   ├── back/
│   │   └── api.py
│   │   
│   ├── front/
│   │   └── (fichiers front-end HTML, CSS)
├── README.md
```

- **src/back/** : Contient les scripts backend, notamment le fichier `test.py` pour tester l'API.
- **src/front/** : Contient les fichiers front-end (HTML, CSS) pour l'interface utilisateur.
- **README.md** : Documentation du projet.

## Fonctionnalités

- **Attribution de points** : Calcul des points de fidélité en fonction des activités des utilisateurs sur les vaults.
- **API Flask** : Fournit une interface permettant de récupérer les points de staking via des requêtes HTTP.
- **Interface utilisateur** : Présente les informations sur les points et l'expérience utilisateur.

## Langages utilisées

- **HTML** : Utilisé pour la structure des pages front-end.
- **CSS** : Utilisé pour le style et la mise en page.
- **Python** : Utilisé pour le traitement des données et l'API Flask.

## Installation

1. Clonez le dépôt :
   ```bash
   git clone https://github.com/charlyppr/KilnHackathon.git
   ```

2. Accédez au répertoire du projet :
   ```bash
   cd KilnHackathon
   ```

3. Créez un environnement virtuel :
   ```bash
   python -m venv venv
   ```

4. Activez l'environnement virtuel :
   - Sur Windows :
     ```bash
     venv\Scripts\activate
     ```
   - Sur macOS/Linux :
     ```bash
     source venv/bin/activate
     ```

5. Installez les dépendances nécessaires :
   ```bash
   pip install Flask
   ```

6. Démarrez l'application Flask :
   ```bash
   python src/back/test.py
   ```

## Utilisation

1. Assurez-vous que l'application Flask est en cours d'exécution.
2. Accédez à `http://127.0.0.1:5000/` pour voir l'interface utilisateur.
3. Pour calculer les points de staking, utilisez le point de terminaison `/points` avec les paramètres `wallet` et `vault`.

Exemple de requête via cURL :
```bash
curl "http://127.0.0.1:5000/points?wallet=VOTRE_ADRESSE_WALLET&vault=VOTRE_ADRESSE_VAULT"
```

## Auteurs

[Simon Hamelin](https://github.com/Simonhamel1)  
[Ewan Clabaut](https://github.com/Clab-ewan)  
[Charly Pupier](https://github.com/charlyppr/)
