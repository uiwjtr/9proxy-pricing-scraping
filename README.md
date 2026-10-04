# 9proxy avis: prix actuels, retour des utilisateurs et quel forfait choisir pour le scraping, le multi-comptes et la vérification d'annonces

Tapez « 9proxy avis » et vous tombez sur deux camps qui ne se parlent pas. D'un côté, des annuaires de proxys qui affichent une note autour de 3,9/5 et des chiffres de performance. De l'autre, une page Trustpilot francophone classée « Bas », autour de 2/5, où l'on raconte des IP qui tombent au bout d'une heure.

Les deux existent. Ce qui manque souvent, c'est la seule question utile avant de sortir sa carte bancaire: est-ce que ce modèle de facturation correspond à ce que je vais réellement en faire? Parce que 9Proxy ne vend pas un abonnement mensuel classique. Il vend des IP résidentielles à l'unité, ou des gigaoctets. Et selon le cas, ça change tout.

## Ce que 9Proxy vend réellement

9Proxy est un fournisseur de proxys résidentiels uniquement. Pas de datacenter, pas de mobile, pas de proxy ISP au catalogue: la société ne vend qu'un seul type de ressource, mais sous deux modèles de facturation distincts.

Le réseau est annoncé à plus de 20 millions d'IP résidentielles dans plus de 90 pays, avec 8 000+ serveurs et un uptime revendiqué de 99,95 %. Ce chiffre de 20 millions revient le plus souvent dans les évaluations tiers, mais il faut le prendre avec des pincettes: certaines pages promotionnelles annoncent 95 millions d'IP, d'anciens annuaires en listent encore 8 ou 9 millions. Le pool a visiblement grossi après un rapprochement avec BeeProxy, et les sources ne se sont jamais alignées depuis. Pour la France, les volumes publiés par zone citent environ 490 000 IP, ce qui place le pays dans le haut du panier européen.

Côté technique, le service couvre HTTP, HTTPS et SOCKS5, avec un ciblage descendant jusqu'au pays, à l'État, à la ville, au code postal et au FAI. Les sessions peuvent être collantes (la même IP tenue sur plusieurs requêtes) ou rotatives.

L'accès se fait par plusieurs canaux:

- l'application Windows, qui route le trafic au niveau de l'OS via une redirection de ports — utile pour les logiciels qui ne gèrent pas nativement les proxys;
- Proxy2Web, un outil dans le navigateur sans installation, authentification par identifiant/mot de passe;
- l'API publique, documentée, pour générer des listes de proxys, gérer les sous-utilisateurs et suivre la consommation;
- ProxyHub, orienté gestion de flottes sur appareils mobiles.

Le tableau de bord est décrit de façon constante comme propre et lisible, y compris par les utilisateurs mécontents du service. C'est le genre de détail qui n'a l'air de rien mais qui évite de perdre une soirée.

Si vous voulez voir la structure des offres directement dans l'interface, le plus simple reste de créer un compte: 👉 [créer un compte 9Proxy et consulter les forfaits](https://bit.ly/9-Proxy).

## Les avis utilisateurs: où se situe le vrai clivage

La lecture croisée des retours donne une image plus cohérente qu'elle n'en a l'air.

Sur Trustpilot (page francophone), la note globale est basse et le grief est presque toujours le même: des IP qui deviennent inutilisables après une heure, et une politique de remplacement jugée trop courte. Un avis de janvier 2026 décrit exactement ce scénario, avec pour conséquence des alertes de sécurité sur les comptes de l'utilisateur. La réponse de 9Proxy à cet avis est instructive: l'entreprise explique que les IP résidentielles dynamiques appartiennent à de vrais internautes, que leur durée de vie ne peut donc pas être garantie, et conseille de passer à des proxys statiques de type ISP pour les sessions longues. Ce n'est pas une excuse marketing, c'est la mécanique réelle des pools résidentiels — sauf que 9Proxy ne propose justement pas d'offre ISP.

À noter aussi: l'entreprise répond à 100 % de ses avis négatifs, généralement sous un mois.

De l'autre côté, les retours positifs viennent souvent de profils techniques. Une évaluation publiée sur G2 par un architecte sécurité cloud décrit quatre mois d'utilisation pour tester des configurations régionales, avec pour point fort la constance des IP et le fait qu'elles ne soient pas immédiatement signalées. Des commentaires similaires, plus courts, circulent sur Product Hunt et AlternativeTo, avec une mention récurrente: la compatibilité avec les navigateurs anti-détection (Dolphin Anty, AdsPower, ixBrowser, Multilogin).

