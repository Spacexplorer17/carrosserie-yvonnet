# Carrosserie Yvonnet — Brief projet V0

Dernière mise à jour : 30 septembre 2026.

## Objet

Préparer puis construire une maquette V0 haute fidélité, multipage, navigable et responsive du futur site Carrosserie Yvonnet. La V0 doit pouvoir être parcourue et critiquée avec le dirigeant. Elle ne constitue ni un site validé pour publication ni une autorisation de déploiement.

Le site doit devenir le point d'entrée numérique de l'écosystème Yvonnet : il présente l'entreprise, ses métiers, ses locaux et ses démarches utiles, puis oriente vers les activités ou réseaux adaptés sans reconstituer leurs outils.

## Hiérarchie de l'écosystème

- **Carrosserie Yvonnet** : marque et sujet principal ; atelier, carrosserie, peinture, entretien et services réellement confirmés.
- **Cognac VSP / AIXAM** : activité de véhicules sans permis à proximité. Le parcours vente/entretien rapporté doit être validé avant publication. Ne pas recréer son catalogue.
- **Five Star** : réseau de carrosserie dans lequel Yvonnet figure publiquement ; ce n'est ni un assureur ni un agrément universel.
- **Club Auto Conseil / My Auto Conseil** : réseau et ressources complémentaires ; ne présenter que les avantages effectivement applicables à Yvonnet.
- **Assureurs et autres partenaires** : catégorie distincte, à afficher uniquement après confirmation actuelle et vérification des droits d'usage des logos.

## Public et parcours prioritaires

Le site s'adresse à de vrais automobilistes du secteur de Cognac/Châteaubernard.

1. Besoin de carrosserie ou peinture → comprendre le métier → contacter l'atelier.
2. Besoin d'entretien ou mécanique → voir les services confirmés → contacter l'atelier.
3. Recherche d'un véhicule sans permis → comprendre le rôle de Cognac VSP/AIXAM → accéder au site externe vérifié.
4. Comprendre les réseaux → distinguer Five Star de Club Auto Conseil et des agréments.
5. Trouver l'établissement → coordonnées, itinéraire et horaires validés.

## Architecture cible

- Accueil → `/`
- Nos métiers
  - Carrosserie & peinture → `/carrosserie-peinture/`
  - Entretien & mécanique → `/entretien-mecanique/`
  - Mobilité & services → `/services/`
- Véhicules
  - Véhicules d'occasion → `/vehicules/occasions/`
  - Cognac VSP · AIXAM → `/cognac-vsp/`
- Nos réseaux
  - Five Star → `/reseaux/five-star/`
  - Club Auto Conseil → `/reseaux/club-auto-conseil/`
- L'entreprise → `/entreprise/`
- Contact → `/contact/`

Chaque destination est une vraie page chargeable directement. Les boutons parents ouvrent des sous-menus au clic et au clavier ; le survol ne doit jamais être le seul moyen d'accès.

## Direction artistique de travail

- Blanc dominant, rouge Yvonnet, anthracite/noir, photographies réelles.
- Palette provisoire : `#FFFFFF`, `#F4F4F2`, `#202124`, rouge de travail `#D71920`, rouge sombre `#AD1320`.
- Ces couleurs ne sont pas présentées comme une charte officielle ; les contrastes priment.
- Deux familles typographiques au maximum. Piste : Barlow Condensed pour certains titres et Source Sans 3 pour le texte, ou équivalent justifié et licencié.
- Grandes photographies utiles, composition éditoriale, angles nets ou très légèrement arrondis, peu d'ombres.
- Aucun univers noir/or, aucune esthétique SaaS, aucun faux atelier généré, aucune supercar de banque d'images.
- Les logos partenaires gardent leurs proportions et couleurs ; ils ne pilotent pas l'identité Yvonnet.

## Principes de contenu

- Écriture factuelle, naturelle et spécifique à Yvonnet.
- Aucun fait commercial ne doit être fabriqué pour compléter une maquette.
- Une donnée publique conserve sa provenance et son statut ; elle n'est pas pour autant validée pour publication.
- Une information inconnue est omise ou annotée `À confirmer` dans la V0.
- Les pages avec peu de matière restent compactes et utiles ; elles ne sont pas gonflées avec du vide ou du texte générique.
- Pas de faux témoignage, statistique, promotion, garantie, badge « ouvert », formulaire réellement envoyé ou calendrier donnant l'illusion d'un rendez-vous confirmé.

## Photographie

Les quatre références initiales sont : accueil/comptoir rouge, façade/cour, façade/signalétique Five Star et assureurs, logo Cognac VSP/AIXAM. Elles sont temporaires et ne sont pas réputées finales, récentes ou libres de droits sans vérification.

Le design doit prévoir des médias remplaçables avec sujet, ratio desktop/mobile, point focal, alternative, provenance, droits et état. Voir `docs/PHOTO_SHOTLIST.md`.

## Contraintes fonctionnelles de la V0

- Indication visible : `Maquette de présentation — contenus en cours de validation`.
- Directive `noindex` dans les pages servies ; `robots.txt` seul ne suffit pas et `noindex` n'est pas un contrôle d'accès.
- Formulaire sans backend : annoncer avant interaction qu'il s'agit d'une démonstration, puis afficher un récapitulatif indiquant qu'aucun message n'a été envoyé.
- Coordonnées, médias, liens externes, services et statuts de validation centralisés.
- Aucun CMS, backend, analytics, chatbot, paiement, synchronisation de stock ou intégration intrusive dans la V0.
- Si le dépôt reste neuf au début du développement, Astro + TypeScript en génération statique est la piste recommandée ; sinon conserver la stack adaptée trouvée.

## Responsive, accessibilité et QA

- Concevoir le mobile séparément, pas simplement empiler le desktop.
- Tester au minimum 320, 360, 390, 430, 768, 1024 et 1440 px, ainsi qu'un écran large.
- HTML sémantique, langue française, lien d'évitement, titres cohérents, labels explicites, focus visible, erreurs compréhensibles, alternatives d'images et `prefers-reduced-motion`.
- Contraste cible de 4,5:1 pour le texte courant dans les cas applicables ; cible tactile d'environ 44 × 44 px.
- Vérifier les dix routes, rechargements directs, liens, sous-menus, clavier, débordements, images, console, formulaire de démonstration et `noindex`.
- Réaliser une revue Anti-Vibe corrective avant de qualifier la V0 de terminée.

## Hors périmètre actuel

- Déploiement, mise en production ou modification du site public.
- DNS, domaine, fiche Google Business, comptes partenaires, Search Console.
- Validation juridique, mentions légales définitives, cookies factices.
- Reprise automatique d'annonces Leboncoin sans flux/API contractuel vérifié.
- Publication de logos d'assureurs ou du statut Tesla sans preuve et autorisation.
