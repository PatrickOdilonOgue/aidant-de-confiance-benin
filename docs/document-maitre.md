# Aidant de confiance — document maître public
Version du 19 novembre 2026. Document de conception, non certification juridique ou technique.

## 1. Résumé exécutif
Le projet vise à encadrer l’aide apportée à un usager pour une démarche administrative au Bénin : choix de l’aidant, droits limités, accord explicite, paiement par le canal officiel et possibilité de révocation. Le démarrage recommandé porte sur une seule démarche, dans un site volontaire. Un pilote de 90 jours ne commence qu’après validation des conditions juridiques, techniques et financières.

L’indépendance vis-à-vis d’un concours signifie que les travaux utiles peuvent continuer sans prix. Elle ne signifie pas que le projet peut s’affranchir des règles administratives. Aucun partenaire, agrément, financement ou accès informatique public n’est acquis. Le budget et les volumes sont des hypothèses.

## 2. Besoin à vérifier
Le dossier initial décrit une difficulté d’accompagnement familial. La version publique ne révèle ni relation familiale identifiable, ni situation médicale, ni adresse. Ce signal qualitatif ne démontre ni la fréquence nationale du problème ni l’absence de procurations existantes. Dix entretiens exploratoires sont proposés, avec usagers, aidants et agents, pour cartographier une démarche et vérifier les solutions déjà admises.

Public initial : adultes capables de consentir souhaitant une aide, notamment personnes âgées, personnes en situation de handicap ou éloignées de leurs proches. Le handicap ne doit pas être assimilé à une incapacité juridique. Mineurs, tutelles, conflits de représentation et incapacité de consentir sont hors pilote ordinaire et orientés vers le cadre compétent.

## 3. Offre et périmètre
Trois niveaux sont séparés :
1. Découverte : entretiens minimisés, cartographie et simulation sans données réelles.
2. Faire avec : aider à comprendre et préparer une démarche, sans récupérer les codes secrets et selon un cadre de données défini.
3. Faire pour : déposer ou suivre à la place de l’usager uniquement si le service autorise cette représentation et les preuves retenues.

La démarche candidate est l’accompagnement d’une demande d’état civil pour un adulte. Le service compétent doit confirmer les actes représentables, les pièces, les frais et les conditions de remise. Le projet ne promet pas un accès au registre d’identité, la suppression de toutes les pièces, zéro déplacement ou un mandat valable partout.

Hors première version : portefeuille financier, transport, foncier et santé, biométrie vocale, USSD national, intégration ANIP non autorisée et décision automatique sur les droits. Le prototype public ne constitue pas l’application réelle.

## 4. Rôles et règles
| Rôle | Périmètre proposé | Limite |
|---|---|---|
| Titulaire | Choisir, comprendre, confirmer, suspendre et réclamer | Le silence ne vaut pas accord |
| Aidant | Préparer, déposer ou suivre selon droits | Ni mot de passe du titulaire ni extension unilatérale du mandat |
| Payeur | Autoriser le débit de ses propres fonds | Le paiement ne donne pas accès au dossier |
| Relais | Expliquer et accompagner | Ni autorité d’identité autoproclamée ni collecte de fonds publics |
| Administration | Vérifier, instruire et décider | Le logiciel ne se substitue pas à sa compétence |
| Opérateur technique | Maintenir et protéger selon contrat | Pas de réutilisation commerciale des données |

Un mandat indique démarche, titulaire, aidant, droits, échéance, plafond cumulé et méthode de révocation. Déposer, suivre, payer et recevoir sont des droits séparés. Création, changement de droits et récupération d’accès exigent une procédure d’identité et de consentement admise, à définir avec le service. Un NPI, une SIM ou un SMS ne sont pas traités comme preuve suffisante à eux seuls.

## 5. Parcours cible
1. Accueillir, expliquer les alternatives et vérifier la compréhension sans pression familiale.
2. Appliquer la méthode de vérification admise ; conserver une référence plutôt qu’une copie si cela suffit.
3. Définir un mandat limité et remettre une copie accessible.
4. Préparer une demande et vérifier les droits à chaque action.
5. Présenter l’objet et les frais au titulaire ; attendre son accord actif.
6. Si des frais existent, obtenir référence et montant depuis le canal officiel. Le payeur autorise séparément son débit.
7. Vérifier le statut du paiement auprès de sa source ; une capture d’écran ne suffit pas.
8. Laisser l’administration instruire et remettre selon ses règles. Aucun délai dépassé ne crée automatiquement un accord.
9. Permettre suspension, réclamation et clôture.

Une révocation bloque les nouvelles actions, mais n’efface pas une transmission ou un paiement déjà effectué. Un paiement tardif est traité en exception avec le bénéficiaire habilité. Aucun remboursement de fonds publics n’est décidé unilatéralement par le projet.

