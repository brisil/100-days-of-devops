🚀 Day 3/100 – Linux File System

Aujourd’hui, j’ai appris comment Linux organise ses fichiers 📂

👉 Tout dans Linux est structuré sous forme d’arborescence (comme un arbre).

---

📌 1. Le point de départ : `/`

👉 `/` (root) est la racine du système
Tous les fichiers et dossiers partent de là

---

📌 2. Les dossiers les plus importants

* `/home` → dossiers des utilisateurs
* `/etc` → fichiers de configuration (très important ⚙️)
* `/var` → logs et données qui changent souvent
* `/tmp` → fichiers temporaires
* `/bin` → commandes essentielles
* `/root` → dossier personnel de l’utilisateur root

💡 Exemple concret :
Les logs système sont souvent dans `/var/log`

---

📌 3. Navigation dans le système

Commandes utilisées :

* Se déplacer :
  cd /
  cd /home
  cd ..

* Voir les fichiers :
  ls
  ls -l

* Voir où on est :
  pwd

---

📌 4. Pourquoi c’est important en DevOps ?

👉 Pour :

* Trouver les logs rapidement
* Modifier des fichiers de configuration
* Debug un serveur

💡 Exemple :
Si une app plante → vérifier `/var/log`

---

🧪 Mini exercices

1. Aller à la racine :
   cd /

2. Explorer `/etc` :
   ls /etc

3. Aller dans les logs :
   cd /var/log
   ls

4. Lire un fichier de log :
   cat syslog

5. Revenir dans ton dossier personnel :
   cd ~

---

⚠️ Important

* Ne pas modifier `/etc` sans comprendre
* `/tmp` est souvent vidé automatiquement

---

💡 Ce que j’ai compris

Linux est organisé de manière logique.
Comprendre la structure permet de mieux gérer et dépanner un système.

---

👉 Question

Si ton application ne fonctionne plus,
dans quel dossier irais-tu chercher les logs ? 

#100DaysOfDevOps #Linux #DevOps
