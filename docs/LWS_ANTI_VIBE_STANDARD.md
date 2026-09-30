# LWS Anti-Vibe Coding Standard

Ce standard est obligatoire pour le projet Carrosserie Yvonnet.

L'IA est utilisée comme outil d'exécution et d'assistance. Elle ne doit pas produire un site reconnaissable comme une landing page générée automatiquement.

## Principes non négociables

### 1. Intention avant décoration

Chaque page, section, composant et élément graphique doit avoir une fonction identifiable.

Avant d'ajouter un élément, pouvoir répondre à : « Quelle information, fonction ou identité apporte-t-il ? »

Si la réponse est uniquement « ça fait moderne », « ça remplit », « ça décore » ou « ça rend mieux », ne pas l'ajouter.

### 2. Aucune décoration IA générique

Éviter par défaut :

- points décoratifs ;
- blobs ;
- orbes ;
- grilles abstraites ;
- gradients gratuits ;
- petites étoiles ;
- pills/badges décoratifs ;
- lignes arbitraires ;
- glow ;
- glassmorphism ;
- icônes ajoutées pour remplir ;
- illustrations abstraites sans fonction ;
- animations répétitives au scroll.

Ces éléments ne sont autorisés que lorsqu'ils appartiennent réellement à l'identité visuelle définie du projet.

### 3. Pas de « cardification »

Ne pas transformer automatiquement chaque information en carte.

Préférer selon le contenu : typographie, photographie, listes, colonnes, tableaux, composition éditoriale, espace et hiérarchie.

Une grille de trois cartes n'est jamais la solution par défaut.

### 4. Zéro répétition

Une idée = un endroit.

Ne pas répéter sous différentes formulations : proximité, qualité, confiance, accompagnement, indépendance, expertise, etc.

Fusionner ou supprimer toute section dont le message existe déjà ailleurs.

### 5. Copywriting humain

Interdire les formulations génériques de landing page IA telles que :

- « Donnez vie à votre vision. »
- « L'excellence au service de... »
- « Une expérience qui vous ressemble. »
- « Votre réussite, notre priorité. »
- « Réinventez votre... »
- « Bien plus qu'un... »
- « Au cœur de... »
- « Passion, expertise et excellence. »

Préférer des phrases factuelles, spécifiques et naturelles. Le contenu doit pouvoir être dit oralement par l'entreprise sans paraître artificiel.

### 6. Contenu spécifique au client

Le site doit refléter son métier réel, ses services réels, sa localisation, son histoire, ses contraintes, ses clients, ses photos, ses preuves vérifiables et son identité.

Test obligatoire : si remplacer le nom et le métier du client par ceux d'un plombier, avocat, restaurant ou autre entreprise laisse la majorité du site crédible, le résultat est trop générique.

### 7. Preuves réelles > décoration

Privilégier : vraies photos, vraies réalisations, vrais locaux, vraie équipe, vrais équipements, vrais avis, vraies certifications et vraies informations.

Ne jamais inventer une preuve sociale pour rendre la page plus convaincante.

### 8. Mobile conçu séparément

Le mobile ne doit pas être simplement le desktop empilé verticalement.

Pour chaque page mobile : revoir l'ordre, supprimer ce qui devient inutile, réduire les textes, adapter les CTA, adapter les images, contrôler la densité et limiter le scroll inutile.

Tester réellement au minimum 320, 360, 390 et 430 px.

### 9. Éviter les landings interminables

Ne pas mettre automatiquement tout le site sur une seule page.

Lorsque le contenu le justifie, créer de vraies pages : Accueil, Services, Réalisations, À propos, Contact, etc.

La navigation doit permettre de comprendre l'architecture du site.

### 10. Animations sobres

Aucune animation ne doit exister uniquement pour montrer qu'une animation est possible. Pas de fade-up systématique sur chaque section. Respecter `prefers-reduced-motion`.

### 11. Test de suppression

À la fin du développement, examiner chaque élément purement visuel.

Question : « Si je le supprime, est-ce que le site perd une information, une fonction ou un élément important de son identité ? »

Si non, envisager sérieusement sa suppression.

### 12. Professionnalisme > effet wow

Ne pas optimiser le site pour une capture Dribbble/Awwwards.

Optimiser pour : crédibilité, compréhension, rapidité, navigation, conversion, accessibilité, durabilité et cohérence métier.

### 13. IA invisible

Le visiteur ne doit pas pouvoir deviner le processus de génération en observant la structure, les textes, les composants, les décorations, les images ou les animations.

Utiliser l'IA massivement en interne est acceptable. Produire un résultat visiblement généré par IA ne l'est pas.

### 14. Revue Anti-Vibe obligatoire

Avant de considérer la tâche terminée, effectuer une revue dédiée.

#### Anti-Vibe / contenu

- répétitions ?
- phrases génériques ?
- informations interchangeables ?
- contenu réellement spécifique ?

#### Anti-Vibe / design

- décoration gratuite ?
- trop de cards ?
- composants clichés ?
- identité réellement cohérente ?

#### Anti-Vibe / mobile

- scroll excessif ?
- desktop simplement empilé ?
- éléments inutiles ?
- navigation adaptée ?

#### Anti-Vibe / business

- le site ressemble-t-il réellement à l'entreprise ?
- les CTA correspondent-ils à son activité ?
- chaque page a-t-elle une fonction commerciale identifiable ?

Lister les problèmes détectés et les corriger avant livraison.

Important : ne jamais « corriger » un manque de personnalité en ajoutant davantage de décoration. La personnalité doit principalement venir du contenu, de la typographie, de la photographie, de la composition et de l'identité réelle du client.

### Complément 15. Incertitude > invention

Une information inconnue, ambiguë ou non vérifiée reste à confirmer. Ne complète jamais une prestation, une certification, un chiffre, un témoignage, une disponibilité ou une promesse par supposition.

Un contenu manquant doit rester identifié comme manquant, sans empêcher de travailler sa future composition.

## Précisions d'application au multipage

- « Zéro répétition » vise le remplissage éditorial : les repères de navigation, coordonnées utiles, CTA contextuels et un bref résumé menant à une page détaillée restent légitimes. Ne supprime pas ces repères au nom d'une application littérale qui dégraderait l'usage.
- « Pas de cardification » n'interdit pas une carte lorsqu'elle porte un vrai objet autonome, par exemple une annonce réelle. Cela interdit d'en faire la réponse automatique à tout le contenu.
- « IA invisible » est un objectif de qualité et de spécificité, pas une autorisation d'inventer des preuves humaines ou une promesse mesurable d'indétectabilité.
