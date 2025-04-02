
# 🌟 Cours Python : 

Les variables sont des éléments fondamentaux en programmation. Elles permettent de stocker des
valeurs que l'on peut réutiliser ou manipuler.

## 1. Déclaration de variables

On peut nommer les variables comme on le souhaite tant qu'on respecte certaines règles (pas d'espaces, pas de mots-clés réservés, etc.). Par exemple :
ma_variable = 12     
azazdzee= "zerfez fzee"


```python
# Exemple de déclaration de variables
nom = "Alice"        # String (str)
age = 25             #  Entier (int)
taille = 1.68        #  Décimal (float)
est_etudiant = True  # Booléen (bool)
```

### ✨ Manipuler les chaînes de caractères (strings)

On peut concaténer des chaînes de caractères avec le symbole + :

```python
mot = "Alice" + "poulet"
print(mot)  # Affiche : Alicepoulet
```

on peut aussi prendre une lettre ou un partie du mot 
les chiffres qui se trouvent entre crochet se refere aux indice soit 0,1,2,3....

```python
mot = "Alice"
prems_lettre = mot[0]          # Premier caractère : "A"
partie_1_du_mot = mot[:2]      # Du début au 2e caractère : "Al"
partie_2_du_mot = mot[2:]      # Du 3e caractère à la fin : "ice"
partie_precise_du_mot = mot[2:4]  # Entre le 3e et 4e caractères : "ic"

print(prems_lettre)            # Affiche : A
print(partie_1_du_mot, partie_2_du_mot, partie_precise_du_mot)
# Affiche : Al ice ic

```
💡 Astuce : Avec print, on peut afficher plusieurs éléments en les séparant par des virgules. Ces derniers seront automatiquement séparés par un espace lors de l'affichage.


On peut aussi "additionner" des morceaux extraits de chaînes :
```python

print(partie_1_du_mot + partie_2_du_mot + partie_precise_du_mot)
# Affiche : Aliceic

```
### 🔢 Manipuler les nombres (int, float)

maintant que les string sont fait 
on peut passer aux int 
c'est plutot simple il ya addition soustraction division et multiplication

* ( + ) pour additioner 
* ( - ) pour soustraire
* ( * ) pour multiplier 
* ( / ) pour diviser 

 

#### 1 Addition :
```python
chiffre = 10
resultat = chiffre + 5
print(resultat)  # Affiche : 15
```

#### 1 Soustraction  :
```python
chiffre = 10
resultat = chiffre - 3
print(resultat)  # Affiche : 7
```
#### 1 Multiplication  :
```python
chiffre = 5
resultat = chiffre * 4
print(resultat)  # Affiche : 20

```
#### 1 Division  :
```python
chiffre = 20
resultat = chiffre / 4
print(resultat)  # Affiche : 5.0
```
💡 Remarque : La division en Python retourne toujours un nombre décimal (float), même si le résultat semble "entier".

#### Combinaison d'opérations
```python
chiffre = 10
resultat = (chiffre + 5) * 2 - 10 / 5
print(resultat)  # Affiche : 27.0

```

(Bonus hors chiffre ) tu peux aussi multiplier des strings entre eux par exemple

```python
mot= "bonjour"
mot= mot*3
print(mot) # affiche bonjourbonjourbonjour
```

# 🌟 Comprendre l'opérateur == et les Booléens

L'opérateur == permet de vérifier si deux valeurs sont égales. Il retourne un booléen, c'est-à-dire une valeur de type True (vrai) ou False (faux).

## ✨ Exemple de base avec ==

```python
a = 5
b = 3

# Comparer deux valeurs
resultat = (a == b)
print(resultat)  # Affiche : False (car 5 n'est pas égal à 3)

c = 5
print(a == c)  # Affiche : True (car 5 est égal à 5)

```
## ⚡ Utilisation pratique
#### Vérifier une condition
Vous pouvez utiliser == pour tester une condition et exécuter du code en fonction du résultat :

```python
mot_de_passe = "python123"
entree_utilisateur = "python123"

if mot_de_passe == entree_utilisateur:
    print("Mot de passe correct ! ✅")
else:
    print("Mot de passe incorrect ! ❌")

```
#### Comparer différents types
Le == fonctionne avec tous les types de données compatibles :

```python
print(10 == 10)          # Affiche : True
print(10 == "10")        # Affiche : False (car int ≠ string)
print("Bonjour" == "bonjour")  # Affiche : False (sensible à la casse)

```

#### Comparer des variables booléennes
Vous pouvez également comparer des booléens entre eux :

```python
est_ouvert = True
est_ferme = False

print(est_ouvert == est_ferme)  # Affiche : False
print(est_ouvert == True)       # Affiche : True

```

## ❓ Différence entre = et ==

* = : Sert à attribuer une valeur à une variable.
```python
x = 5
```
* == : Sert à vérifier si deux valeurs sont égales.
```python
print(x == 5)  # Vérifie si x est égal à 5, retourne True
```

# 🔄 La boucle for
La boucle for est utilisée pour parcourir une séquence (comme une liste, une chaîne, ou un range).

### Syntaxe de base :

```python
for variable in sequence:
    # Instructions à exécuter
```
### Exemple 1 : Parcourir une liste
```python
fruits = ["pomme", "banane", "cerise"]
for element in fruits:
    print(element)  # Affiche chaque fruit
```

### Exemple 2 : Utiliser range()
```python
for i in range(5):
    print(i)  # Affiche : 0, 1, 2, 3, 4
```
💡 Astuce : range(start, stop, step) permet de définir un point de départ (start), un point d'arrêt (stop, exclusif), et un pas (step)

