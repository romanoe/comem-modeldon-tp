# Modélisation de Données · environnement de TP

Environnement de travail du cours **Modélisation de Données** (HEIG-VD / COMEM+) : VS Code, SQLite et l'extension Database Client, déjà installés. Les slides du cours sont sur [comem-modeldon.onrender.com](https://comem-modeldon.onrender.com).

Aucune connaissance de Git n'est nécessaire.

---

## Ouvrir l'environnement

### Dans le navigateur (Codespaces)

1. Se connecter à GitHub
2. Ouvrir [codespaces.new/romanoe/comem-modeldon-tp](https://codespaces.new/romanoe/comem-modeldon-tp)
3. Cliquer sur **Create codespace**, attendre une à deux minutes

### Sur sa machine (Docker)

1. Installer l'extension VS Code **Dev Containers** (`ms-vscode-remote.remote-containers`)
2. Télécharger ce dépôt : bouton **Code**, puis **Download ZIP**, et le décompresser
3. Ouvrir le dossier dans VS Code
4. Cliquer sur **Reopen in Container** dans la notification

### Vérifier

Dans le terminal de VS Code :

```bash
sqlite3 --version
```

---

## Travailler sur un exercice

1. Télécharger le fichier `.sql` depuis le lien donné sur les slides
2. Le glisser dans l'explorateur de VS Code
3. Exécuter le script dans le terminal :

```bash
sqlite3 bibliotheque.db
sqlite> .read bibliotheque.sql
sqlite> .tables
sqlite> .quit
```

4. Ouvrir le panneau **Database** de la barre latérale, cliquer sur **+**, choisir **SQLite** et sélectionner le fichier `.db` pour voir les tables

---

## Garder son travail

Les fichiers créés restent dans l'environnement, pas sur GitHub.

- **Codespaces** : un codespace inactif est supprimé après 30 jours. Télécharger ses fichiers en fin de séance : clic droit, **Download**.
- **Docker** : les fichiers sont dans le dossier décompressé, sur la machine.
