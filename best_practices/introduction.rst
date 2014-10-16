.. index::
   single: Les bonnes pratiques du framework Symfony

Les bonnes pratiques du framework Symfony
=========================================

Le framework Symfony est bien connu pour être *réellement* flexible et utilisé
pour construire des micro-site, des applications d'entreprise permettant de tenir
des milliard de connexions et être la base d'autres frameworks. Depuis qu'il est
sorti en juillet 2011, la communauté a appris énormément sur ce qui est possible
et comment faire les choses *de la meilleure manière*.

Les ressources de la communauté - comme les blogs ou les présentations - ont créées
un ensemble de recommandations non-officielles pour développer des applications 
Symfony. Malheureusement, un certain nombre de ces recommandations ne sont pas 
nécessaires pour les applications web. La plupart du temps, elles compliquent
inutilement les choses et ne suivent pas la philosophie pragmatique de Symfony.

Qu'apporte ce guide ?
---------------------

Ce guide entends définir ceci en décrivant les **bonnes pratiques officielles
permettant de développer des applications web avec le framework Symfony**. Elles
sont les bonnes pratiques qui collent à la philosophie du framework telle 
qu'imaginée par le créateur original `Fabien Potencier`_.

.. note::

    **Bonnes pratiques** est une expression désignant *"un ensemble de procédures 
    définies qui permettent de produire des résultats optimums"*. Et c'est exactement
    ce que ce guide entend procurer. Sauf si vous n'êtes pas d'accord avec 
    l'ensemble des recommandations, nous pensons qu'elles peuvent vous aider 
    à construire de grosses application avec moins de complexité.

Ce guide est *particulièrement adapté* pour :

* Les sites internet et les applications web développés avec le framework Symfony.

Pour les autres cas, ce guide devrait être un bon **point de départ** que vous 
pouvez ensuite **amender et adapter à vos besoins**:

* Bundles partagés avec la comunauté Symfony;
* Développeurs avancés ou équipe créant leurs propres standarts;
* Quelques applications complexe ayant des pré-requis fortement personnalisés;
* Bundles devant être partagés en interne dans une entreprise.

Nous savons que les vieilles habitudes ont la vie dure et que certains d'entre
vous seront choqués par certaines de ces bonnes pratiques. Mais en suivant 
celles-ci vous serez capable de développer des applications rapides, en 
retirant de la complexité et avec le même niveau ou plus de qualité. C'est
également un objet mouvant qui continuera à s'améliorer.

Gardez en tête que ce sont des **recommandations facultatives** que vous
et votre équipe pouvait ou ne pouvait pas suivre pour développer des 
applications Symfony. Si vous souhaitez continuer à suivre vos propres
bonnes pratiques et méthodologies, vous pouvez bien entendu faire cela.
Symfony est assez flexible pour s'adapter à vos besoins. Cela ne changera
jamais.

À qui s'adresse ce livre (Indice : ce n'est pas un tutoriel)
------------------------------------------------------------

Chaque développeur Symfony, que vous soyez expert ou novice, peut lire ce
guide. Mais, comme ce n'est pas un tutoriel, quelques connaissances de base
sur Symfony sont requises pour pouvoir tout comprendre. Si vous êtes totalement
novice avec Symfony, bienvenu ! Commencez par le premier tutoriel `The Quick Tour`_.

Nous avons volontairement garder ce guide court. Nous ne voulons par répéter des
explications que vous pouvez trouver dans la vaste documentation de Symfony, 
comme les discussions autour de l'injection de dépendance ou des ///front controllers///.
Nous allons uniquement mettre l'accent sur l'explication de la façon de faire de
ce que vous connaissez déjà.

The Application
---------------

In addition to this guide, you'll find a sample application developed with
all these best practices in mind. **The application is a simple blog engine**,
because that will allow us to focus on the Symfony concepts and features without
getting buried in difficult details.

Instead of developing the application step by step in this guide, you'll find
selected snippets of code through the chapters. Please refer to the last chapter
of this guide to find more details about this application and the instructions
to install it.

Don't Update Your Existing Applications
---------------------------------------

After reading this handbook, some of you may be considering refactoring your
existing Symfony applications. Our recommendation is sound and clear: **you
should not refactor your existing applications to comply with these best
practices**. The reasons for not doing it are various:

* Your existing applications are not wrong, they just follow another set of
  guidelines;
* A full codebase refactorization is prone to introduce errors in your
  applications;
* The amount of work spent on this could be better dedicated to improving
  your tests or adding features that provide real value to the end users.

.. _`Fabien Potencier`: https://connect.sensiolabs.com/profile/fabpot
.. _`The Quick Tour`: http://symfony.com/doc/current/quick_tour/the_big_picture.html
.. _`The Official Symfony Book`: http://symfony.com/doc/current/book/index.html
.. _`The Symfony Cookbook`: http://symfony.com/doc/current/cookbook/index.html
.. _`github.com/.../...`: http://github.com/.../...
