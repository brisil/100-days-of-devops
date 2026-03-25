🚀 Day 2/100 – Linux Permissions & Users

Aujourd’hui, j’ai appris un concept ESSENTIEL en Linux : **les permissions** 🔐

👉 Sans ça, impossible de sécuriser un serveur.

---

📌 1. À quoi servent les permissions ?

Les permissions permettent de contrôler :

* Qui peut lire un fichier
* Qui peut le modifier
* Qui peut l’exécuter

💡 Exemple concret :
Un fichier sensible (mot de passe, config) ne doit pas être accessible à tout le monde.

---

📌 2. Structure des permissions

Exemple :
-rwxr-xr--

👉 Découpage :

* `-` → type (fichier)
* `rwx` → droits du propriétaire (user)
* `r-x` → droits du groupe
* `r--` → droits des autres

---

📌 3. Signification des lettres

* r (read) → lire le fichier
* w (write) → modifier le fichier
* x (execute) → exécuter (script/programme)

---

📌 4. Les 3 niveaux d’utilisateurs

👤 user → propriétaire du fichier
👥 group → groupe d’utilisateurs
🌍 others → tous les autres

---

📌 5. Commandes importantes

* Voir les permissions :
  ls -l

* Modifier les permissions :
  chmod 755 file.txt

* Rendre un fichier exécutable :
  chmod +x script.sh

* Changer le propriétaire :
  chown user:group file.txt

---

📌 6. Comprendre les chiffres (TRÈS IMPORTANT)

Chaque permission a une valeur :

* r = 4
* w = 2
* x = 1

👉 Exemple :
chmod 755 file.txt

=

* 7 (4+2+1) → rwx (user)
* 5 (4+0+1) → r-x (group)
* 5 (4+0+1) → r-x (others)

---

📌 7. Attention à chmod 777 ⚠️

chmod 777 file.txt

👉 Tout le monde peut :

* lire
* modifier
* exécuter

🚨 Risque :
n’importe qui peut casser ton système

👉 À éviter en production !

---

🧪 Mini exercice

1. Créer un fichier :
   touch test.txt

2. Ajouter du contenu :
   echo "Hello DevOps" > test.txt

3. Donner tous les droits :
   chmod 777 test.txt

4. Vérifier :
   ls -l

5. Sécuriser le fichier :
   chmod 600 test.txt

---

💡 Ce que j’ai compris

Les permissions sont la base de la sécurité Linux.
Un mauvais réglage peut rendre un système vulnérable.

---

👉 Question

Quelle permission utiliseriez-vous pour :

* un script ?
* un fichier sensible ? 👀

#100DaysOfDevOps #Linux #DevOps
