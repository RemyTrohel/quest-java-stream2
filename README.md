# **Challenge**
## **Fichage des agents**
Ta mission précédente (et surtout les donuts offerts à la dernière réunion) t'ont rendu populaire au *S.H.I.E.L.D*... Mais pas assez pour t'éviter les basses besognes qui reviennent à un bleu tel que toi !

L'accueil est muni d'un système de reconnaissance vocale, qui permet à chaque agent de s'identifier. Le système reconnaît les noms et prénoms des agents, puis les stockent dans une chaîne de caractères.

Cependant, la base de données des agents enregistre ces derniers dans des instances de type `Agent`, qui possèdent des attributs `firstName` et `lastName`.

Ta mission est de transformer les chaînes de caractères fournies en instances d'`Agent`.

Pour démarrer, [fais un *Fork* du dépôt suivant](https://github.com/WildCodeSchool/quest-java-stream2) puis clone-le en local.

> Pense bien à faire un *Fork*, sinon tu ne pourras rien pousser !

1. Ouvre les classes `Shield` et `Agent` afin d'en étudier les contenus respectifs
2. Dans `Shield.java`, utilise un `Stream` et la méthode `map` pour transformer une liste de `String` en liste d'`Agent`
3. Utilise une `Function`, dans laquelle tu pourras appeler la méthode `split` sur la chaîne de caractère afin d'en extraire de nom et le prénom : utilise ces derniers pour créer une instance d'`Agent` et la retourner
4. Ensuite utilise une lambda
5. Tu ne dois pas modifier la classe `Agent` !
6. Compile et exécute le code, afin de vérifier que les deux listes s'affichent bien dans le terminal

Résultat attendu lors de l'exécution de `Shield` :

```
Agents:
Coulson Phil
May Melinda
Johnson Daisy
Fitz Leopold
Simmons Jemma
```
### **Critères de validation**
- Le dépôt *GitHub* contient bien les fichiers `Agent.java` et `Shield.java`. Seul `Shield.java` doit avoir été modifié.
- La classe `Shield` contient bien un `Stream` qui transforme une liste d'`Agent`, en utilisant la méthode `map` et une `Function`
- La classe `Shield` se compile sans erreur et affiche dans le terminal le même résultat que celui présenté précédemment
