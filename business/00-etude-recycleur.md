# Le Recycleur — étude de faisabilité pas à pas

> Machine de collecte récompensée, multi-compartiments, avec un jeu construit sur l'univers **Tape-Taupe**.
> Document de travail. Tous les chiffres sont des **hypothèses de cadrage** à revérifier par devis et par cotation réelle
> (les cours matière varient de ±40 % d'une année sur l'autre).

---

## Étape 0 — La conclusion d'abord, pour ne pas se raconter d'histoires

Trois choses à intégrer avant tout le reste :

1. **La matière première ne paiera jamais la machine.** Une canette rapporte ~1,8 centime de métal.
   Même à 200 canettes/jour, ça fait ~110 €/mois, alors que la machine seule en coûte 200 à 280 en amortissement.
   La matière représentera **15 à 25 % de vos revenus**, pas 100 %.
2. **Le vrai produit, ce n'est pas le déchet, c'est l'attention.** Vous créez un point de passage volontaire,
   récurrent, identifié, avec un compte utilisateur. Ça, ça se vend : à l'enseigne qui héberge, à l'annonceur,
   à la collectivité qui a un budget prévention des déchets, au commerçant qui veut du trafic.
   Le déchet est le prétexte, l'audience est l'actif.
3. **Le marché est déjà validé — et occupé.** Lemon Tri (machines + récompenses, en magasin et en entreprise),
   Cliiink / Terradona (conteneur à verre gamifié avec points, vendu aux collectivités), Yoyo (bouteilles plastique
   + communauté + points), Tomra (le leader mondial de la machine elle-même).
   Bonne nouvelle : quelqu'un paie déjà pour ça. Mauvaise nouvelle : il faudra faire mieux qu'eux sur un axe.
   **Votre axe, c'est le jeu.** Aucun d'eux ne va plus loin que le système de points.

---

## Étape 1 — Quels objets déposer ? (le tri par valeur, pas par bonne intention)

Le bon critère n'est pas « qu'est-ce qui se recycle », c'est **combien d'euros par litre de machine**.
Une machine, c'est un volume fini qu'il faut vider avec un camion. Le PET est le pire ratio du marché :
il remplit tout et ne vaut rien.

### Tableau des matières (cours européens indicatifs, à recoter)

| Flux | Prix reprise | Poids unitaire | **€ / objet** | € / m³ de machine | Verdict |
|---|---|---|---|---|---|
| **Canette alu (UBC)** compactée | 900–1 400 €/t | 14 g | **0,018 €** | ~200 € | Moteur de trafic. Iconique. À garder. |
| Boîte de conserve acier | 100–250 €/t | 45 g | 0,008 € | ~40 € | Optionnel, alourdit les tournées |
| **Bouteille PET clair** | 250–450 €/t | 28 g | **0,010 €** | ~18 € | Indispensable en image, désastreux en volume → **compacteur obligatoire** |
| Flacon PEHD | 300–500 €/t | 30 g | 0,013 € | ~25 € | Idem |
| Capsule café alu | filière dédiée | 1,2 g | 0,0012 € | faible | Symbolique, pas rentable seul |
| Verre | 20–30 €/t | 300 g | 0,008 € | ~10 € | **Non.** Lourd, dangereux, sans valeur |
| Textile | 0 à négatif | — | ≤ 0 | — | **Non.** Filière en crise depuis 2024 |
| Papier / carton | 40–120 €/t | — | ~0 | ~15 € | **Non** en machine |
| **Câbles, chargeurs, écouteurs** | 1 500–3 000 €/t (mêlé cuivre) | 80 g | **0,08–0,20 €** | ~400 € | **Oui.** 10× la canette |
| **Petit DEEE** (souris, télécos, jouets élec.) | 200–500 €/t + soutien REP | 200 g | **0,05–0,12 €** | ~250 € | **Oui** |
| **Cartouche jet d'encre vide** | réemploi | 90 g | **0,20–2 €** | très élevé | **Oui.** Filière de reconditionnement mature |
| **Toner laser vide (OEM)** | réemploi | 800 g | **1–12 €** | très élevé | **Oui**, mais encombrant → bac dédié |
| **Smartphone / petit écran** | reconditionnement | 160 g | **3–60 €** si vivant, 0,5–2 € si HS | énorme | **Le jackpot.** Compartiment sécurisé + effacement des données |
| Piles alcalines | pris en charge REP (~0 €) | 24 g | 0 € | 0 | À accepter (service rendu, pas revenu) |
| Batteries lithium / vapes | valorisable mais **risque incendie** | — | variable | — | Seulement avec bac coupe-feu certifié |
| **Huile alimentaire usagée** | 400–800 €/t (biodiesel) | 1 L = 0,92 kg | **0,37–0,74 € / L** | **~550 €** | **La meilleure densité de valeur.** Quasi personne ne collecte en ville |
| Bouchons plastique | 200–300 €/t | 2 g | 0,0005 € | faible | Symbolique (assos), pas un revenu |

