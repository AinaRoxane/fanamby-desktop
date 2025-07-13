# Guide d’installation et d’utilisation de Fanamby


## Cas 1 : Installation via `.deb` (pour systèmes Ubuntu/Debian)

1. Copier le fichier `fanamby_0.1.0_amd64.deb` dans un dossier de votre système.

2. Ouvrir un terminal dans ce même dossier.

3. Exécuter les commandes suivantes :

```bash
sudo apt install libwebkit2gtk-4.1-0 libgtk-3-0 ffmpeg
sudo dpkg -i fanamby_0.1.0_amd64.deb
```

---

## Cas 2 : Installation à partir du code source (`source_code`)

Guide d'installation complet dans [Documentation Tauri](https://v1.tauri.app/v1/guides/getting-started/prerequisites/)
> Prérequis :
> * Node.js v20.19.0 minimum
> * Rustc v1.88.0 
> * FFmpeg installé (et accessible via le terminal)

1. Décompresser l’archive `source_code.zip`.

2. Ouvrir un terminal dans le dossier `svelterust/`.

3. Installer les dépendances avec la commande suivante :

```bash
npm install
```

4. Vérifier que `ffmpeg` fonctionne :

```bash
ffmpeg -version
```

---

## Lancer l’application

1. Ouvrir le menu des applications (en appuyant sur la touche "windows").

2. Rechercher **Fanamby**.

3. Lancer l’application depuis la liste des résultats.

---

## Utilisation de l’application

1. Cliquer sur le bouton "Workspace" puis le bouton "folder" pour choisir le dossier contenant votre vidéo.

2. Sélectionner ensuite, via filechooser, un fichier vidéo dans ce dossier.
Le chargement peut prendre entre 2 et 5 secondes.

3. Une fois la vidéo affichée, cliquer sur le bouton "Lecture" pour démarrer.

4. Pour déclencher l’analyse (extraction d’un extrait) soit:

   * taper deux fois sur le pavé tactile,
   * cliquer sur le bouton "Pause" du lecteur vidéo.

5. Remplir les champs du formulaire (nom du joueur, indicateur, secondes avant/après).

6. Cliquer sur le bouton pour extraire le clip.

---

## Sauvegarde des extraits

* Les extraits sont enregistrés dans un sous-dossier nommé :

  ```
  fanamby-YYYY-MM-DD
  ```

  Ce dossier est créé dans le même répertoire que la vidéo d’origine.

* Les fichiers extraits suivent ce format de nommage :

  ```
  joueur_[indicateur]_hh:mm:ss.mp4
  ```