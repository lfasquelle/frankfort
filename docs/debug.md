# Débuguer



## Qu'est ce qu'un bug?



!!! note 
    Extrait de [wikipedia](https://fr.wikipedia.org/wiki/Bug_(informatique))
    
    En informatique, un bug (insecte en anglais) ou bogue (au Québec et en France) 
    est un défaut de conception d'un programme informatique à l'origine d'un dysfonctionnement.

    La gravité du dysfonctionnement peut aller de bénigne, 
    causant par exemple des défauts d'affichage mineurs, à majeure, 
    tels un crash système pouvant entraîner de graves accidents, 
    par exemple la destruction en vol de la première fusée Ariane 5, en 1996.

    Un bug peut résider dans une application, 
    dans les logiciels tiers utilisés par cette application, 
    voire dans le firmware d'un composant matériel 
    comme ce fut le cas du bug de la division du Pentium. 
     
     
Un bug, c'est essentiellement un défaut de programmation.

En apprenant à programmer, vous commettrez deux types de bugs:

+ l'erreur de syntaxe: non respect de la syntaxe du langage, oubli d'une indentation, oubli d'un paramètre
dans une fonction... 
Dans ce cas, votre programme ne s'exécute même pas. Toute erreur de ce type devra être corrigée, que ce soit durant
les séances d'exercices ou pour un travail en-dehors du temps de classe. Pour un devoir à rendre, la présence
d'une telle erreur entraîne la note minimale.
+ l'erreur de logique: le programme ne fait pas tout à fait ce qui est attendu, vous avez oublié un ou des 
cas... Il faut également autant que possible éliminer ce genre d'erreurs. 


## Corriger un bug de syntaxe

Les outils pour corriger un tel bug:

+ Relire le cours.
+ Consulter la documentation python en ligne ou en local (fonction help...)
+ Utiliser les f-strings et la fonction print pour afficher les résultats intermédiaires et comprendre à
quel moment une variable n'est pas du type attendu.
+ On peut également utiliser le site [python tutor](http://pythontutor.com/visualize.html#mode=edit) qui permet
de visualiser l'état des variables au fur et à mesure du déroulement, ce qui facilite le repèrage de la source 
du bug. 
+ L'affichage des états des variables peut aussi être obtenu avec les bons éditeurs dédiés 
([spyder par exemple](https://docs.spyder-ide.org/variableexplorer.html)).



## Corriger un bug de logique



+ Toujours anticiper en prévoyant un jeu de tests de  vos fonctions, c'est à dire des exemples de paramètres
et du résultat qui doit être obtenu. Penser toujours aux cas extrêmes: par exemple, pour une fonction concernant
les chaînes de caractères, que se passe-t-il pour la chaîne vide?
+  Utiliser les f-strings et la fonction print pour afficher les résultats intermédiaires et comprendre à
quel moment une variable n'a plus la valeur espérée.
+ Afficher l'état des variables avec les outils proposés par un bon IDE ou pythontutor par exemple.
+ &Eacute;crire une fonction de tests.
+ Utiliser les outils de debug d'un bon IDE ([par exemple spyder](https://docs.spyder-ide.org/debugging.html)).


 
