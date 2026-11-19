# Portfolio d'Armel Mounet

Site statique (HTML, CSS, JavaScript), sans serveur ni base de données, avec un assistant de discussion intégré.
Hébergement gratuit sur GitHub Pages : **https://andrearmel.github.io**

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `index.html` | Le site complet, avec l'assistant |
| `photo.jpg`, `hero.jpg` | Photos |
| `logos/` | Logos des entreprises, écoles et certifications |
| `cv.pdf` | **À ajouter** : ton CV, sous ce nom exact |

## Mise en ligne gratuite (sans installer Git)

1. Connecte-toi sur https://github.com avec le compte **Andrearmel**.
2. En haut à droite : **+** puis **New repository**.
   - Repository name : `Andrearmel.github.io` (exactement, avec ton nom d'utilisateur)
   - Visibilité : **Public**
   - Clique sur **Create repository**.
3. Sur la page du dépôt, clique sur le lien **uploading an existing file**.
4. Ouvre ton dossier dans l'Explorateur Windows, sélectionne **tout le contenu** (Ctrl + A) : `index.html`, `photo.jpg`, `hero.jpg`, `cv.pdf`, `README.md` et le dossier `logos`, puis glisse-le dans la page.
   Dépose bien le *contenu* du dossier, pas le dossier lui-même, pour que `index.html` soit à la racine.
5. En bas, clique sur **Commit changes**.
6. Va dans **Settings** puis **Pages** :
   - Source : **Deploy from a branch**
   - Branch : **main**, dossier **/ (root)**, puis **Save**.
7. Attends 1 à 2 minutes et ouvre **https://andrearmel.github.io**.

## Mettre à jour le site

Dans le dépôt : **Add file** puis **Upload files**, glisse le fichier modifié (il remplace l'ancien), puis **Commit changes**. Le site se met à jour en 1 à 2 minutes.

## Avec Git (PowerShell), si tu préfères

```powershell
cd "C:\Users\MOUNET_ANDRE_ARMEL_R\Downloads\MEMOIRE_MASTER_2\Nouveau dossier"
git init
git add index.html photo.jpg hero.jpg cv.pdf README.md logos
git commit -m "Portfolio"
git branch -M main
git remote add origin https://github.com/Andrearmel/Andrearmel.github.io.git
git push -u origin main
```

Les fichiers d'origine des logos (`.jfif`, `OCI.png`, `images.png`…) et `index_ancien.html` n'ont pas besoin d'être envoyés.

## Modifier les réponses de l'assistant

Dans `index.html`, cherche `const KB = [`. Chaque ligne associe des mots-clés (`k`, en minuscules et sans accents) à une réponse (`a`). Ajoute ou modifie une ligne sur le même modèle.
