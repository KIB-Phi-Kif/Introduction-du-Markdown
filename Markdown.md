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

