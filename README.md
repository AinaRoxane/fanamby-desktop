# 📘 Guide d’installation et d’utilisation de **Fanamby**

## 🧩 Cas 1 : Installation via `.deb` (recommandé pour Ubuntu/Debian)

1. **Copiez** le fichier `fanamby_0.1.0_amd64.deb` dans un dossier de votre système (Ubuntu/Debian).

2. **Ouvrez un terminal** dans ce même dossier.

3. **Exécutez les commandes suivantes dans le terminal :**

```bash
sudo apt install libwebkit2gtk-4.1-0 libgtk-3-0 ffmpeg
sudo dpkg -i fanamby_0.1.0_amd64.deb
```

---

## 🛠️ Cas 2 : Installation depuis les sources (`source_code`)

> ⚠️ Vous aurez besoin de **Node.js (≥ v20.19.0)**, **Rust**, et **FFmpeg** installés sur votre machine.
> Consultez : [https://v1.tauri.app/v1/guides/getting-started/prerequisites/](https://v1.tauri.app/v1/guides/getting-started/prerequisites/)

1. Décompressez l’archive `source_code.zip`.

2. Ouvrez un terminal dans le dossier `svelterust/`.

3. Exécutez la commande suivante pour installer les dépendances :

```bash
npm install
```

4. Vérifiez que la commande suivante fonctionne dans votre terminal :

```bash
ffmpeg -version
```

---

## 🚀 Lancement de l’application

4. Ouvrez le menu **Windows** (ou la recherche d'applications de votre système) et tapez **Fanamby**.
   L'application devrait apparaître dans les résultats. Cliquez pour la lancer.

---

## 🎬 Utilisation

5. Une fois l’interface chargée :

* Cliquez sur **Workspace** (bouton avec l’icône `Folder`) pour sélectionner le dossier contenant votre vidéo.
* Cliquez ensuite sur le sélecteur de fichier pour choisir la vidéo à analyser.
  *🕒 Le chargement peut prendre entre 2 et 10 secondes.*

6. La vidéo s'affichera à l’écran. Cliquez sur lecture (`Play`) pour la visionner.

7. Pour capturer un extrait :

* **Double-tapez** sur le pavé tactile, **ou**
* **Cliquez** sur le bouton `Pause` du lecteur pour faire apparaître le formulaire de découpage.

---

## 💾 Sauvegarde des extraits

* Les extraits sont automatiquement enregistrés dans un dossier :

  ```
  fanamby-AAAA-MM-JJ
  ```

  situé dans le **même répertoire** que la vidéo source.

* Le nom de chaque extrait suit ce format :

  ```
  joueur_[indicateur]_hh:mm:ss.mp4
  ```