Les annuaires tiers, eux, se situent entre les deux. ProxyLook attribue 3,9/5 à 9Proxy, avec un taux de succès mesuré à 97 % et une latence P95 d'environ 1,3 seconde — en dessous des 99,5 % et 0,6 s annoncés par l'éditeur, ce qui reste dans le domaine du plausible pour du résidentiel rotatif. Le même annuaire pointe l'absence d'essai gratuit, une politique de remboursement étroite et l'absence d'offres datacenter, ISP ou mobile.

Autrement dit: les avis négatifs ne disent pas « le service est une arnaque ». Ils disent « je l'ai utilisé pour un usage qui ne correspondait pas au produit ». Nuance importante quand on cherche à savoir si 9proxy est fiable.

## La panne de fin juin 2026, et ce qu'elle change pour vous

Un point qui remonte dans plusieurs sources indépendantes: autour du 28 juin 2026, le site de 9Proxy a cessé de répondre, renvoyant des erreurs au niveau de l'hôte derrière Cloudflare, tandis que l'application desktop partait en timeout. Support silencieux, aucune communication technique détaillée, pas d'explication publique de la cause.

Certains évaluateurs ont rapproché l'épisode d'une opération de démantèlement visant un autre réseau de proxys plus tôt dans l'année, mais rien ne permet de confirmer ce lien. Panne matérielle ou autre chose, personne n'a tranché publiquement.

Ce qui est vérifiable, en revanche, c'est la conséquence pratique pour un utilisateur: quand un pipeline de scraping ou une flotte de comptes repose sur un fournisseur unique et que ce fournisseur tombe, tout s'arrête. C'est un argument en faveur du fractionnement des dépendances, pas nécessairement contre 9Proxy en particulier.

## Tarifs 9Proxy: tous les forfaits actuels

Il faut d'abord poser un contexte. Le 18 mai 2026, 9Proxy a annoncé sa première hausse de prix depuis trois ans, effective au 1er juin. Deux familles ont bougé: les forfaits par IP et les packs combinés. Les forfaits au gigaoctet, eux, n'ont pas changé. Les tarifs ci-dessous sont ceux publiés après cette mise à jour.

Aucun de ces forfaits n'est un abonnement: c'est un achat unique, crédité sur un solde. Les IP non utilisées n'expirent pas; la bande passante achetée reste valable 180 jours (validité illimitée sur l'offre Enterprise).

| Type | Forfait | Prix | Prix unitaire | Validité |
| --- | --- | --- | --- | --- |
| Par IP | 100 IP | 24 $ | 0,24 $/IP | IP sans expiration |
| Par IP | 500 IP | 72 $ | 0,144 $/IP | IP sans expiration |
| Par IP | 1 000 IP + 500 offertes | 126 $ | 0,084 $/IP | IP sans expiration |
| Par IP | 2 500 IP | 210 $ | 0,084 $/IP | IP sans expiration |
| Par IP | 5 000 IP | 360 $ | 0,072 $/IP | IP sans expiration |
| Par IP | 15 000 IP | 720 $ | 0,048 $/IP | IP sans expiration |
| Par IP | 25 000 IP | 863 $ | 0,035 $/IP | IP sans expiration |
| Par IP | 50 000 IP | 1 438 $ | 0,029 $/IP | IP sans expiration |
| Par IP (Business) | 100 000 IP | 2 300 $ | 0,023 $/IP | IP sans expiration |
| Par IP (Business) | 200 000 IP | 4 140 $ | 0,021 $/IP | IP sans expiration |
| Par IP (Business) | 500 000 IP | 8 625 $ | 0,018 $/IP | IP sans expiration |
| Au Go | 5 Go | 15 $ | 3,00 $/Go | 180 jours |
| Au Go | 50 Go + 5 offerts | 105 $ | 2,10 $/Go | 180 jours |
| Au Go | 100 Go | 150 $ | 1,50 $/Go | 180 jours |
| Au Go | 200 Go | 200 $ | 1,00 $/Go | 180 jours |
| Au Go | 1 000 Go | 800 $ | 0,80 $/Go | 180 jours |
| Au Go | 2 000 Go | 1 500 $ | 0,75 $/Go | 180 jours |
| Au Go (Enterprise) | 3 000 Go | 2 160 $ | 0,72 $/Go | Illimitée |
| Au Go (Enterprise) | 6 000 Go | 4 200 $ | 0,70 $/Go | Illimitée |
| Au Go (Enterprise) | 10 000 Go | 6 800 $ | 0,68 $/Go | Illimitée |
| Pack combiné | 100 IP + 5 Go (Starter) | 30 $ | — | Go valables 180 jours |
| Pack combiné | 1 500 IP + 50 Go (Popular) | 180 $ | — | Go valables 180 jours |
| Pack combiné | 5 000 IP + 500 Go (Pro) | 720 $ | — | Go valables 180 jours |