### Ce que ça dicte comme design de machine

**5 à 6 ouvertures, pas 12.** Chaque compartiment supplémentaire coûte un capteur, un bac, une rotation de vidage,
et surtout de la charge mentale pour l'utilisateur devant la machine.

| Trappe | Contenu | Rôle |
|---|---|---|
| 1 | Canettes alu + acier | Volume, habitude, image |
| 2 | Bouteilles PET / PEHD (avec compacteur) | Volume, image |
| 3 | **Petits DEEE + câbles + chargeurs** | **Marge** |
| 4 | **Cartouches / toners** | **Marge** |
| 5 | Piles + petites batteries (bac coupe-feu) | Service, conformité, aimant à trafic |
| 6 | **Huile de friture usagée** (bidon → cuve, trappe séparée) | **Marge + différenciation forte** |

> **La logique :** les flux 1 et 2 font venir les gens toutes les semaines. Les flux 3, 4, 6 font l'argent.
> Le jeu sert précisément à faire glisser les gens du flux 1 vers les flux 3-4-6.

---

## Étape 2 — D'où vient réellement l'argent (5 robinets, pas 1)

| # | Source | Mécanisme | Réaliste / machine / mois |
|---|---|---|---|
| 1 | **Matière** | revente aux recycleurs / affineurs | **150 – 250 €** |
| 2 | **Abonnement de l'hôte** | l'enseigne, la mairie, le campus, le bailleur ou l'entreprise paie le service (trafic + preuve RSE + tonnages certifiés) | **250 – 600 €** |
| 3 | **Média (écran)** | affichage local sur la machine, sponsor de saison, marque qui sponsorise « la Taupe Alu » | **100 – 400 €** |
| 4 | **Commissions partenaires** | le restaurant paie 0,30–1,50 € par bon effectivement utilisé, ou 40–90 €/mois pour être au catalogue | **50 – 200 €** (lent à démarrer) |
| 5 | **Soutiens & REP** | ADEME, Citeo, Ecosystem, Corepile, appels à projets collectivités | **variable, souvent en amorçage** |

### Le joker à surveiller : la consigne

Là où la consigne existe (Allemagne, Scandinavie), l'exploitant de machine touche une **commission de manutention
de l'ordre de 0,01 à 0,03 € par contenant** — indépendante du cours des métaux. À 300 contenants/jour,
c'est **200 à 270 €/mois de plus, par machine**, et ça change tout le modèle.
En France le dossier est ouvert depuis la loi AGEC et repoussé plusieurs fois.
**Ne construisez pas dessus, mais construisez une machine capable de le faire le jour où ça arrive**
(lecture code-barres EAN + reconnaissance de forme + comptage certifiable). C'est un choix technique à faire maintenant.

### La règle d'or sur les récompenses

**Ne financez jamais une récompense avec votre trésorerie.** Trois sources légitimes :

