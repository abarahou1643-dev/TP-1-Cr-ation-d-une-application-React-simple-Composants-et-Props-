
# TP React - Application de Composants et Props

##  Accès au Projet

### Lien Google Drive
**[👉 CLIQUEZ ICI POUR ACCÉDER AU PROJET COMPLET SUR GOOGLE DRIVE](https://drive.google.com/drive/folders/votre-lien-ici?usp=sharing)**

*Le projet est hébergé sur Google Drive en raison de la taille des fichiers node_modules qui dépasse les limites de GitHub.*

---


## 📋 Objectif du Projet
Ce TP vise à consolider les connaissances en React par la création d'une application complète étape par étape. À la fin de ce TP, vous serez capable de :

- Initialiser un projet React avec Create React App
- Créer et intégrer des composants fonctionnels avec JSX
- Utiliser les props pour transmettre des données entre composants
- Structurer efficacement une application React
- Valider les données avec PropTypes

##  Fonctionnalités Implémentées

### Composants Créés
1. **HelloWorld** - Composant d'introduction simple
2. **Greeting** - Composant de salutation personnalisable avec props
3. **Profil** - Composant de profil utilisateur avec image et validation
4. **Voiture** - Composant d'affichage de véhicules avec caractéristiques
5. **ListeCourses** - Composant de listes dynamiques

### Technologies Utilisées
-  **React** 18.x
-  **CSS-in-JS** (Styled Components)
-  **PropTypes** pour la validation
-  **Images externes** (Pravatar)

##  Structure du Projet

```
tp-react/
├── public/
│   ├── index.html
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── HelloWorld.js
│   │   ├── Greeting.js
│   │   ├── Profil.js
│   │   ├── Voiture.js
│   │   └── ListeCourses.js
│   ├── App.js
│   ├── App.css
│   ├── index.js
│   └── index.css
├── package.json
└── README.md
```

##  Installation et Exécution

### Prérequis
- Node.js (version 14 ou supérieure)
- npm ou yarn

### Étapes d'installation

1. **Télécharger le projet depuis Google Drive**
   - Accédez au lien Drive ci-dessus
   - Téléchargez le dossier `tp-react` complet

2. **Ouvrir le projet**
   ```bash
   cd tp-react
   ```

3. **Installer les dépendances**
   ```bash
   npm install
   ```

4. **Démarrer l'application**
   ```bash
   npm start
   ```

5. **Ouvrir dans le navigateur**
   ```
   http://localhost:3000
   ```

##  Scripts Disponibles

- `npm start` - Lance le serveur de développement
- `npm run build` - Crée une version de production
- `npm test` - Lance les tests
- `npm run eject` - Éjecte la configuration (irréversible)

##  Composants Détaillés

### HelloWorld
```jsx
function HelloWorld() {
  return <h1>Hello World !</h1>;
}
```

### Greeting
```jsx
function Greeting({ prenom }) {
  return <h2>Bonjour, {prenom} !</h2>;
}
```

### Profil
```jsx
function Profil({ utilisateur, taille }) {
  return (
    <div>
      <img src={utilisateur.photo} width={taille} alt={utilisateur.nom} />
      <p>{utilisateur.nom}</p>
    </div>
  );
}
```

##  Validation des Props

Le projet utilise **PropTypes** pour valider les données :

```jsx
Profil.propTypes = {
  utilisateur: PropTypes.shape({
    nom: PropTypes.string.isRequired,
    photo: PropTypes.string.isRequired,
  }).isRequired,
  taille: PropTypes.number,
};
```

##  Fonctionnalités Avancées

-  **Composants réutilisables**
-  **Props dynamiques**
-  **Validation de types**
-  **Stylage moderne**
-  **Images externes**
-  **Listes dynamiques**

##  Design et Interface

L'application utilise un design moderne avec :
- Cartes avec ombres portées
- Dégradés de couleurs
- Bordures arrondies
- Espacement cohérent
- Typographie responsive

##  Apprentissages Clés

### Concepts React Maîtrisés
1. **Composants fonctionnels**
2. **JSX et rendu conditionnel**
3. **Props et transmission de données**
4. **PropTypes et validation**
5. **Structure d'application**
6. **Gestion des styles**

### Bonnes Pratiques Implémentées
- Séparation des préoccupations
- Composants modulaires
- Code maintenable
- Validation des données
- Documentation claire

## Dépendances

### Principales
```json
{
  "react": "^18.2.0",
  "react-dom": "^18.2.0",
  "react-scripts": "5.0.1",
  "prop-types": "^15.8.1"
}
```

### Développement
```json
{
  "web-vitals": "^2.1.4"
}
```

##  Note Importante

**Pourquoi Google Drive ?**
- Le dossier `node_modules` est très volumineux (~200MB)
- GitHub a des limitations de taille pour les fichiers
- Google Drive permet le partage de projets complets

##  Démonstration de l'Application

<img width="959" height="473" alt="1" src="https://github.com/user-attachments/assets/7a103193-77fc-4641-be2f-d5cf2876da6f" />


<img width="959" height="539" alt="2" src="https://github.com/user-attachments/assets/12ed1382-f2ff-4ea6-a652-8074dd72c503" />




https://github.com/user-attachments/assets/c872a939-a15a-4962-9723-9295ae73658f




##  Conclusion

Ce TP démontre une maîtrise complète des concepts fondamentaux de React, incluant la création de composants, l'utilisation des props, la validation des données et la structuration d'applications. L'application est fonctionnelle, bien structurée et prête pour l'ajout de fonctionnalités avancées.

---

** Lien Drive : [https://drive.google.com/drive/folders/votre-lien-ici?usp=sharing](https://drive.google.com/drive/folders/votre-lien-ici?usp=sharing)**

