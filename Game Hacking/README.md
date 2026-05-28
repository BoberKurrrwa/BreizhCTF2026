# Game Hacking 
Étant novice dans le monde des CTF, c'était la première fois que je rencontrais une catégorie Game Hacking. Je n'avais alors pas compris par quel moyen on devait trouver les flags, c'est pour cela que j'ai tenté de jouer au jeu de façon "normale".

> [!CAUTION]
> J'explique ici tout mon raisonnement, donc pour ceux qui veulent juste voir ce que j'ai fait au final, regardez simplement les vidéos !

## Welcome to Happy's adventures [1/5] (Difficulté : Very Easy)

Pour le Flag n°1, il suffisait de lancer le jeu et de se rendre sur l'ordinateur dans la première salle (chose que je n'ai pas faite à la première tentative puisque j'ai intéragit directement avec le canapé, me faisant alors entrer dans une cinématique qui nous amène dans la salle suivante...).


## A way out [2/5] (Difficulté : Easy)


Pour le Flag n°2, une fois arriver dans notre salle, il fallait récupérer des barettes de RAM sur une table afin de les lancer sur une cible. 

Le but était de réussir à lancer 2 barettes en moins de 2 secondes afin d'ouvrir une porte, or il y avait un délai de 5 secondes entre chaque lancé.

Ne comprenant pas comment il fallait faire, j'ai tenté par tout moyen de lancer plus vite les barettes (la lancer depuis le plus loin possible de la salle, puis courir en me rapprochant de la cible afin de lancer une barette une fois contre la cible (cela me faisait gagner jusqu'à 2 secondes)).

Ne trouvant pas comment activer la porte, j'ai commencé à chercher des moyens détourné dans le jeu pour passer au niveau suivant. Après une longue recherche, j'ai découvert que la zone de collision de la table me permettait de monter dessus dans les coins, puis avec une grande précision, je pouvais sauter sur la zone de collision des barettes de RAM que l'on a du récupérer précédemment. Une fois ceci réaliser, j'ai tenté de sauter directement sur morceau de mur qui dépassait légèrement, mais hélas cela m'était impossible.
J'ai ensuite pu observer qu'un léger morceau de mur dépassait à un autre endroit et j'ai tenté de sauter dessus. J'ai vu qu'il me retenait légèrement avant de me laisser tomber, alors j'ai tenté avec un nouvel angle, en allant le plus loin possible et c'était enfin bon.
Il ne me restait plus qu'à sauter par dessus le mur (après avoir tenté de sauter sur le toit à côté de moi mais qui était en fait non-solide...) et j'ai pu accéder à la 2e partie de la salle, puis à la porte menant à la salle suivante.

<video src="src/flag_2.mp4" controls alt="Flag n°2"></video>

## Kill them all [3/5] (Difficulté : Medium)

Pour le flag n°3, des ennemies invisibles apparaissent dans la salle et on doit les tuer. 

Le problème est que comme je ne sais toujours pas comment m'y prendre (😅), j'ai tenté de parcourir la salle afin de voir si je rentrais en collision avec les zones de collision des personnages invisibles, or je n'ai jamais pu en trouver. 

En allant vers la porte qui mène à la suite du niveau, j'ai vu que je pouvais intéragir avec cette dernière en me tenant sur son côté, et donc passer directement à la salle suivante.

<video src="src/flag_3.mp4" controls alt="Flag n°3"></video>

## Rush B no stop [4/5] (Difficulté : Easy)

J'arrive alors dans la salle du flag n°4. Dans ce niveau, il nous est possible de ramasser une trousse de soin sur un cadavre, mais lorque l'on fait cela, un drone se met à nous pourchasser et nous tirer dessus. Il nous faut alors nous enfuir au travers d'un champ par un petit chemin. 

Malheureusement ce chemin contient des plantes qui nous font des dégâts. Le problème est que dès que l'on prend 2 dégats, on meurt. Dès que l'on sort du chemin, on meurt également.

Le principe serait donc de dupliquer la trousse de soin en trifouillant les données du jeu, or j'ai opté pour une autre option (unintended).

Pour cette option, j'ai découvert que le drône tirait des munitions qui ne nous faisait pas de dégâts, et qui se mettait à gravité autour de nous. Lorsque de nombreuses munitions s'accumulent autour de moi, il arrive par moment que ces dernières me propulsent en l'air. Dans ce cas, il faut en profiter pour passer par dessus les plantes. 

J'ai donc joué avec le moteur de collision du jeu plusieurs fois afin d'atteindre la fin du niveau et obtenir le flag au moment d'atteindre la porte vers la salle n°5.

<video src="src/flag_4.mp4" controls alt="Flag n°4"></video>

## A way back home [5/5] (Difficulté : Hard)

Flag n°5, cette fois-ci il fallait aller tout en haut du phare dans lequel on venait tout juste de rentrer, malheureusement il m'était impossible de faire quoi que ce soit depuis le jeu directement. J'ai pourtant tenté de [bunny hop](https://fr.wikipedia.org/wiki/Bunny_hopping) :

![](https://media.tenor.com/nLSPDXcShSUAAAAM/bhop-bomb.gif)

Que ce soit en avant ou en arrière, rien ne fonctionnait. 

J'ai donc décidé d'arrêter là sans pouvoir finir le jeu 😔🥺.