- **Le partenaire** : le restaurant offre −2 € (coût réel pour lui ~0,60 €) parce qu'il gagne un client. Il paie pour l'accès, pas vous.
- **L'hôte** : la grande surface finance « −1 € dès 10 € d'achat » sur son budget promo — ça lui remonte du panier moyen.
- **Le collectif** : l'arbre planté, la fresque, le banc, le concert de quartier → payés par la collectivité, sur un budget qui existe déjà.

Votre seule dépense assumée : un petit **fonds jackpot plafonné** (la Taupe d'Or, cf. étape 3), typiquement 30–50 €/machine/mois, sponsorisable.

---

## Étape 3 — Le jeu : « Les Taupes du Sous-Sol »

L'objectif de game design est précis : **transformer 8 secondes de corvée en 8 secondes de plaisir**,
puis donner une raison de revenir dans 6 jours, puis pousser vers les matières qui rapportent.
Trois couches.

### Couche 1 — La machine (le geste, 8 secondes) : c'est du Tape-Taupe inversé

Sous la ville vit un peuple de taupes ingénieures. Elles ne mangent pas les déchets : **elles les forgent**.
Chaque trappe est un terrier. Chaque matière a sa taupe.

- **La taupe appelle.** Un seul terrier s'illumine à la fois, une taupe sort de l'écran et pointe sa trappe.
  Vous ne « triez » plus, vous **nourrissez la bonne taupe**. Le geste est identique, l'intention est renversée.
- **Le Rush.** 30 secondes au chrono pour placer un maximum d'objets dans les bons terriers.
  Bon dépôt = son, lumière, vibration du bac, **+combo** (exactement la mécanique combo x3 / x5 déjà codée dans `index.html`).
  Mauvais dépôt = combo cassé, la taupe boude.
- **La Taupe Piégée.** Reprise directe du trap du jeu actuel : un objet non conforme (verre, ordure, emballage souillé)
  déclenche « **Ce n'est pas pour moi !** ». C'est de la pédagogie au tri déguisée en punition ludique — et ça protège vos bacs,
  donc votre prix de revente (un lot pollué se vend 30 % moins cher, voire est refusé).
- **La Taupe d'Or.** ~1 dépôt sur 80, tiré au sort, déclenche une animation dorée et une **récompense rare immédiate**
  (le repas offert, la place de ciné). La récompense **variable** crée l'habitude bien plus fortement que « 1 point = 1 point » —
  c'est ce qui manque à tous les concurrents actuels.

### Couche 2 — Le compte (la rétention, entre deux visites)

- **Ton terrier.** Tu élèves une colonie. Chaque matière déposée fait éclore et évoluer une taupe :
  Alu la Vive, Cuivrette, Plastok, Pétrolia (huile), Volta (piles), Circuita (électronique)…
  30 à 40 espèces, avec des raretés. **Une espèce ne peut éclore que si tu déposes sa matière.**
  → C'est le levier qui pousse un collectionneur de canettes à rapporter ses vieux chargeurs. Votre marge est là.
- **Le minerai, pas le point.** Les taupes te paient en **Alumium, Petrolite, Cuivrine, Volt**.
  Chaque récompense partenaire a un prix dans une monnaie différente.
  Et surtout : **vous pilotez le taux de change en temps réel.**
  Stock d'alu bas, cours du métal haut ? → week-end « **RUÉE VERS L'ALU** », l'Alumium vaut double.
  *Le game design devient un outil de pilotage industriel.* C'est ça, votre vraie innovation — ça n'existe nulle part.
- **La galerie souterraine.** Chaque machine est un nœud sur une carte de la ville.
  Le quartier creuse collectivement une galerie entre deux machines. Galerie reliée = **palier collectif atteint =
  récompense réelle et visible dans la rue** (un arbre, un banc, une fresque, un concert).
  Le collectif crée la pression sociale, la presse locale gratuite, et c'est *exactement* l'argument qui fait signer une mairie.
- **Les saisons.** Ligues de 6 semaines entre quartiers, écoles, entreprises, classement, trophée physique remis en mairie.
  C'est le produit que vous vendez aux collectivités et aux campus.
- **La Taupe Légendaire.** Chaque semaine, une taupe rarissime n'apparaît que dans **une seule machine de la ville, tirée au hasard**,
  annoncée le matin dans l'appli. Chasse au trésor urbaine. C'est le mécanisme qui a fait Pokémon Go — il fonctionne, et il est gratuit pour vous.

### Couche 3 — L'anti-triche (sinon tout s'effondre)

Un système de récompense sans contrôle se fait vider en 3 semaines par 4 personnes malignes.

- Détection matière physique : **poids + capteur inductif/capacitif + caméra** (pas juste un code-barres, qui se photocopie).
- **1 compte = plafond de minerai par jour** + plafond par machine + détection des schémas anormaux.
- Récompense créditée **après** validation matière, pas au moment du dépôt.
- Les objets de valeur (téléphones) passent en **vérification humaine différée** avant paiement du bonus.

---

## Étape 4 — Les chiffres : est-ce rentable ?

### 4.1 Compte d'exploitation d'**une** machine (scénario réaliste, bon emplacement, année 2)

Hypothèses : entrée d'hypermarché ou campus, ~30 000 passages/mois, 2 % de conversion,
600 sessions/mois × 6 objets = **3 600 objets/mois** (120/jour).
Mix : 55 % canettes, 25 % PET, 10 % DEEE/cartouches, 10 % divers, + 60 L d'huile.

**Revenus**

| Poste | Détail | € / mois |
|---|---|---|
| Alu | 1 980 canettes × 14 g = 27,7 kg × 1 200 €/t | 33 |
| PET | 900 × 28 g = 25 kg × 350 €/t | 9 |
| Petits DEEE / câbles | 300 objets × 0,08 € | 24 |
| Cartouches / téléphones | 60 objets × 1,50 € moyen | 90 |
| Huile | 60 L × 0,55 € | 33 |
| **Sous-total matière** | | **189** |
| Abonnement hôte | contrat de service | 350 |
| Média / sponsor | écran + sponsor de saison | 150 |
| Commissions partenaires | bons utilisés | 60 |
| **TOTAL** | | **749** |

> À noter : **10 % des objets déposés font 65 % du revenu matière.** Toute la stratégie de jeu doit viser ces 10 %.

**Coûts**

| Poste | Détail | € / mois |
|---|---|---|
| Amortissement machine | 12 000 € sur 60 mois (ou leasing ~280 €) | 200 |
| Collecte / vidage | 2 rotations/sem., mutualisées sur 8 machines/tournée | 130 |
| Maintenance, pièces, SAV | | 60 |
| Connectivité, hébergement, SaaS | | 15 |
| Assurance, vandalisme, provision | | 30 |
| Emplacement | négocié à 0 € en échange du service | 0 |
| Fonds jackpot (Taupe d'Or) | plafonné | 40 |
| **TOTAL** | | **475** |

**Marge de contribution : ≈ 275 €/machine/mois** en régime établi et bon emplacement.
En emplacement moyen (60 objets/jour, pas d'abonnement hôte), on tombe à **−100 €/mois** : la machine perd de l'argent.
**Le modèle est extrêmement sensible à l'emplacement.** Il n'y a pas de « machine moyenne », il y a des bons et des mauvais sites.

### 4.2 Le seuil de rentabilité de l'entreprise

Structure minimale en année 2 : 4 personnes (vous + 1 dev + 1 ops + 1 commercial) ≈ 22 000 €/mois chargés,
+ 5 000 € de frais = **27 000 €/mois, soit 324 k€/an**.

| Modèle | Calcul | Verdict |
|---|---|---|
| **A. Parc opéré (vous possédez les machines)** | 324 000 / (275 × 12) = **~100 machines** rien que pour l'équilibre, soit **1,2 M€ de CAPEX** | Lourd. Non finançable au démarrage sans levée ou leasing massif |
| **B. Vente / location + licence logicielle** | marge ~4 000 € par machine vendue + 150 €/mois d'abonnement. Équilibre à **~50 machines vendues/an + 100 machines sous licence** | **Atteignable en année 2-3 avec un commercial.** Pas de risque déchet, pas de camion, marge logicielle |

**Recommandation : modèle B.** Vous ne vendez pas du recyclage, vous vendez un **dispositif d'engagement clé en main**
à ceux qui ont déjà le trafic et déjà le budget : grande distribution, collectivités, campus, grandes entreprises (QVT + RSE),
festivals, stades, bailleurs sociaux. Ils gèrent (ou sous-traitent) le vidage. Vous gardez le jeu, la donnée, la marque et le catalogue de récompenses.

Le modèle A reste pertinent **plus tard**, en zone dense, et **uniquement sur les flux à haute valeur** (DEEE, cartouches, huile),
ou le jour où une consigne arrive.

### 4.3 Ce qui tue le projet (à surveiller comme le lait sur le feu)

| Risque | Impact | Parade |
|---|---|---|
| Emplacement médiocre | marge négative immédiate | contrat avec clause de volume minimum, droit de retrait à 6 mois |
| Coût de collecte | 1 machine isolée = tournée non rentable | **densité avant expansion** : saturer une ville avant d'en ouvrir une deuxième |
| Effondrement du cours de l'alu | −40 % sur la ligne matière | la matière n'est que 25 % des revenus → c'est justement la protection |
| Fraude | vous payez des récompenses pour du vide | détection matière physique + plafonds + validation différée |
| Incendie batterie lithium | sinistre total, assurance refusée | bac coupe-feu certifié ou pas de lithium du tout |
| Vandalisme / propreté | l'hôte résilie | télémétrie de remplissage, alerte, engagement de passage sous 24 h |
| Lassitude du jeu | fréquentation divisée par 3 au bout de 4 mois | saisons, événements, nouvelles espèces — c'est un **coût récurrent de contenu**, budgétez-le |

---

## Étape 5 — Réglementaire France (à ne pas découvrir après avoir acheté la machine)

- **Collecte de déchets = activité réglementée.** Selon les quantités stockées, relève du régime ICPE
  (déclaration ou enregistrement, rubriques DEEE / métaux / plastiques). Une machine en magasin reste petite,
  mais **votre local de massification, lui, sera concerné**.
- **Transport de déchets** : récépissé préfectoral obligatoire au-delà des seuils (0,1 t dangereux / 0,5 t non dangereux par chargement).
- **Filières REP** : DEEE, piles, cartouches et emballages sont sous éco-organismes agréés
  (Ecosystem, Ecologic, Corepile, Screlec, Citeo). **On ne revend pas librement des DEEE.**
  En revanche, être **point d'apport volontaire conventionné** peut ouvrir des soutiens — c'est un revenu, pas un obstacle.
- **RGPD** : compte utilisateur, géolocalisation, données de comportement → registre, base légale, durée de conservation, mineurs.
  Attention particulière : un jeu qui attire des enfants entraîne des obligations renforcées.
- **Données personnelles sur les téléphones collectés** : obligation d'effacement sécurisé et responsabilité en cas de fuite.
  C'est le flux le plus rentable **et** le plus engageant juridiquement.
- **Hygiène (huile)** : cuve étanche, bac de rétention, contrat avec un collecteur agréé.

---

## Étape 6 — Le plan pas à pas (ce que je ferais à votre place)

### Phase 0 — Valider qu'on vous paiera (0–2 mois, 3–8 k€)

Ne dessinez pas la machine. Vendez-la avant qu'elle existe.

- 10 entretiens : directeurs de magasin, services déchets de 3 collectivités, 2 campus, 2 grandes entreprises.
  **Une seule question qui compte : « combien payez-vous par mois pour ça ? »** S'ils ne chiffrent pas, il n'y a pas de marché.
- 15 commerçants pour le catalogue de récompenses : accepteraient-ils 0,50 € par bon utilisé ?
- Cotations réelles : appelez 3 recycleurs et faites-vous coter alu, DEEE, cartouches, huile. Remplacez mes chiffres par les leurs.
- **Livrable : le tableau de l'étape 4.1 rempli avec de vrais prix.** Go / no-go sur ce tableau.

### Phase 1 — Le pilote « magicien d'Oz » (2–6 mois, 15–30 k€)

**Ne construisez pas la machine.** Simulez-la.
Un meuble de tri instrumenté : 5 bacs, une balance connectée, un QR code, une tablette qui fait tourner **le jeu Tape-Taupe existant**,
et 4 h/semaine de présence humaine. 1 500 à 4 000 € par point, sur 2 ou 3 sites contrastés
(hypermarché / campus / pied d'immeuble).

Les 5 chiffres à mesurer, et rien d'autre :

1. **Taux de conversion** : % des passants qui déposent. Seuil de survie : **> 1,5 %**.
2. **Objets par session** : cible **> 5**.
3. **Rétention à 4 semaines** : % qui revient. Seuil : **> 25 %**.
4. **Mix matière** : quelle part des flux à valeur (DEEE, cartouches, huile) ? Cible **> 8 %** en nombre d'objets.
5. **Coût réel de collecte** par rotation, chronomètre en main.

> Si conversion < 1 % ou rétention < 20 %, le jeu ne compense pas la friction du geste.
> **Ne passez pas en phase 2** : pivotez vers un contexte captif (entreprise, campus, immeuble) où la fréquentation est acquise.

### Phase 2 — Une vraie machine, 3 à 5 sites (6–14 mois, 80–200 k€)

- Machine d'occasion, ou partenariat avec un fabricant existant (Tomra, Sielaff, ou des fabricants est-européens/turcs 40 % moins chers)
  plutôt qu'un développement hardware maison, qui vous coûtera 2 ans et 300 k€.
- Contrats hôtes signés **avant** l'installation, avec volume minimum.
- Objectif unique : **prouver une marge positive par machine sur 6 mois consécutifs.**

### Phase 3 — Choisir le modèle et changer d'échelle

Avec 6 mois de données réelles, l'arbitrage A vs B se tranche tout seul.
Financement : leasing du hardware (l'actif est un bon collatéral), subventions ADEME / région,
puis levée uniquement si le modèle A est retenu.

---

## Étape 7 — Ce que vous avez déjà, et le prochain pas concret

Vous avez déjà, dans ce dépôt, le cœur du produit : un jeu Tape-Taupe qui tourne, avec grille de trous,
combos, taupe-piège, difficulté croissante et record local. **C'est le prototype de l'écran de la machine.**

Le prochain commit utile n'est pas une machine. C'est :

1. Ajouter au jeu la notion de **matière** : les taupes deviennent Alu, Cuivrette, Plastok, Pétrolia — on ne tape plus, on nourrit.
2. Ajouter un **compte + minerai + terrier** (collection d'espèces), en local d'abord.
3. Un **écran de récompense** avec 5 faux partenaires, pour tester la désirabilité auprès de 30 personnes réelles.

Ça coûte quelques week-ends, ça ne coûte pas 12 000 € de machine, et ça vous donne le support de démonstration
pour faire les 10 entretiens de la phase 0.

---

## Verdict

| Question | Réponse |
|---|---|
| Rentable en revendant la matière ? | **Non.** Jamais. 150–250 €/mois/machine, ça ne paie même pas la machine. |
| Rentable comme dispositif média + RSE + logiciel ? | **Oui, c'est possible** — ~275 €/mois de marge par machine bien placée. |
| En possédant le parc ? | Il faut ~100 machines et 1,2 M€ pour atteindre l'équilibre. Trop lourd pour démarrer. |
| En vendant le système à ceux qui ont le trafic ? | **Voie recommandée.** Équilibre atteignable en année 2-3. |
| Le facteur décisif ? | **L'emplacement**, puis le jeu. Un mauvais emplacement perd de l'argent quel que soit le jeu. |
| Votre différenciation défendable ? | **Le jeu et le taux de change du minerai** — piloter l'économie du jeu selon le cours des matières. Personne ne le fait. |