👉 [Voir tous les forfaits et les prix appliqués sur votre compte](https://bit.ly/9-Proxy)

Deux remarques sur ce tableau. D'abord, les tarifs « à partir de 0,015 $/IP » qu'on lit encore un peu partout correspondent à l'ancienne grille: le plancher actuel est de 0,018 $/IP, et il faut commander 500 000 IP pour l'atteindre. Ensuite, les gros paliers affichent parfois un prix total légèrement inférieur à l'arrondi du prix unitaire — ce sont les montants facturés qui font foi, pas les colonnes calculées.

## IP ou Go: comment choisir sans se tromper

C'est la seule décision qui compte vraiment ici, et elle dépend d'une question simple: votre charge de travail consomme-t-elle beaucoup de données par IP, ou beaucoup d'IP pour peu de données?

Le forfait par IP donne une bande passante illimitée tant que l'IP est active. Une IP résidentielle tient de quelques heures à environ 24 heures selon l'utilisateur d'origine. C'est le bon choix pour tout ce qui exige de garder la même identité réseau sur la durée: sessions de comptes, paniers e-commerce, plateformes avec détection anti-bot agressive. Contrainte à connaître: ce modèle passe par l'application desktop.

Le forfait au Go fonctionne à l'inverse. On paie le trafic, on génère autant d'endpoints qu'on veut, avec rotation automatique. C'est plus économique quand chaque requête transporte peu de données mais doit sortir d'une IP différente: surveillance de SERP, vérification d'annonces, contrôle de prix, polling d'API. Tout se pilote depuis le dashboard, sans application à installer.

Les packs combinés, eux, visent les charges mixtes: une partie du projet a besoin d'IP stables, l'autre de rotation. Le pack 1 500 IP + 50 Go est présenté comme le plus populaire sur le site, ce qui est cohérent avec son positionnement: on passe sous les 0,10 $/IP sans s'engager sur des dizaines de milliers d'unités.

Quelques repères concrets si vous hésitez:

- Tester le service sur une cible réelle: **5 Go à 15 $**, soit 3 $/Go. C'est le ticket d'entrée le moins risqué.
- Faire tourner quelques dizaines de profils de navigateurs anti-détection: **100 IP à 24 $**, bande passante illimitée.
- Alimenter un pipeline de collecte régulier: **50 Go + 5 offerts à 105 $** ou **100 Go à 150 $**.
- Répartir la facture sur plusieurs clients: **Starter (100 IP + 5 Go) à 30 $** par projet.

## Les limites à connaître avant de payer

Certaines contraintes sortent régulièrement dans les retours utilisateurs et dans les analyses tierces. Elles sont factuelles, et elles pèsent plus lourd que n'importe quelle promesse de performance.

**La fenêtre de remplacement de 60 secondes.** Si une IP échoue dans la minute suivant son activation, elle est recréditée. Au-delà, elle est considérée comme consommée. Or, comme le montre l'avis Trustpilot de janvier 2026, les défaillances réelles surviennent souvent plus tard. C'est le principal point de friction du produit.

**Pas d'essai gratuit affiché.** Aucune page publique ne propose d'essai. L'équipe de 9Proxy indique sur ses canaux communautaires proposer ponctuellement un essai limité aux nouveaux utilisateurs, selon les disponibilités, et des pages tierces évoquent 5 à 10 IP de test — mais rien d'officiel ni de garanti. Conséquence: prévoyez de valider la qualité des IP sur vos propres cibles avec le plus petit pack possible.

**Pas de remboursement en argent.** Les conditions publiées parlent de crédit, pas de restitution. Si votre usage ne colle pas, la sortie est étroite.

**Streaming non supporté sur les offres par IP.** La politique d'usage a évolué et 9Proxy indique ne plus prendre en charge la lecture de contenus en streaming (YouTube notamment) sur les forfaits par IP. Plusieurs vieux articles francophones vantent encore 9Proxy pour débloquer du contenu géo-restreint: c'est obsolète.

**Résidentiel uniquement.** Les proxys statiques ISP, les datacenter et les mobile ne font pas partie du catalogue. Une ligne datacenter est annoncée comme « bientôt disponible », mais rien n'est commercialisé à ce jour.

**Les chiffres de performance sont éditeur.** 99,5 % de réussite, 0,6 s de temps de réponse, 99,95 % d'uptime: ce sont des données publiées par 9Proxy. Les mesures indépendantes disponibles sont plus basses (autour de 97 % de réussite, P95 à 1,3 s). Correct, mais pas identique.

Un point positif mérite d'être cité au passage: la « Today List ». Les proxys utilisés dans les 24 dernières heures peuvent être réutilisés sans frais supplémentaires. Sur des phases de test ou des sessions qui se terminent plus tôt que prévu, ça évite de brûler du crédit inutilement.

## S'inscrire et lancer ses premiers proxys

Le parcours est court. Créez un compte via 👉 [l'inscription 9Proxy](https://bit.ly/9-Proxy), confirmez l'e-mail, choisissez un mode de facturation, puis générez vos identifiants. Pas de processus KYC long qui bloque l'accès, contrairement à certains acteurs orientés grands comptes.

Ensuite:

1. Choisissez votre authentification: identifiant/mot de passe (avec des sous-utilisateurs si plusieurs personnes ou scripts partagent le solde) ou liste blanche d'IP, qui supprime les mots de passe.
2. Sélectionnez le pays, l'État ou la ville. Sur les offres au Go, le code postal et le FAI sont également disponibles.
3. Définissez le mode de session: rotatif (nouvelle IP à chaque requête) ou sticky (même IP pendant X minutes).
4. Exportez les endpoints en .txt ou .csv, ou récupérez directement les exemples de code fournis.

Les moyens de paiement sont larges: cartes bancaires, Apple Pay, Google Pay, Alipay, et cryptomonnaies via un processeur dédié (BTC, ETH, LTC, TRX, USDT en TRC20 et ERC20, DOGE, DAI, BCH). Payer en crypto ajoute automatiquement 5 % d'IP bonus — un détail qui compte si vous prévoyez de gros volumes.

Dernier réflexe avant de monter en charge: testez 100 à 500 requêtes sur votre cible réelle. Les taux de réussite varient beaucoup selon le site visé, et c'est le seul moyen de savoir si le pool tient face à votre anti-bot.

## Questions fréquentes

**9Proxy est-il fiable?**
Le service fonctionne et a des utilisateurs actifs depuis 2021. Ce qui est documenté, ce n'est pas une fraude, mais deux fragilités: une politique de remplacement très courte et une panne de service notable fin juin 2026. Traitez-le comme un fournisseur à tester avant de lui confier une production critique.

**Existe-t-il un essai gratuit?**
Aucun essai n'est affiché publiquement. L'équipe mentionne un essai limité selon disponibilité, sans garantie publique. Le vrai test à faible risque, c'est le pack 5 Go à 15 $.

**Combien coûte l'entrée de gamme?**
**15 $** pour 5 Go, ou **24 $** pour 100 IP avec bande passante illimitée.

**Les crédits expirent-ils?**
Les IP non utilisées n'expirent pas. La bande passante achetée est valable 180 jours, sauf sur l'offre Enterprise où la validité est illimitée.

## Verdict

9Proxy n'est ni le désastre décrit sur Trustpilot, ni le fournisseur miracle des pages de comparaison. C'est un spécialiste du résidentiel avec un modèle de facturation qui a un avantage réel — la bande passante illimitée par IP, à des tarifs unitaires que peu d'acteurs atteignent — et des contreparties tout aussi réelles: pas d'essai gratuit, remplacement limité à 60 secondes, pas d'offre ISP ou datacenter, et un historique de performance qui repose largement sur des chiffres maison.

Il convient bien si vous gérez des sessions de comptes, du multi-profils ou de la collecte de données avec des volumes de trafic difficiles à prévoir, et si vous acceptez de valider la qualité du pool sur vos propres cibles avant d'augmenter les volumes. Il convient mal si vous cherchez des IP figées pour des sessions de plusieurs jours, du streaming, ou une production où un remboursement en argent est indispensable en cas de problème.

Dans le doute, commencez petit, mesurez, puis décidez: 👉 [ouvrir un compte 9Proxy et choisir un forfait](https://bit.ly/9-Proxy).
