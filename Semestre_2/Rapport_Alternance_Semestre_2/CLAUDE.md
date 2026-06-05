# Rapport d'alternance CBA — Semestre 2

Mémo de travail pour ce rapport. À lire avant toute intervention sur `src/main.tex`.

## 1. Contexte

- **Auteur :** Lucas Moussaoui, Master ILSEN (CERI, Avignon), en alternance chez **CBA Informatique Libérale**.
- **Poste :** développeur Front-End dans l'équipe **Agathe You / Agathe Emotion**.
- **Tuteur entreprise :** Tom Andrieu — **Tuteur CERI :** Vincent Labatut.
- **Document :** projet LaTeX, compilé avec **LuaLaTeX**. Fichier principal `src/main.tex` ; commandes maison (`\initDocument`, `\imageCenter`, `\setImagesPath`) dans `src/preamble/` et `src/utils/`. Images dans `res/images/`.
- Le rapport actuel (~26 p.) contient déjà tout le **Semestre 1**. Objectif : **ajouter 15 à 20 pages de Semestre 2** (figures comprises) sans casser l'existant.
- **Rapport de référence (modèle) :** ancien alternant Hicham, rapport cumulatif sur 4 semestres →
  `C:\Users\Noxyzz\Documents\Cour\Alternance\Rapport_Alternance_Hicham_S4\src\main.tex`
  (utile pour le style, le ton et la manière de gérer un rapport multi-semestres).

## 2. Méthode de travail (IMPORTANT)

- **Lucas écrit la prose lui-même**, « normalement ». Le rôle de Claude est de :
  1. **mettre en forme en LaTeX** en respectant le style du document existant (`\subsection`, `itemize`, `\textbf`, `\imageCenter`, `\newpage`…) ;
  2. **challenger Lucas comme un examinateur de soutenance** sur ce qu'il doit dire ou non (fond, pertinence, cohérence, attendus d'un rapport d'alternance).
- **Ne JAMAIS inventer** le travail, les missions ou les chiffres : c'est un document académique évalué décrivant une expérience réelle. On n'adapte que le contenu fourni par Lucas.
- **Convention `;;`** : quand Lucas écrit `;;` dans un message, ce qui suit s'adresse à Claude
  (méta-commentaire, consigne) et ne fait PAS partie du contenu à intégrer au rapport.
- **Édition concurrente de `main.tex`** : ne PAS modifier `main.tex` pendant que Lucas y rédige
  (risque de conflit de sauvegarde / perte de brouillon). Attendre qu'il confirme avoir sauvegardé,
  ou lui demander de coller son texte dans le chat.
- **Conventions typographiques du rapport** :
  - `\textit{...}` pour les termes anglais / jargon technique (*User Story*, *WebView*, *logs*, *toggle*…) ;
  - `\textbf{...}` pour la mise en valeur (noms de produits, rôles, notions clés) ;
  - à la **première occurrence** d'un terme complexe : courte explication en français entre parenthèses
    ou via « c'est-à-dire » — le rapport doit rester lisible par un non-informaticien.

## 3. Intentions du nouveau rapport

