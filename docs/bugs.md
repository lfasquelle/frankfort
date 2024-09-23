# Quelques erreurs à connaître



Lorsque vous faîtes certaines erreurs (par exemple des erreurs de syntaxe), 
Python peut parfois les détecter et  envoie dans ce cas un message correspondant à l'erreur.

!!! note 
    Parfois une erreur en engendre une autre et le message renvoyé demande un temps de réflexion...
    
    
    
Vous **devez** reconnaître les erreurs les plus classiques et savoir les corriger.
   
   
   
    
## division by zero

```
>>> mot = ''
>>> 3/len(mot)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: division by zero
```

Cette erreur `division by zero` est facile à comprendre. Bien sûr, elle est rarement aussi directe que dans le 
code précédent. En général, il s'agit d'une division par une variable et cette variable a pris la valeur 0... Il
faut alors repérer dans son code à quel moment cette variable prend la valeur 0 et corriger...


## is not callable



```
>>> mot = 'coucou'
>>> mot(2)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'str' object is not callable
```


L'erreur `is not callable` peut se traduire par *n'est pas appelable*. Une fonction peut être  appelée (f étant le nom
d'une fonction, un code tel que `f(2)` qui calcule f(2) effectue un *appel* à la fonction) et en classe de première NSI, 
ce sera les seuls objets python appelables.

Si on suppose que le codeur voulait accèder à l'élément d'indice 2 de la chaîne 'coucou', 
l'erreur faite ici est d'avoir utilisé  des parenthèses au lieu de crochets, c'est à dire d'avoir 
écrit `mot(2)` au lieu de `mot[2]`.


## out of range


```
>>> mot = 'coucou'
>>> mot[6]
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
IndexError: string index out of range
```

`out of range` se traduit par *hors de portée* ou *en-dehors de la plage* (ou *en-dehors de la fourchette* ...).
Cette erreur se produit en général  quand vous cherchez à accèder à un élément d'indice n'existant pas.  
Dans l'exemple, les indices vont de 0 à 5: il n'y a pas d'élément ayant pour indice 6 dans la chaîne 'coucou'.



## IndentationError

Une erreur d'indentation a lieu à chaque fois que vous délimitez mal vos blocs d'instructions.

Exemple:

```python
s = 0
p = 1
for i in range(10):
    s = s + i
      p = p*i
```

Le décalage pour l'instruction `p = p*i`  n'a aucun "sens" ici...
