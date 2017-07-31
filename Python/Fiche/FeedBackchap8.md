
## Exercice à choix multiple : La caractère .

    Quelle chaine ne matche pas l'expression régulière '^[A-Z].*\.$' ?
Votre choix : 

L'euro est nettement inférieur à la livre : Très  bien  ! Cette regex correpond au chaine qui commence par une majuscule et qui te termine par un point.
Autres cas : Regarde bien ces 2 parties ^ [A-Z] et '\.$'. 


## Exercice à choix multiple : Autoriser plusieurs caractères

    Quelle est la bonne syntaxe pour savoir si la chaine L contient un "ou" ou un "oi" ou un "on" ou un "om" ?
Votre choix : 

re.search(^ [o][inmu],ch) : Bravo, on recherche bien une chaine qui commence par un o suivi d'un 'i' ou 'n' ou 'm' ou 'u'
Autres cas : La résponse ce trouve dans les []

## Exercice à choix multiple : Les listes standards
    Quelle chaine matche l'expression régulière '^[A-Z]|[0-9]$' ?
Votre choix : 

je fait le 12 : Je vois que tu as l'oeil ! La regex match les chaines commencant par une majuscule OU finisant par un chiffre.
Autres cas : Regarde bien il y a un OU au millieu.
