# Promenons-nous (la clim' n'y est pas)

Reprise de **« Promenons-nous dans les bois »** — actualité : canicule et sécheresse
de l'été 2026 (≈50 départements en restriction d'eau) + hausse des tarifs
réglementés de l'électricité au 1er août.

| Paramètre | Valeur |
|---|---|
| Ton | Familial, tout public |
| Format | Vertical 9:16 (TikTok / Reels / Shorts) |
| Durée cible | 58–65 s |
| Tempo | ~100 BPM |
| Gimmick | Le loup ne mange personne : il a trop chaud. Le vrai monstre, c'est la facture. |

---

## 1. Paroles

### Structure

| Bloc | Durée approx. | Cumul |
|---|---|---|
| Intro parlée | 5 s | 0:05 |
| Refrain 1 | 13 s | 0:18 |
| Couplet (appel / réponse ×6) | 20 s | 0:38 |
| Chute | 8 s | 0:46 |
| Refrain final | 13 s | 0:59 |

### Texte à coller dans Suno

```
[Spoken Intro]
Trente-huit degrés dans la maison...
Le loup, lui, il a fermé ses volets.

[Chorus]
Promenons-nous dans les bois
Pendant que la clim' n'y est pas
Si la clim' y était
On respirerait
Mais comme elle n'y est pas
On va bien transpirer
Loup, y es-tu ? Tu as chaud ? M'entends-tu ?

[Verse - call and response]
J'enlève ma chemise !
J'enlève mon pantalon !
Je ferme tous mes volets !
Je bois toute ma gourde !
J'allume le ventilo !
Je regarde ma facture...

[Spoken]
AAAAAAH !

[Bridge]
Le loup n'a mangé personne
Il est couché sur le carrelage
Avec le chat, avec le chien
Et le ventilo au maximum

[Chorus - outro]
Promenons-nous dans les bois
Pendant qu'il fait moins de trente
Si le loup y était
Il roupillerait
Mais comme elle n'y est pas
On ira tous à l'ombre
```

### Notes de calage mélodique

Le nombre de syllabes colle sur la comptine d'origine, ça se chante sans réfléchir :

| Original | Reprise | Syll. |
|---|---|---|
| Promenons-nous dans les bois | Promenons-nous dans les bois | 7 |
| Pendant que le loup n'y est pas | Pendant que la clim' n'y est pas | 8 |
| Si le loup y était | Si la clim' y était | 6 |
| Il nous mangerait | On respirerait | 5 |
| Mais comme il n'y est pas | Mais comme elle n'y est pas | 6 |
| Il nous mangera pas | On va bien transpirer | 6 |

Les 6 réponses du loup remplacent le rituel de l'habillage : au lieu de s'habiller
pour venir manger, il se déshabille pour survivre. La 6e (« Je regarde ma
facture... ») casse le rythme, puis le cri arrive une seconde plus tard — c'est là
qu'est la vanne, il faut laisser le silence respirer.

---

## 2. Prompt Suno

**Title**
```
Promenons-nous (la clim' n'y est pas)
```

**Style of Music**
```
french children nursery rhyme, kids choir singalong, acoustic guitar, ukulele,
glockenspiel, light hand claps, upbeat major key, 100 BPM, playful and warm,
call and response, clean modern production, short and punchy, no drums overload
```

**Exclude styles**
```
rap, trap, heavy drums, distorted guitar, dark, sad, slow ballad
```

### Méthode de génération

1. Générer **4 takes** (2 générations × 2 variantes).
2. Ne garder que celles entre **55 et 70 s** — au-delà, Suno rallonge en inventant
   des couplets, il faut re-générer plutôt que couper au montage.
3. Critères de sélection, dans l'ordre :
   - le refrain est bien reconnaissable comme la comptine d'origine ;
   - les 6 réponses du loup sont détachées les unes des autres (pas noyées) ;
   - il y a un vrai silence avant le « AAAAAAH ! ».
4. Si Suno chante le « AAAAAAH ! » au lieu de le crier : remplacer par
   `[Spoken] Aaah ! Ma facture !` et relancer.
5. Télécharger en **WAV** si dispo (meilleur pour CapCut), sinon MP3.

---

## 3. Banque d'images à collecter (en parallèle de Suno)

Sources libres de droits : [Pexels](https://www.pexels.com),
[Unsplash](https://unsplash.com), [Pixabay](https://pixabay.com),
[Wikimedia Commons](https://commons.wikimedia.org).
**Tout en vertical / portrait** quand c'est possible, sinon prévoir un recadrage.

### Bloc intro + refrain (ambiance canicule)
- `thermomètre canicule` / `heat wave thermometer`
- `soleil écrasant ville` / `heat haze street`
- `carte météo France rouge` (capture d'un bulletin, ou générer un visuel simple)
- `forêt sèche été` / `dry forest summer`
- `rivière asséchée` / `dried river bed cracked earth`
- `pelouse jaune grillée`

### Bloc appel / réponse (1 image par réponse, rythme rapide)
| Réponse | Recherche image |
|---|---|
| J'enlève ma chemise ! | `homme chaud transpire chemise` / `hot sweaty summer` |
| J'enlève mon pantalon ! | `short été jambes canapé` (rester bon enfant) |
| Je ferme tous mes volets ! | `volets fermés soleil` / `closed shutters summer` |
| Je bois toute ma gourde ! | `boire gourde eau soif` / `drinking water bottle thirsty` |
| J'allume le ventilo ! | `ventilateur` / `electric fan close up` |
| Je regarde ma facture... | `facture électricité` / `electricity bill euros` |

### Bloc chute
- `chien allongé carrelage chaleur`
- `chat étalé sol frais` (le grand classique du chat en tapis)
- `ventilateur gros plan pales`
- Optionnel : plan large d'un salon volets fermés, pénombre

### Bloc refrain final
- `ombre arbre parc été`
- `enfants jouent eau fontaine`
- `coucher de soleil apaisant`
- `pluie sur sol sec` (la libération)

**À viser : ~25 à 30 images.** Sur 60 s, ça fait environ 2 s par plan, avec des
rafales plus rapides (0,4 s) sur les 6 réponses du loup.

---

## 4. Prochaines étapes

- [x] Paroles
- [x] Prompt Suno
- [ ] Génération Suno → me donner la **durée exacte** de la take retenue
- [ ] Storyboard timecodé plan par plan (dépend de la durée réelle)
- [ ] Recette de montage CapCut (découpe, transitions, sous-titres, export)
