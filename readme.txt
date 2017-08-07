=== Plugin Name ===
Contributors: adfever
Donate link: http://www.adfever.com/
Tags: adfever, publicité, advertising, sponsored links, monetization, ads, pub, adfever.com, ad, fever
Requires at least: 3.4
Tested up to: 3.6.1
Stable tag: 0.9.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Plugin de monétisation pour les membres de la régie publicitaire AdFever.

== Description ==

Ce plugin permet aux éditeurs membres de la plateforme publicitaire AdFever - [AdFever.com](http://www.Adfever.com/ "Régie publicitaire AdFever") - d'ajouter simplement des liens sponsorisés sur votre installation de wordpress.

Pour que ce plugin fonctionne, vous devrez posséder un compte éditeur AdFever. Les liens sponsorisés pourront alors être affichés automatiquement avant ou après vos articles. Les annonces affichées dépendent des tags associés à vos posts et du titre de vos posts.

L'interface d'administration du plugin vous permet de personnaliser l'affichage des liens sponsorisés.
Il est également possible d'intégrer manuellement les liens sponsorisés dans votre thème et de définir la présentation des annonces via des styles CSS.

== Installation ==

1. Uploadez le dossier 'adfever-monetisation' dans le répertoire '/wp-content/plugins/'
2. Activez le plugin via la page 'Extensions' de votre interface d'administration
3. Configurez le plugin via la page 'AdFever Monétisation' de votre interface d'administration
4. Renseignez votre AID et SID AdFever
5. Personnalisez l'affichage des annonces

Si vous désirez intégrer manuellement les annonces à votre thème wordpress, vous devrez insérer le code suivant à l'intérieur de la "Loop" de wordpress.
`<?php if function_exists(AF_theme_callback) {AF_theme_callback(get_the_ID());}; ?>`


== Frequently Asked Questions ==

= Où récupérer mon AID et/ou SID AdFever =

Pour récupérer vos identifiants, connectez-vous à votre espace éditeur sur [AdFever.com](http://www.Adfever.com/ "Régie publicitaire AdFever") puis rendez-vous dans la rubrique Inventaire.

= Les annonces ne s'affichent pas =

* Vérifiez que vous avez bien renseigné votre AID et SID dans la page de configuration du plugin.
* Vérifiez que le fichier header.php de votre thème contienne bien la ligne `<?php wp_head(); ?>`.
* Essayez d'ajouter des tags plus génériques à votre article.

== Screenshots ==

1. Page de configuration du plugin

== Changelog ==

= 0.9.3 =
* Version stable du plugin