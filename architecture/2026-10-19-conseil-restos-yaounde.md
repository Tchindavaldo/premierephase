# Conseil LLM : vendre des sites web aux restos de Yaoundé

- **Date :** 2026-10-19
- **Outil :** skill `llm-council` (installé dans `.claude/skills/llm-council/`)
- **Déroulé :** 5 conseillers en parallèle, puis 1 relecture anonyme groupée (au lieu de 5 relectures, pour économiser le quota), puis la synthèse du président

## Avis des conseillers (résumé)
- **Contradicteur :** solution sans problème. Les restos sans site ont fait un choix rationnel, Maps/OSM est incomplet, les budgets sont faibles (30–80 k), des outils gratuits existent déjà (WhatsApp Business, Google Business, Facebook), et rien n'a été validé.
- **Premiers principes :** mauvaise question. Le resto veut des commandes, pas un site. Le filtre « pas de site » ne trie rien : il faut viser ceux qui reçoivent déjà beaucoup de demandes. Proposer un abonnement plutôt qu'une vente unique.
- **Expansionniste :** le vrai produit est la commande directe WhatsApp + MoMo, sans commission (Glovo prend 20–30 %). Une plateforme multi-restos, un annuaire, puis d'autres villes et d'autres commerces.
- **Œil extérieur :** « site » ne veut rien dire pour un patron de maquis. Lui montrer *son propre* menu en ligne. Un prix simple : 25 k + 5 k/mois.
- **Exécutant :** menu digital + commande WhatsApp + QR code. Prix : 25–40 k + 5 k/mois, 100–150 k pour le haut de gamme. Une liste faite à la main, des visites sur place. Objectif : 20 visites → 3 clients.

## Relecture anonyme
- Réponse la plus forte : l'**Exécutant**, la seule qu'on peut lancer tout de suite, avec un seuil d'abandon.
- Plus gros angle mort : l'**Expansionniste**. Glovo apporte des clients et des livreurs, pas seulement une commission.
- Ce que tous ont raté : **le trafic** (qui amène les clients vers le lien ?), **la livraison**, **l'encaissement mensuel** (impayés), **la concurrence locale**, **la charge de maintenance pour une personne seule**.

## Verdict du président
**Points d'accord :** ne pas vendre « un site ». Vendre un **menu digital avec commande WhatsApp**, un QR code et un lien en bio, payable en MoMo, avec un abonnement mensuel. Valider sur le terrain avant de coder ou de lancer un scraping.

**Désaccords :** l'ambition (petit service rentable ou plateforme SaaS) et le ciblage (petits maquis ou restos déjà très demandés).

**Recommandation :**
1. Offre : **« Votre menu en ligne + commandes sur WhatsApp »**. 25 000 FCFA d'installation + 5 000 FCFA/mois (mises à jour comprises). Formule premium à 100–150 k pour le haut de gamme.
2. Un seul modèle réutilisable, pour pouvoir maintenir 50 restos seul.
3. Inclure dans l'abonnement la **fiche Google Maps corrigée** et un **kit de promotion** (QR codes de table, visuel pour les statuts WhatsApp), pour régler le problème du trafic.
4. Paiement d'avance en MoMo. Si l'abonnement n'est pas payé, le lien est suspendu (à annoncer dès le départ).
5. Cibler en premier les restos qui ont **déjà une activité Facebook/Instagram** et qui ne sont pas sur Glovo.
6. L'idée d'une plateforme ou d'un annuaire seulement **après 20 clients payants**.

**Première action :** faire **3 démos réelles** (avec le vrai menu, tiré de leur Facebook) pour 3 restos de ton quartier, puis aller les leur montrer sur ton téléphone entre 15 h et 17 h.