- Produire **un seul rapport intégré couvrant les 2 semestres** (pas deux rapports juxtaposés), sur le **modèle éprouvé de Hicham** (ancien alternant, rapport cumulatif sur 4 semestres).
- Le contexte (entreprise, équipe, méthodo, outils, technos) est **tenu à jour au présent** avec les données fraîches du S2 — on ne crée PAS de section « évolution » séparée (source de redite).
- Fil rouge différenciant du S2 : **l'intégration de l'intelligence artificielle** dans les pratiques (les siennes + celles de l'entreprise).
- Approfondissement technique des parties existantes là où ça apporte une **vraie valeur** (surtout les technologies), sans gonfler artificiellement.

## 4. Où le « Semestre 2 » apparaît explicitement

Le découpage par semestre n'est visible qu'à **deux endroits** (le reste est fondu dans le contexte mis à jour) :
1. **Fonctionnalités développées** : nouveau groupe de tickets S2 ajouté à la suite des tickets S1.
2. **Analyse et bilan** : une analyse critique dédiée au S2.

## 5. Structure cible

```
1  Introduction                     [MAJ : couvre 2 semestres + angle IA]
2  CBA Informatique Libérale        [MAJ si besoin]
3  Environnements de travail
   3.1 Mon équipe                   [MAJ : changements d'équipe]
   3.2 La méthodologie
       3.2.1 SCRUM                  [MAJ : 1 phrase — Master Planning reporté]
       3.2.2 User Story
   3.3 Outils utilisés
   3.4 Technologies utilisées
       3.4.1 Struts … 3.4.4 Ui-Kit
       3.4.5 Le développement iOS   [NOUVEAU S2]
   3.5 L'intelligence artificielle au quotidien   [NOUVEAU S2 — section clé]
4  Mon début dans l'entreprise      [inchangé : historique S1]
5  Fonctionnalités Développées
   5.1 … 5.7  (tickets S1)
   >>> Bloc "FONCTIONNALITÉS — SEMESTRE 2" : nouveaux tickets 5.8+   [NOUVEAU S2]
6  Analyse et bilan de l'alternance
   6.1 Analyse critique — Semestre 1
   6.2 Analyse critique — Semestre 2   [NOUVEAU S2 — accueille la "montée en autonomie"]
   6.3 Lien Théorie - Pratique         [MAJ]
   6.4 Bilan personnel et professionnel [MAJ]
7  Conclusion
   7.1 Synthèse des points clés        [MAJ : synthèse globale 2 semestres]
   7.2 Conclusion du Semestre 2        [NOUVEAU S2 — conclusion propre exigée par la consigne]
   7.3 Ouverture                       [MAJ : retirer Master Planning, recentrer sur l'IA]
```

> **Introduction de la nouvelle partie S2** : la consigne impose de décrire en tête des réalisations
> du semestre tout changement *significatif* d'équipe ou de mission, et de montrer comment le travail
> a évolué. C'est le rôle du paragraphe d'intro placé juste avant les tickets S2 (bloc balisé dans `main.tex`).

(Optionnel, façon Hicham : une section **« Résolution de bugs »** si des anomalies ont été corrigées — pages concrètes et appréciées d'un correcteur.)

(Idée différée — **Lexique** façon Hicham : pas pour ce semestre (le rapport est encore assez court et
les termes sont expliqués à la première occurrence) ; à envisager au S3/S4 quand le volume aura grossi.)

## 6. Décisions prises (récap des échanges)

- ❌ **Pas de découpage « Partie I / Partie II »** : on actualise en place plutôt que de juxtaposer (évite la redite et tient la promesse d'« approfondir »).
- ✅ Le **Master Planning** annoncé en ouverture du S1 a été **reporté** → juste **une phrase** en 3.2.1 ; le SCRUM décrit reste en vigueur.
- ✅ La section **IA (3.5)** parle de l'**usage concret** (le sien + l'entreprise), des **formations** reçues et des **bonnes pratiques** — **sans définir ce qu'est l'IA** (éviter la dissertation / le hors-sujet).
- ✅ La **« montée en autonomie »** (rôle élargi, tickets plus complexes, moins de supervision) n'est PAS une section à part : elle vit dans **6.2 (Analyse critique S2)**.
- ✅ Section 6 restructurée pour éviter de nommer deux choses « bilan » : on parle d'**analyse critique** S1/S2 + bilan personnel séparé.

## 7. Consignes officielles CERI (semestre pair) — à respecter impérativement

1. **Corrections du tuteur CERI à intégrer.** Le rapport S1 a reçu un retour (forces/faiblesses)
   du tuteur CERI lors de la rencontre de mars. **Ces corrections DOIVENT être intégrées** dans cette
   version. Document de référence : la **grille d'évaluation rapport/soutenance** (dispo au secrétariat CERI).
   👉 *Statut : retour PAS ENCORE reçu (au 3 juin 2026) — attendu vers la semaine du 8 juin 2026.*
   *On peut rédiger le S2 en attendant, mais NE PAS figer les corrections S1 avant d'avoir ce retour.*
2. **Nouvelle partie S2 = 15 pages min, 20 max (figures comprises).** Doit : décrire tout changement
   significatif d'équipe/mission **en introduction de la partie**, montrer l'**évolution du travail**
   dans le temps / de nouveaux éléments techniques, et comporter un **bilan ET une conclusion propres** au S2.
3. **Page de garde** (à conserver, complète) : nom + prénom · diplôme + année + parcours ·
   entreprise (nom + ville) · tuteurs entreprise & CERI · dates début/fin de contrat.
4. **Objectifs inchangés** vs S1, mais **prise de recul plus importante** attendue
   (exigence renforcée en Master 2 ; Lucas est en M1, mais le recul reste un attendu fort).

## 8. Garde-fous examinateur

- **Traçabilité S2** : le correcteur doit identifier sans ambiguïté ce qui a été fait ce semestre → les nouveaux tickets, le 6.2 et la conclusion 7.2 doivent être nets et repérables.
- **Anti-redite** : chaque ajout S2 doit montrer une **progression**, pas redécrire le S1.
- **Anti-remplissage** : approfondir seulement là où il y a de la valeur technique ; ne pas rallonger pour faire du volume.
- **Budget pages** : viser **15 à 20 p.** de S2 (figures comprises) ; si les tickets ne suffisent pas, proposer la section « Résolution de bugs ».
- **Prise de recul** (attendu n°1 du semestre pair) : privilégier l'analyse réflexive à la simple description.
  Surtout en **6.2 (analyse critique S2)** et **7.2 (conclusion S2)** :
  **moins de « j'ai fait X », plus de « voilà ce que j'en retire / pourquoi c'était formateur ».**

## 9. État d'avancement

- [x] Squelette LaTeX posé (sections vides + marqueurs `% TODO S2`), document compile (`exit=0`).
- [x] Page de garde complétée (entreprise + ville, année/parcours) — **à VÉRIFIER par Lucas**.
- [ ] **Retour tuteur CERI sur le S1** : pas encore reçu (attendu ~semaine du 8 juin 2026) → intégrer les corrections dès réception.
- [ ] Intro de la nouvelle partie S2 (changements équipe/mission + évolution du travail)
- [ ] 3.5 Intelligence artificielle — à rédiger
- [x] 3.4.5 Développement iOS — rédigé (angle "techno de l'équipe" ; le vécu perso iOS ira dans les tickets S2 avec renvoi croisé)
- [ ] Tickets S2 (5.8+) — à rédiger
- [ ] 6.2 Analyse critique S2 — à rédiger
- [ ] 7.2 Conclusion du Semestre 2 — à rédiger
- [x] MAJ intro (§1) : couvre les 2 semestres + angle IA
- [ ] MAJ : 3.1 équipe, 3.2.1 Master Planning, 6.3, 6.4, 7.1 synthèse, 7.3 ouverture

> Les emplacements exacts à remplir sont balisés par des commentaires `% TODO S2` directement dans `src/main.tex`.
