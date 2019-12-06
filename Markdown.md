je suis un texte ecrit en **Markdown**



Titre de niveau 1
=================
Traduction en HTML : 

	<h1>Titre de niveau 1</h1>

Ceci est un paagraphe de texte.

Ceci est un autre paragraphe de texte.

Titre de niveau 2
-----------------
Traduction en HTML : 

	<h2>Titre de niveau 2</h2>

Mon paragraphe.
Lignejuste en-dessous



Il existe aussi une autre syntaxe pour les titres qui vous permet même de faire des titres de niveau 3 (et 4, et plus si affinités) :

# Titre de niveau 1

## Titre de niveau 2

### Titre de niveau 3



A. Emphase faible (italique)
----------------------------

Voici un mot *important* à mon sens
Voici un mot _important_ à mon sens

Dans les deux cas, la Traduction en HTML : sera le suivant :

	<p>Voici un mot <em>important</em> à mon sens</p>


B. Emphase forte (gras)
-------------------------

Voici des mots **très importants**, j'insiste !
Voici des mots __très importants__, j'insiste !

Dans les deux cas, la Traduction en HTML : sera le suivant :

	<p>Voici des mots <strong>très importants</strong>, j'insiste !</p>




1.Les listes
=============
Créer des listes en Markdown est un vrai bonheur, vous allez voir qu'il n'y a rien de plus simple ! Comme vous le savez sûrement, il existe deux types de listes : les listes à puces et les listes numérotées.


1.1.Les listes à puces
-----------------------
* Une puce
* Une autre puce
* Et encore une autre puce !

Vous pouvez remplacer les étoiles par des tirets ou des signes « + », cela aura exactement le même effet !


Résultat en HTML :

	<ul>
		<li>Une puce</li>
		<li>Une autre puce</li>
		<li>Et encore une autre puce !</li>
	</ul>


Notez que vous pouvez imbriquer les listes à puces :

* Une puce
* Une autre puce
    * Une sous-puce
    * Une autre sous-puce
* Et encore une autre puce !

* Et encore une autre puce !


1.2.Les listes à puces numérotées
----------------------------------
Pour créer une liste numérotée, c'est très intuitif : il suffit de commencer les puces par des numéros !

1. Et de un
2. Et de deux
3. Et de trois

Résultat en HTML :

	<ol>
		<li>Une puce</li>
		<li>Une autre puce</li>
		<li>Et encore une autre puce !</li>
	</ol>


2.Les citations
================
Les citations fonctionnent comme les réponses des e-mails : vous devez précéder les lignes citées d'un chevron «> »!

> Ceci est un texte cité. Vous pouvez répondre
> à cette citation en écrivant un paragraphe
> normal juste en-dessous !

Résultat en HTML :
<blockquote><p>Ceci est un texte cité. Vous pouvez répondre à cette citation en écrivant un paragraphe normal juste en-dessous !</p></blockquote>

Sachez que vous pouvez imbriquer des citations et du Markdown à l'intérieur des citations !

> Une citation
>
> > Une réponse à la citation
> >
> > Réponse qui contient une liste à puces :
> >
> > * Puce
> > * Autre puce



3.Codes source
===============

Pour insérer un code source, il suffit de l'indenter, c'est-à-dire de le faire précéder de 4 espaces ou d'une tabulation :

Voici un code en C :

    int main()
    {
        printf("Hello world!\n");
        return 0;
    }


Résultat en HTML :

	<p>Voici un code en C :</p>

	<pre><code>int main()
	{
	    printf("Hello world!\n");
	    return 0;
	}
	</code></pre>



