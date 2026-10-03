# Plateformes d'abonnement et de vente directe (Patreon, Substack, Ko-fi, Tipeee, marketplaces)

*Sources consultées le 03/10/2026 : urssaf.fr (liste des revenus artistiques, 31/03/2026), CGI art. 1649 ter A à E, BOI-INT-AEA-30-20231213, impots.gouv (DPI-DAC7, économie collaborative), règlement d'exécution (UE) 282/2011 art. 9 bis, pages d'aide Patreon (accès partiel — voir §4).*

## 1. Ce qu'une plateforme n'est pas

Une plateforme d'abonnement ou de paiement **n'est ni un éditeur, ni un organisme de gestion collective, ni un producteur**. Conséquences :
- **pas de précompte** des cotisations sociales (CSS L. 382-4 : seuls les diffuseurs français précomptent) ;
- **pas de retenue de TVA** (CGI 285 bis) ;
- **pas de déclaration art. 241** aux impôts → les droits ne sont pas « intégralement déclarés par des tiers » → **BNC**, pas traitements et salaires (CGI 93 1 quater).

L'erreur classique — « la plateforme s'occupe des déclarations comme mon éditeur » — est fausse sur les trois points. **Tout est à la charge de l'auteur.**

## 2. Qualification des revenus (côté URSSAF artistes-auteurs)

La liste URSSAF des revenus artistiques principaux inclut : l'**autoédition / autodiffusion** « quel que soit le format, le support ou le nombre d'exemplaires », y compris « par l'intermédiaire de plateformes et marketplaces » ; les **droits d'auteur versés par un diffuseur étranger ou un particulier** ; le **financement participatif** (déclaré net de la commission de la plateforme). Le **blogueur** qui « rédige du contenu et des articles » est cité parmi les activités éligibles.

| Offre sur la plateforme | Qualification | Case de déclaration probable |
|---|---|---|
| Abonnement donnant accès à des **écrits** (essais, analyses, newsletters, chapitres) | revenu artistique principal (autoédition via plateforme / diffuseur étranger) | « Auto-édition, auto-diffusion » ou « Droits d'auteur hors OGC » — **à confirmer** ; brut vs net de commission non tranché pour l'autoédition (net admis pour le financement participatif) |
| Don / pourboire sans contrepartie | financement participatif | net de commission |
| Podcast, vidéo originaux | œuvre audiovisuelle/sonore | idem, branche concernée |
| Accès à un **canal communautaire**, Q&R, « shout-out », appel, commission personnalisée | **service** à la demande d'un utilisateur — ni œuvre, ni accessoire listé | **hors régime** (micro-entreprise) ou zone grise si marginal ; isoler la part |
| Formation en ligne, webinar | prestation de service | hors régime |

**Aucune source officielle ne nomme Patreon ou Substack.** Dire que la qualification est une lecture des textes, et proposer de la faire confirmer (URSSAF par écrit, expert-comptable).

## 3. TVA

- **Fournisseur réputé** : pour les services fournis par voie électronique, la plateforme qui prend part à la fourniture peut être réputée agir en son nom propre (règlement d'exécution (UE) 282/2011, art. 9 bis) et **collecter la TVA auprès des abonnés UE** (c'est ce que fait Patreon). L'auteur fournit alors un service à la plateforme. Deux conséquences à faire trancher : (a) le montant à retenir dans son CA (brut payé par les abonnés ou net reversé) ; (b) la **qualification** de sa propre opération — livraison d'œuvres / cession de droits (10 %, plafond 50 000 €) ou service électronique (20 %, plafond « autres opérations » 35 000 €). Voir [tva.md](tva.md) §7.
- En franchise, l'auteur ne facture pas de TVA ; il surveille simplement le plafond applicable.

## 4. DAC7 — ce que les plateformes transmettent au fisc

- Cadre : directive (UE) 2021/514 ; CGI art. 1649 ter A à E ; BOI-INT-AEA-30. Opérations réalisées depuis le 01/01/2023 ; dépôt au 31 janvier N+1 ; échange entre États membres au 28 février.
- Opérations visées : vente de biens, **« prestation de services par des personnes physiques »** (« travail à l'heure ou à la tâche… à la demande d'un utilisateur »), location de moyens de transport, location immobilière. Aucun seuil pour les services.
- Données : identité, NIF, **contrepartie totale par trimestre**, nombre d'opérations, commissions retenues, compte financier → préremplissage et récapitulatif annuel en janvier.
- **Patreon** (page d'aide « EU Creator: income reporting requirements (DAC7) », non lisible directement le 03/10/2026, HTTP 403 ; extrait de recherche) : Patreon indique déclarer les créateurs résidents UE pour « commissions, live chats, fan requests, member shout-outs, phone calls, and any other personal services carried out at the request of a user ». **Les abonnements à des contenus publiés ne semblent pas visés** — à vérifier auprès de Patreon. Ne jamais en déduire qu'un revenu non transmis n'a pas à être déclaré.
- **Substack** : paiements via Stripe ; régime DAC7 à vérifier de la même manière.

## 5. Reconstituer ses encaissements

- **Page des versements** (Patreon : `patreon.com/payouts`, historique complet ; API interne `payoutsv2/<campaign>/history` chargée par la page) : date, montant, destination (Hyperwallet, Stripe, PayPal), statut. Exclure les débits « abonnements à d'autres créateurs ».
- **Analyses → Revenus** : revenus bruts, frais de plateforme, frais de paiement, revenus nets par mois (6 derniers mois affichés ; « Exporter les données » pour un CSV).
- **Relevés bancaires** : les virements « Hyperwallet » / « Stripe » font foi pour la date d'encaissement (année civile).
- Tableau à produire : par année civile, encaissements totaux ; puis par mois si une régularisation URSSAF exige le détail.

## 6. À faire trancher

1. Case URSSAF (autoédition vs droits hors OGC) et brut/net de commission.
2. Qualification TVA de l'opération de l'auteur vis-à-vis de la plateforme et montant du CA.
3. Part « service » d'une offre mixte (canal, Q&R) : seuil de tolérance ?
4. Périmètre DAC7 réel de chaque plateforme (abonnements inclus ou non).
