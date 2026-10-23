# 📒 Mon carnet de bord

**Nom MAVIOGA:** 

**Prénom KEMI :** 

**Adresse de mon site :** https:/kmavioga3.pythonanywhere.com

> Modifiez ce fichier directement sur GitHub (icône crayon ✏️) pour répondre aux questions de chaque exercice.
> Écrivez avec vos propres mots : une réponse courte et juste vaut mieux qu'un long copier-coller ! 🙂

---

## 🟢 Exercice 1 — Mon premier déploiement

1. Où se trouve physiquement le code qui fabrique votre page : sur votre ordinateur, sur GitHub ou sur PythonAnywhere ?

   > _Ma réponse :Sur GitHub.

2. Pourquoi votre voisin(e) peut-il voir votre site, alors que vous n'avez rien installé sur son ordinateur ?

   > _Ma réponse :Grâce à PythonAnywhere qui héberge le site en ligne.

---

## 🟢 Exercice 2 — Les URL et les routes

1. Dans l'URL `https://www.google.com/maps`, quel est le nom de domaine ? Quel est le chemin ?

   > _Ma réponse :Grâce à PythonAnywhere qui héberge le site en ligne.

2. Que veut dire le message *Not Found* ? Qui l'a envoyé : votre navigateur ou le serveur ?

   > _Ma réponse :Le serveur l'a envoyé pour dire que la page n'existe pas.