Code en ligne
---------------
Si vous voulez écrire un morceau de code au milieu d'un paragraphe, entourez-le d'accents graves comme ceci : \` Exemple :

La fonction `printf()` permet d'afficher du texte

Résultat  en HTML: 

	<p>La fonction <code>printf()</code> permet d'afficher du texte</p>



4.Les liens
============

Pour créer un lien, vous devez placer le texte du lien entre crochets suivis de l'URL entre parenthèses :

Rendez-vous sur le [Site du Zéro](http://www.siteduzero.com) pour tout apprendre à partir de Zéro !

Résultat  en HTML: 

Rendez-vous sur le `<a href="http://www.siteduzero.com">Site du Zéro</a>` pour tout apprendre à partir de Zéro !


5.Les images
============

Les images s'insèrent de la même façon que les liens. Vous devez simplement mettre un point d'exclamation devant les premiers crochets :

![Zozor](http://uploads.siteduzero.com/files/420001_421000/420263.png)


Le texte entre crochets est le texte alternatif de l'image (je vous invite à le renseigner à chaque fois pour ceux qui ne peuvent pas voir les images). 

Résultat en HTML:


6.Barre de séparation
=====================

Faire une barre de séparation en Markdown ? Rien de plus intuitif !

-------------------------

Vous pouvez aussi remplacer les tirets par des étoiles. Leur nombre importe peu (il faut au moins en mettre quelques-uns !).


Résultat en HTML: 

	<hr />
	
	
7.Les tableaux 	
===============
Je vais mettre un compplement sur les tableaux avec Markdown.
Vous aller voir avec markdown tout est intuitif...

Lorsqu'on doit rediger unrapport en utilisant du markdown, il y a toujours des formulaires ou des tableaux dont nous devons faire. J’utilise normalement l’éditeur Markdown pour écrire de petits livres (des petits ebooks).

Voici deux façons d'écrire des formulaires de démarques en markdown.

7.1. Méthode Minimalisme
-------------------------
			Name  |price|Nbr  
			-|-|-
			Banana| $1 | 5 |
			Apple | $1 | 6 |
			Mango | $1 | 7 |



Visuellement on verra ceci : 

Name  |price|Nbr  
-|-|-
Banana| $1 | 5 |
Apple | $1 | 6 |
Mango | $1 | 7 |

7.2. Méthode Simple
--------------------

			Name | 111 | 222 | 333 | 444
			   - | :-: | :-: | :-: | -:
			 aaa | bbb | ccc | ddd | eee| 
			 fff | ggg | hhh | iii | 000|
			 
Visuellement on verra ceci : 

name | 111 | 222 | 333 | 444
   - | :-: | :-: | :-: | -:
 aaa | bbb | ccc | ddd | eee| 
 fff | ggg | hhh | iii | 000|

7.3. Méthode Native
--------------------
				name | 111 | 222 | 333 | 444
				:-: | :-: | :-: | :-: | :-:
				aaa | bbb | ccc | ddd | eee | 
				fff | ggg | hhh | iii | 000 |
				
Visuellement on verra ceci : 

name | 111 | 222 | 333 | 444
:-: | :-: | :-: | :-: | :-:
aaa | bbb | ccc | ddd | eee| 
fff | ggg | hhh | iii | 000|

7.4. La différence entre differentes méthodes
----------------------------------------------
Bien que la méthode simple soit légèrement plus simple, les première et dernière colonnes ne sont pas centrées car il n'y a pas de format avant et après, ce qui est assez fastidieux pour la méthode minimaliste. Les méthodes minimalistes sont simples, mais elles sont toutes alignées à gauche. Le format natif est plus beau.

Opinion personnelle : Les patients atteints de TOC doivent utiliser la méthode native, d’autres, n’hésitez pas à utiliser ce qui vous plait.


7.5. Description de la syntaxe
-------------------------------

1) Les espaces supplémentaires entre "|" ,"-"  et ":" seront ignorés sans affecter la mise en page.
2) La barre de titre par défaut est alignée au centre et le contenu est aligné à gauche.
3)" -: " indique que le contenu et la barre de titre sont alignés à droite, " :- " indique que le contenu et la barre de titre sont alignés à gauche, et " :-: " indique que le contenu et la barre de titre sont alignés au centre.
4) Les espaces supplémentaires entre le contenu et " | " sont ignorés. Le premier " | " et le dernier " | " de chaque ligne peuvent être omis et il doit y avoir au moins un des " - ".



--> Ressources pour aller plus loin
====================================
Vous venez d'avoir une bonne vue d'ensemble du Markdown et vous connaissez maintenant les principales possibilités offertes par ce petit langage étonnant. :) Sachez que nous n'avons pas couvert ici toutes les possibilités. On peut :

  * Faire une table des matières de liens (liens par références) en pied de page ;

  * Ajouter des infobulles aux liens et aux images ;

  * Créer des tableaux (uniquement dans certaines implémentations de Markdown) ;

  * etc.


Vous trouverez toutes les informations concernant le langage sur :

  * [Le site officiel de Markdown](https://daringfireball.net/projects/markdown/syntax)
  * [Cette traduction en français](https://michelf.ca/projets/php-markdown/syntaxe/) 




Et si ce que je veux faire n'est pas possible en Markdown ? 

Écrivez simplement du HTML dans ce cas ! En effet, vous pouvez sans problème mixer du Markdown et du HTML quand vous le souhaitez :

	Ce texte comprend du *Markdown* mais aussi du <abbr title="HyperText Markup Language">HTML</abbr> !

