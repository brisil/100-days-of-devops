🚀 Day 4/100 – Linux Processes

Aujourd’hui, j’ai appris comment fonctionnent les processus en Linux ⚙️

👉 Un processus = un programme en cours d’exécution

Exemple :
Quand tu ouvres un terminal, un processus est lancé.

---

📌 1. Voir les processus

* Afficher les processus :
  ps

* Version détaillée :
  ps aux

👉 Tu verras :

* USER → utilisateur
* PID → identifiant du processus
* %CPU → utilisation CPU
* %MEM → mémoire utilisée

---

📌 2. Processus en temps réel

* Surveiller en direct :
  top

👉 Très utile pour voir ce qui consomme des ressources

---

📌 3. Gérer les processus

* Tuer un processus :
  kill PID

* Forcer l’arrêt :
  kill -9 PID

⚠️ Attention :
kill -9 = arrêt brutal (à éviter si possible)

---

📌 4. Trouver un processus

* Rechercher un processus :
  ps aux | grep nom_du_processus

---

📌 5. Pourquoi c’est important en DevOps ?

👉 Pour :

* Identifier un programme qui plante
* Surveiller les performances
* Libérer des ressources

💡 Exemple réel :
Si un serveur est lent → vérifier avec `top`

---

🧪 Mini exercices

1. Afficher tous les processus :
   ps aux

2. Lancer un processus :
   sleep 1000

3. Trouver ce processus :
   ps aux | grep sleep

4. Tuer le processus :
   kill PID

5. Vérifier qu’il est arrêté

---

⚠️ Important

* Toujours vérifier avant de tuer un processus
* Ne pas tuer un processus système critique

---

💡 Ce que j’ai compris

Les processus permettent de comprendre ce que fait le système en temps réel.
C’est essentiel pour diagnostiquer un problème.

---

👉 Question

Quelle commande utiliseriez-vous pour voir la consommation CPU en temps réel ? 👀

#100DaysOfDevOps #Linux #DevOps
