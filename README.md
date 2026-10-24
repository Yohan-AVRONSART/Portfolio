# Portfolio — Yohan AVRONSART

Portfolio de Yohan AVRONSART, étudiant en MSc IA et Data à Epitech Paris (promo 2029).
Après plusieurs années de R&D dans l'optique, je me reconvertis dans l'informatique et je
recherche un stage ou une alternance en développement ou en data.

- **Site en ligne** : 
- **LinkedIn** : <https://www.linkedin.com/in/yohan-avronsart-973181307/>
- **GitHub** : <https://github.com/Yohan-AVRONSART>

## Contenu du site

Le site compte quatre pages, reliées par le même menu de navigation :

| Page | Fichier | Contenu |
|---|---|---|
| Accueil | `index.html` | Phrase d'accroche, photo, présentation, téléchargement du CV, lien LinkedIn |
| Projets | `projets.html` | Projets professionnels et scolaires : contexte, objectif, compétences, liens |
| Parcours | `parcours.html` | Ce que j'ai appris et comment j'ai progressé, formations, langues, centres d'intérêt |
| Contact | `contact.html` | Formulaire de contact |

## Structure du dépôt

```
Portfolio_AVRONSART_Yohan/
├── index.html          # Accueil
├── projets.html        # Projets
├── parcours.html       # Parcours
├── contact.html        # Contact
├── css/
│   ├── base.css        # Variables (couleurs, polices, espacements), reset, typographie
│   ├── layout.css      # Structure commune : en-tête, menu, pied de page, colonnes
│   └── components.css  # Composants : boutons, cartes, étiquettes, formulaire
├── assets/
│   ├── cv.pdf          # CV téléchargeable
│   └── photo_yohan.png # Photo de l'accueil
└── README.md
```

## Choix techniques

- **HTML et CSS uniquement**, sans framework, sans préprocesseur et sans JavaScript.
  Le site reste léger, et il n'y a aucune étape de build : les fichiers du dépôt sont
  exactement ceux qui sont publiés.
- **Convention BEM** pour nommer les classes (`card`, `card__links`, `card--placeholder`).
- **Variables CSS** dans `base.css` : couleurs et polices se changent à un seul endroit.
- **Responsive** : mises en page en grille et en flexbox, menu burger sur les écrans
  de moins de 700px, réalisé en CSS pur (astuce de la case à cocher).
- **Accessibilité** : lien « Aller au contenu », page active signalée par `aria-current`,
  texte alternatif sur la photo, titres hiérarchisés, menu utilisable au clavier.
- **SEO** : langue déclarée (`lang="fr"`), titre et meta description propres à chaque page.
- **Formulaire sans backend** : les messages sont transmis par e-mail via le service
  [FormSubmit](https://formsubmit.co/).

## Lancer le site en local

Aucune installation n'est nécessaire. Ouvrir `index.html` dans un navigateur, ou lancer
un petit serveur depuis le dossier du projet :

```bash
python3 -m http.server
```

puis ouvrir <http://localhost:8000>.

## Publication (GitHub Pages)

Le site est publié avec GitHub Pages, directement depuis la branche `main`.

Configuration, à faire une seule fois :

1. Sur GitHub, ouvrir le dépôt puis **Settings → Pages**.
2. Dans **Build and deployment → Source**, choisir **Deploy from a branch**.
3. Choisir la branche `main` et le dossier `/ (root)`, puis **Save**.

Ensuite, la publication est automatique : chaque `git push` sur `main` met le site en
ligne en une à deux minutes, sans autre action. L'avancement de chaque publication est
visible dans l'onglet **Actions** du dépôt.

## Ressources et crédits

- **Textes** : rédigés par moi.
- **Photo** : photo personnelle.
- **Polices** : polices système déjà installées sur l'appareil du visiteur
  (Segoe UI, Palatino, Georgia…), aucune police téléchargée.
- **Images, icônes et thèmes** : aucune ressource tierce. Le design et le CSS sont
  réalisés à la main.
- **Formulaire** : service gratuit [FormSubmit](https://formsubmit.co/).

## Auteur

**Yohan AVRONSART** — Epitech, MSc Pro IA et Data, promo 2029