```python
for i in range(2, 10, 2):
    print(i)  # Affiche : 2, 4, 6, 8 , en effet on affiche les nombres de 2 à 10 avec un decalage de 2 
```

# 🔁 La boucle while

### Syntaxe de base :

```python
while condition:
    # Instructions à exécuter
```
### Exemple 1 : Compteur simple
```python
compteur = 0
while compteur < 5:
    print(compteur)
    compteur += 1  # Incrémentation (comme compteur = compteur +1)
# Affiche : 0, 1, 2, 3, 4
```

# 🚌 LES LISTES 
Une liste est une collection ordonnée et modifiable d'éléments.

### Création

```python
ma_liste = [1, 2, 3, 4]
```
### Accès aux éléments (comme les strings vu précédements)

```python
# Accéder au premier élément
print(ma_liste[0])  # 1

# Accéder au dernier élément
print(ma_liste[-1])  # 4

```
### Ajouter des éléments

```python
ma_liste.append(5)  # Ajoute 5 à la fin , la liste devient [1, 2, 3, 4, 5]
```

### Modifier des éléments

```python
ma_liste[0] = 10  # Change le premier élément en 10 , la liste devient [10, 2, 3, 4, 5]

```
### Supprimer des éléments
```python
ma_liste.pop(1)  # Supprime l'élément à l'indice 1 (ici 2)
print(ma_liste)  # [10, 3, 4, 5]

```
### Longueur de la liste
```python
len(ma_liste)  # Retourne la longueur de la liste ,dans ce cas si 5 element ( [10, 2, 3, 4, 5] )
```

### Prendre par partie 

```python
# Obtenir une sous-liste
sous_liste = ma_liste[1:3]  # [3, 4]
```

# 🤖 Les Fonctions en Python

Une fonction est un bloc de code qui peut être réutilisé pour accomplir une tâche spécifique. Elle prend des entrées, exécute des instructions et peut retourner un résultat.

### Définir une fonction

La syntaxe de base pour définir une fonction en Python est :

```python
def nom_de_la_fonction(param1, param2):
    # Code à exécuter
    return resultat
```
### Exemple 
```python
def addition(a, b):
    return a + b

# Appel de la fonction
resultat = addition(3, 5)
print(resultat)  # 8

```

### Fonctions sans retour (rivet utilise un autre nom mais j'ai oublié )

Une fonction peut ne pas retourner de valeur

```python
def afficher_message():
    print("Message affiché!")

afficher_message()  # Message affiché!


```

# 🗂️ Les Dictionnaires en Python

Un dictionnaire est une structure de données super pratique en Python ! Contrairement aux listes qui utilisent des indices numériques, les dictionnaires stockent des données sous forme de paires **clé-valeur**. C’est comme un vrai dictionnaire : tu cherches un mot (la clé) et tu trouves sa définition (la valeur).

### Création d’un dictionnaire

On utilise des accolades `{}` pour créer un dictionnaire, avec des paires `clé: valeur` séparées par des virgules.

```python
mon_dico = {"nom": "Alice", "age": 25, "ville": "Paris"}
```
Ici :
    "nom", "age", "ville" sont les clés.
    "Alice", 25, "Paris" sont les valeurs

### Accéder aux éléments
Pour récupérer une valeur, on utilise la clé entre crochets [] :

```python
print(mon_dico["nom"])  # Affiche : Alice
print(mon_dico["age"])  # Affiche : 25
```

### Ajouter ou modifier des éléments
Les dictionnaires sont modifiables ! Pour ajouter ou mettre à jour une paire clé-valeur, il suffit d’assigner une valeur à une clé :

```python
mon_dico["pays"] = "France"  # Ajoute une nouvelle paire (si la clé "pays" n'existe pas alors il va automatiquement en creer une dcp)
mon_dico["age"] = 26         # Met à jour la valeur de "age"
print(mon_dico)  # Affiche : {"nom": "Alice", "age": 26, "ville": "Paris", "pays": "France"}
```

### Supprimer des éléments
Pour supprimer une paire clé-valeur, on peut utiliser .pop() ou del :

```python
mon_dico.pop("ville")  # Supprime la clé "ville" et sa valeur
print(mon_dico)  # Affiche : {"nom": "Alice", "age": 26, "pays": "France"}

del mon_dico["pays"]  # Une autre façon de supprimer
print(mon_dico)  # Affiche : {"nom": "Alice", "age": 26}
```
### Parcourir un dictionnaire
On peut utiliser une boucle for pour explorer un dictionnaire. :

```python
for cle in mon_dico:
    print(cle)  # Affiche : nom, age
```
### Longueur d’un dictionnaire
Comme pour les listes, on utilise len() pour connaître le nombre de paires clé-valeur :

```python
print(len(mon_dico))  # Affiche : 2 (car il reste "nom" et "age")
```

## Exemple pratique : Gestion d’un inventaire
Imaginons qu’on gère un petit magasin :
```python
inventaire = {"pommes": 10, "bananes": 5, "oranges": 8}

# Ajouter un produit
inventaire["poires"] = 3

# Mettre à jour le stock
inventaire["pommes"] -= 2  # Vendre 2 pommes

# Afficher l’inventaire
for produit, quantite in inventaire.items():
    print(f"{produit} : {quantite} en stock")
# Affiche :
# pommes : 8 en stock
# bananes : 5 en stock
# oranges : 8 en stock
# poires : 3 en stock
```
# FINIIIIIISS 🥳🥳