## 6. Conformité et données
Avant tout usage réel : identifier le responsable de chaque traitement, la base juridique, les destinataires, les formalités, la durée, les sous-traitants, l’hébergement et les éventuels accès depuis l’étranger. La représentation, la preuve de consentement et la remise d’un acte doivent être validées pour chaque démarche. Une convention ne peut pas supprimer une obligation légale.

Le guide APDP rappelle les principes de minimisation, de proportionnalité et de conservation limitée : https://archive.apdp.bj/wp-content/uploads/2022/01/GUIDE-DE-MISE-EN-CONFORMITE_Pt_YD_revu.pdf . Cette source de cadrage ne remplace pas une analyse juridique actualisée du traitement.

Données candidates : identifiant interne, contact nécessaire, référence de vérification, mandat, confirmation, référence du dossier, statut et référence de paiement. Pas de copie d’identité, acte, donnée médicale ou enregistrement vocal par défaut. Les durées exactes seront approuvées avant ouverture ; aucune conservation indéfinie n’est prévue. Les journaux nominatifs restent privés. Les publications ne contiennent que des résultats agrégés ne permettant pas d’identifier les participants.

## 7. Application réelle à construire
Architecture proposée : interface accessible, serveur d’authentification et d’autorisation, base relationnelle, journal privé, file de notifications et connecteurs expressément autorisés. Un monolithe modulaire suffit pour commencer ; les accès institutionnels ne sont pas présumés publics.

Objets minimaux : personne, vérification, mandat versionné, demande, consentement lié à une action, avis, paiement, événement et incident. Contrôles côté serveur : refus par défaut, portée, échéance, plafond cumulé avec réservation des engagements, références uniques, idempotence et autorisation à chaque consultation. Les retours de paiement doivent être authentifiés et rapprochés.

Les comptes professionnels sont individuels, les secrets protégés et les environnements séparés. Prévoir sauvegardes chiffrées, restauration testée, correctifs, habilitations et procédure d’incident. Un journal chaîné ou une signature ne rend pas l’ensemble infalsifiable. La démonstration HTML ne teste aucune de ces garanties serveur.

## 8. Organisation et exploitation
Équipe proposée : porteur et suppléant, référent administratif, relais formé, développeur, testeur indépendant et conseil juridique/données à temps partiel. Identifier les responsables dans une convention avant ouverture. Les institutions évoquées sont des interlocuteurs à solliciter, pas des partenaires annoncés.

Chaque jour : vérifier disponibilité, demandes en attente, incidents et rapprochements. Chaque semaine : revoir les accès inhabituels, les réclamations, les dossiers incomplets et les dépenses. Chaque mois : restauration, revue des droits et politique de purge. En panne ou incident grave, suspendre les nouvelles actions sensibles et orienter vers le canal officiel.

Tester avec les personnes concernées : clavier, lecteur d’écran, zoom à 200 %, langage simple et possibilité d’accompagnement sans téléphone. Aucun accès à un droit public ne doit dépendre de la participation au pilote.

## 9. Financement et modèle économique
Hypothèse : prestation d’accompagnement ou contrat pilote financé par une structure volontaire, puis maintenance institutionnelle si sa valeur est démontrée. Aucun acheteur n’est acquis. Les frais publics restent séparés des recettes du projet ; aucun transit de ces fonds ni commission sur les droits publics n’est retenu. Une participation privée éventuelle serait facultative, distincte et encadrée.

Le budget de référence est détaillé séparément : 5 525 000 FCFA hors réserve, 6 353 750 FCFA avec réserve de 15 %. Montants internes à remplacer par devis. Aucun financement ni revenu confirmé ; ne pas engager la totalité sans fonds disponibles.

## 10. Calendrier, indicateurs et décision
Hypothèse : trois mois de préparation, puis 90 jours d’exploitation. Les accords peuvent décaler ce calendrier. Commencer sur un site, une démarche, et au maximum cinquante titulaires volontaires et cent demandes, objectifs proposés et non résultats. Un deuxième site exige une revue préalable.

Mesurer déplacements, temps, coûts nets incluant les frais nouveaux, complétude, issue, compréhension, incidents et satisfaction. Conserver les dénominateurs et les données manquantes ; ne pas remplacer un manque par zéro. Une comparaison descriptive avant/après ne prouve pas seule une causalité ni un impact national.

Poursuivre uniquement si besoin confirmé, droit d’agir établi, financement disponible, recette satisfaisante et exploitation maîtrisée. Aucun incident critique non résolu ne permet l’extension. Si arrêt : prévenir, bloquer les nouvelles opérations, traiter les dossiers et paiements en cours, révoquer les accès et appliquer les durées de conservation.

## 11. Livraison et réversibilité
Exiger code source, licences identifiées, documentation, migrations, tests, accès détenus par le porteur, sauvegardes et reprise par un tiers selon contrat. Payer les lots après réception. Avant production, exécuter les cas de refus, expiration, révocation, paiement répété ou discordant, récupération d’accès et restauration. La seule réussite du scénario fictif n’est pas une recette de production.
