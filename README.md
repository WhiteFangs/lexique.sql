# Lexique SQL
[Lexique 3](http://www.lexique.org/) est une base de données qui fournit pour 135000 mots du français de nombreuses informations linguistiques. 
Elle est présentée ici au format SQL, plus adaptée que le format texte pour une utilisation avec des requêtes.

## Informations

La liste des informations disponibles dans la base est détaillée dans la [documentation de Lexique 3](http://www.lexique.org/outils/Manuel_Lexique.htm#_Toc152122354).
Les tables comprennent, outre les mots, les lemmes, les fréquences, le genre, le nombre, la catégorie grammaticale, 
et de nombreuses représentations orthographiques, phonémiques et syllabiques, etc.

## Format

La base de données Lexique 3 est disponible sur le site officiel aux [formats texte et Excel](http://www.lexique.org/telLexique.php).
En revanche, ces formats ne sont pas très pratiques pour des applications web qui reposent sur des requêtes, 
j'ai donc trouvé la même base réenregistrée au format [SQLite](https://gist.github.com/WhiteFangs/9556b513b7fc18f9ac4cc72527407ae5), 
et pour mes besoins personnels je l'ai réadapté pour une utilisation dans ma base MySQL, donc au format SQL classique. 

## Exemples d'utilisation

L'application ["Si à la Saint-Valentin on te tient la main…"](http://louphole.com/applications/saint-valentin/) sur mon site
repose uniquement sur Lexique 3 en faisant des inférences de rimes en fonction de la fin du nom donné.

Lexique 3 est également la base de données sur laquelle repose la base de données de rimes [Drime](https://drime.a3nm.net/) crée par [Antoine Amarilli (a3nm)](https://a3nm.net/index.html.fr), 
utilisée dans plusieurs de mes applications.

Le programme [Fréquences des mots](http://louphole.com/bibliotech/frequence-des-mots/) est une implémentation naïve et brutale de requêtes des mots d'un texte sur la base Lexique
pour obtenir leurs fréquences. 
