# TP2_Injection_des_dependances

1- Partie 1:

Dans cette partie en a fait l'injection des dépendance utilisant le framework spring :

Tout d'abord on a crée des insterfaces avec leur implémentations .
Apres on a crée le fichier de configaration XML:
![image](https://user-images.githubusercontent.com/102295113/162547998-297aa771-158b-43fc-ba5a-ef10b1eb2b14.png)

- Apres l'execution de ce code on obtient le resultat suivant:

![image](https://user-images.githubusercontent.com/102295113/162549639-15fb0eaa-c07c-4c0a-8a04-bed734552f81.png)

- Pour appelé l'implémentation du la version du base de donnees il suffit de remplace la classe ext.DaoImplVWS par la classe dao.DaoImpl dans le fichier applicationContext.xml et on obtient le resultat suivant:

![image](https://user-images.githubusercontent.com/102295113/162549593-1b1ee040-377e-4ee9-bad0-b3689131c6a9.png)

- Pour appelé l'implémentation du la version de capteur il suffit de remplace la classe dao.DaoImpl par la classe dao.DaoImp2 dans le fichier applicationContext.xml et on obtient le resultat suivant:

![image](https://user-images.githubusercontent.com/102295113/162550501-9c84f1e3-a936-40a9-8303-9b381014c39a.png)


2- Partie 2:
Dans cette partie en a fait l'injection des dépendance utilisant spring Annotation :

![image](https://user-images.githubusercontent.com/102295113/162550473-da3c95f9-2cc9-4ae8-b1a4-b0e983e9f064.png)

-  Apres l'execution de ce code on obtient le resultat suivant:

![image](https://user-images.githubusercontent.com/102295113/162548214-bcf2334d-8b58-4704-b398-b9178cf312e3.png)

Puis , on ajoute la notion Qualifier dans le fichier IMetier.java qui prmmet d'injecter l'istance qu'on veut:
-Pour injecté l'istance dao:

![image](https://user-images.githubusercontent.com/102295113/162550168-4b20fa48-8a2d-4a52-bad4-37907b411cd1.png)

-Pour injecté l'istance dao2 il suffit tout simplement de remplacer dao par dao2:

![image](https://user-images.githubusercontent.com/102295113/162550248-edbec471-7b81-4d77-85b4-99707b122715.png)

Et finalement , on a fait l'injection par constructeur :

![image](https://user-images.githubusercontent.com/102295113/162550591-1ffb90e4-6e6b-4f55-b5d2-26137a615b8c.png)

Apres l'execution de ce code on obtient le resultat suivant: 
![image](https://user-images.githubusercontent.com/102295113/162550635-ae3276a6-577d-43b8-84f7-05c69b747a97.png)





