
## Exercice à choix multiple : Mode ouverture 4
    Avec l'ouverture ci-dessous, dans quel mode est ouvert le fichier ?
    open('fichier.txt')
    
    Votre choix : 
 Read : Correct ! Si le mode n'est pas spécifié, par défaut le fichier est ouvert en lecture.
 Autres : Le fichier a un mode d'ouverture par défaut, celui qui ne changera rien à son contenu !
 
 
## Exercice à choix multiple : Lien fichier
    Quelle est la méthode pour écrire dans un fichier ?
    
    Votre choix : 
 
 write: Bravo, ne l'oubli pas. Cette méthode te seras très utile dans le future !
 print : Print permet d'afficher une variable, tu devrais retourné a la leçon 1
 echo : Il existe un moyen d'utilisé des commande système mais cette commande affiche ce qu'il a en argument
 append : Ne confond pas, l'argument 'a' de la methode open et la méthode write. 
 read : On veut écrire, pas lire =D
 
## Exercice à choix multiple : Exception
    Quel est le type d'erreur levé si `fichier.txt` n'existe pas ?
    try:
        fichier = open('fichier.txt')
    Except ???:
        exit(1)
        
    Votre choix : 
    
FileNotFoundEror :   Correct ! Essayez par exemple de code avec un fichier inexistant : try : fichierIn=open("toto.txt",'r') except Exception as e : print(type(e)) sys.exit()

Autres cas : Si on t'envoie sur un site qui n'existe pas, ton navigateur va te dire ?