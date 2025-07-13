# Guide d’installation et d’utilisation de Fanamby

## Installation

1. **Copiez** le fichier `fanamby_0.1.0_amd64.deb` dans un répertoire de votre système d’exploitation (Ubuntu/Debian).

2. **Ouvrez un terminal** dans ce même répertoire.

3. **Exécutez les commandes suivantes dans le terminal :**

```bash
sudo apt install libwebkit2gtk-4.1-0 libgtk-3-0 ffmpeg
sudo dpkg -i fanamby_0.1.0_amd64.deb
```

---

## Lancement de l’application

4. Cliquez sur le menu "Windows" et recherchez **Fanamby**. L’application devrait apparaître dans la liste des résultats. Cliquez dessus pour la lancer.

---

## Utilisation

5. Une fois l’interface affichée :

* Cliquez sur **Workspace** (bouton bleu "Folder") pour sélectionner le dossier contenant votre fichier vidéo.
* Cliquez ensuite sur le sélecteur de fichiers pour choisir la vidéo à analyser.
  *Note : le chargement de la vidéo peut prendre entre 2 et 10 secondes.*

6. La vidéo devrait s’afficher dans l’interface. Cliquez sur le bouton lecture pour commencer la lecture.

7. Pour démarrer une analyse :

* Pour faire apparaître la fenêtre de saisie des informations d’extrait, vous pouvez soit :

  * taper deux fois sur le pavé tactile de la souris,
  * soit cliquer directement sur pause dans le lecteur vidéo.

---

## Informations complémentaires

* Les extraits vidéo seront enregistrés dans un sous-dossier nommé `fanamby-{date du jour}` situé dans le même répertoire que la vidéo originale.
* Le nom des extraits suit le format : `joueur_[indicateur]_hh:mm:ss.mp4`