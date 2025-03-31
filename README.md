# Projet ASM : Implémentation de str_to_word_array

## Objectif
Le but de ce projet est d'implémenter une fonction `str_to_word_array` en langage assembleur. Cette fonction prend une chaîne de caractères (`char*`) et la transforme en un tableau de chaînes de caractères (`char**`) en utilisant des séparateurs spécifiques.

## Spécifications

### Prototype de la fonction
Voici le prototype pour tester votre fonction à l'aide d'un fichier C.
```c
char **str_to_word_array(char *str);
```

### Description
La fonction doit découper la chaîne d'entrée en "mots" selon les séparateurs suivants :
* Espace (' ')
* Tabulation ('\t')
* Saut de ligne ('\n')

### Comportement attendu
1. La fonction doit analyser la chaîne d'entrée et compter le nombre de mots.
2. Elle doit allouer dynamiquement un tableau de pointeurs de taille suffisante pour contenir tous les mots plus un pointeur NULL final.
3. Elle doit copier chaque mot dans un espace mémoire alloué dynamiquement.
4. Les séparateurs consécutifs doivent être traités comme un seul séparateur.
5. La fonction doit renvoyer un pointeur vers le tableau de pointeurs (tableau de mots).
6. Le dernier élément du tableau retourné doit être NULL pour marquer la fin du tableau.

### Exemple
```
Entrée: "Hello  world\tASM\nproject" 
Sortie: ["Hello", "world", "ASM", "project", NULL]
```
