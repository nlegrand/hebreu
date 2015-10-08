Hebreu
======

Je suis en train d'apprendre l'hébreu, ce projet me permet de générer
un livret de révision, avec vocabulaire, grammaire etc. Il va évoluer
au fur et à mesure de mon apprentissage.

Le contenu n'intéresse sans doute que moi, cela dit les méthodes
utilisées pour imprimer un livret de droite à gauche à l'aide de
XeLaTeX et psutils peut servire d'exemples à d'autres.

Dépendances
===========

- Make
- XeLaTeX, with geometry, fontspec, bidi packages
- psutils
- ConTeXt (only for pstopdf utility)
- croscore fonts
- la fonte Trashim CLM

Sur Debian, `apt-get install texlive-full psutils fonts-croscore`
devrait être suffisant. Bon, il faut aussi installer [Trashim
CLM](http://culmus.sourceforge.net/fancy/).

Utilisation
===========

Créer le livret `livret.pdf` :

    make

Tout nettoyer

    make clean

Ensuite il faut imprimer `livret.pdf` avec l'option recto-verso :
short edge (flip).