3. Que se passe-t-il si deux fonctions portent le même nom dans `flask_app.py` ? (Indice : essayez, puis lisez l'Error log.)

   > _Ma réponse :Cela crée un bug ou une erreur.

---

## 🔵 Exercice 3 — Le langage HTML

1. Quelle est la différence entre ce que le serveur **envoie** et ce que le navigateur **affiche** ?

   > _Ma réponse :Le serveur envoie du code brut ; le navigateur affiche une page visuelle.

2. À quoi servent les balises `<h1>`, `<p>`, `<ul>` et `<li>` ?

   > _Ma réponse :<h1> = grand titre, <p> = paragraphe, <ul>/<li> = listes.

3. Pourquoi l'image s'affiche-t-elle alors qu'elle n'est pas sur votre serveur ?

   > _Ma réponse :L'attribut src pointe vers un lien externe.

---

## 🔵 Exercice 4 — Les templates

1. Pourquoi est-ce une bonne idée de séparer le code Python et le HTML ? (Pensez à une équipe avec un développeur et un graphiste.)

   > _Ma réponse :Pour séparer la logique (Python) du design (HTML).

2. Les `{{ prenom }}` sont-ils remplacés par le serveur ou par le navigateur ? Comment l'avez-vous vérifié ?

   > Par le serveur. On le voit dans le code source du navigateur.

---

## 🔵 Exercice 5 — Le CSS et les liens

1. Quelle est la différence de rôle entre le HTML et le CSS ?

   > _Ma réponse :HTML = structure ; CSS = design.

2. Pour afficher votre page `/presentation`, combien de fichiers le navigateur doit-il télécharger ? (Vous pourrez le vérifier à l'exercice suivant !)

   > _Ma réponse :Au moins deux (HTML et CSS).

3. Pourquoi faut-il parfois faire **Ctrl + F5** pour voir les changements de CSS ?

   > _Ma réponse :Pour vider le cache du navigateur.

---

## 🟣 Exercice 6 — Espionner le navigateur

1. Que signifie HTTP ? Qui envoie la **requête** et qui envoie la **réponse** ?

   > _Ma réponse :HyperText Transfer Protocol. Le client (navigateur) demande, le serveur répond.

2. Combien de requêtes votre page `/presentation` a-t-elle déclenchées ? Lesquelles ?

   > _Ma réponse :Deux ou trois (HTML, CSS, favicon).

3. Que signifie le code `200` ? Et le code `404` de la favicon ?

   > _Ma réponse :200 = succès ; 404 = non trouvé.

4. Pourquoi les modifications faites dans l'onglet Éléments ne sont-elles pas visibles par les autres visiteurs ?

   > _Ma réponse :Car c'est uniquement stocké dans la mémoire locale de votre navigateur.

---

## 🟣 Exercice 7 — Envoyer des informations dans l'URL

1. Dans l'URL `https://www.youtube.com/results?search_query=chat`, quel est le nom du paramètre ? Quelle est sa valeur ?

   > _Ma réponse :Paramètre : search_query / Valeur : chat.

2. Pourquoi le serveur plante-t-il avec `a=bonjour` ? Que faudrait-il faire pour l'éviter ?

   > _Ma réponse :Le code s'attend à un nombre et reçoit du texte. Il faut valider les données.

3. Pourquoi est-il dangereux d'afficher **tel quel** ce que l'utilisateur envoie ?

   > _Ma réponse :Risque d'injection de code malveillant (faille XSS).

---

## 🟣 Exercice 8 — Les formulaires

1. Quelle est la différence visible entre GET et POST ?

   > _Ma réponse :GET affiche les données dans l'URL ; POST les cache.

2. Pour un formulaire de **recherche**, quelle méthode choisiriez-vous ? Et pour un formulaire de **connexion avec mot de passe** ? Pourquoi ?

   > _Ma réponse :Recherche = GET (partageable) ; Connexion = POST (sécurisé).
3. Les données envoyées en POST sont-elles vraiment « secrètes » ? (Pensez à ce que vous avez vu dans l'onglet Réseau.)

   > _Ma réponse :Non, elles sont lisibles en clair dans l'onglet Réseau (sans HTTPS).

---

## 🔴 Exercice 9 — Les codes de statut

1. Quelle est la différence entre une erreur `4xx` et une erreur `5xx` ? Qui est « fautif » dans chaque cas ?

   > _Ma réponse :4xx = faute du client ; 5xx = faute du serveur.

2. Comment fonctionne une redirection ? Qui fait la deuxième requête : le serveur ou le navigateur ?

   > _Ma réponse :Le serveur répond avec une redirection, et c'est le navigateur qui fait la deuxième requête.

3. Donnez un exemple de situation où un vrai site utilise une redirection.

   > _Ma réponse :Rediriger google.com vers [https://www.google.com](https://www.google.com).

---

## 🔴 Exercice 10 — Ce que le serveur sait de vous

1. Citez trois informations que le serveur connaît sur vous, sans que vous ayez rien rempli.

   > _Ma réponse :Adresse IP, type de navigateur, langue préférée.

2. À quoi peut servir l'en-tête `Accept-Language` pour un site comme Wikipédia ?

   > _Ma réponse :Afficher directement le site dans la bonne langue.

3. Dans l'Access log, retrouvez une requête qui a reçu un code `404`. Quelle page était demandée ?

   > _Ma réponse :/favicon.ico (ou une autre page inexistante).

4. Après cet exercice, que pensez-vous de la notion de « navigation anonyme » ?

   > _Ma réponse :Elle est très relative (l'adresse IP reste visible par le serveur).
---

## 🔴 Exercice 11 — Le Web des machines : API et JSON

1. Quelle est la différence entre une page HTML et une réponse JSON ? À qui chacune est-elle destinée ?

   > _Ma réponse :HTML = pour les humains ; JSON = pour les machines.

2. Dans la page `/horloge`, quel code s'exécute sur le **serveur** et quel code s'exécute dans le **navigateur** ?

   > _Ma réponse :Python s'exécute sur le serveur ; JavaScript s'exécute dans le navigateur.

3. Citez une application de votre téléphone qui, selon vous, utilise une API. Quelles données échange-t-elle ?

   > _Ma réponse :Une app météo (échange de données GPS contre des températures).
---

## 🏁 Pour conclure

En quelques phrases, expliquez à un ami ce qui se passe entre le moment où il tape une adresse dans son navigateur et celui où la page s'affiche :

> _Ma réponse :Tu tapes l'adresse, ton navigateur envoie une requête au serveur, le serveur prépare la page et renvoie le code, puis ton navigateur l'affiche.
