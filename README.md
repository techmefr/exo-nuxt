# TP Nuxt 3 - Développement d'un site.

![Maquette](./maquette.avif)

## Contexte

Vous allez développer une application web inspirée de la maquette ci-dessus. Ce projet vous permettra de maîtriser progressivement l'écosystème Nuxt 3 : interface utilisateur avec Vuetify, gestion d'état avec Pinia, et qualité logicielle avec les tests unitaires.

L'approche sera itérative - chaque étape construit sur la précédente tout en introduisant de nouveaux concepts.

---

## Étape 1 - Initialisation du projet

Créez votre environnement de développement Nuxt 3. Configurez Vite comme bundler.

**Ce qu'on attend :** Un projet fonctionnel avec une page d'accueil basique. Initialisez votre dépôt Git dès maintenant.

---

## Étape 2 - Intégration de Vuetify

Recherchez comment intégrer Vuetify à votre projet Nuxt 3. Vous découvrirez qu'il existe plusieurs approches - choisissez celle qui correspond le mieux aux recommandations officielles **actuelles**.

---

## Étape 3 - Construction de l'interface

Analysez attentivement la maquette fournie. le but étant d'utiliser au mieux vuetify et de comprendre comment construire et maîtriser sa grille mais aussi les composants de bases. Bien sûr il faudra utiliser au mieux Vue.

**L'objectif ici :** Reproduire fidèlement cette interface en vous appuyant sur les composants Vuetify. Vous devrez faire quelques recherches pour identifier quels composants utiliser - c'est volontaire. Cette exploration vous sera utile pour la suite. Pas besoin de penser aux responsive, les utilisateurs ne seront que sur desktop, ce n'est pas le but de l'exercice.

---

## Étape 4 - Mise en place des tests

Maintenant que vous avez une interface, sécurisez votre développement avec Vitest et Vue Test Utils. 

**Premier objectif :** Vérifier que vos composants se renderisent correctement.

Les tests peuvent sembler fastidieux au début, mais ils vous feront gagner un temps fou sur un vrai projet tout en permettant de ne pas casser des fonctionnalités au fur et à mesure de l'avancement du projet.

---

## Étape 5 - Tableau de données

Créez une page avec un tableau de données. [Simulez des données d'outils de design (nom, catégorie, prix, note utilisateur, etc.).](https://dummyjson.com/docs)

**Fonctionnalités requises :** pagination, triage par ordre croissant ou décroissant et possibilité de modifier le nombre d'éléments par page. Explorez les composants Vuetify dédiés aux tables - ils sont plus puissants qu'on ne le pense. Il faut utiliser les données du back uniquement et utiliser la version serveur du tableau avec une recharge pour chaque action faîte... Qui dit API dit sécurité ;)

---

## Étape 6 - Gestion d'état avec Pinia

Intégrez Pinia et développez une fonctionnalité de contact. Les utilisateurs doivent pouvoir envoyer des commentaires via un formulaire avec plusieurs champs (nom, prénom, email, téléphone, message) et vous devez pouvoir consulter ces messages sur une page dédiée.

**Point clé :** Toute la logique de stockage passe par Pinia. Pas d'API pour l'instant, juste de la gestion d'état côté client. Vous découvrirez la puissance de Pinia pour organiser votre logique métier. Bien évidemment, on pense sécurité même si back first ;)

---
## Étape 7 - Traduction avec i18n

Pour cetet étape il s'agit de traduire en deux langues minimums tout ce qui est visible dans l'application et de réfléchir à l'organisation de ces données.

---

## Étape 8 - Système de préférences utilisateur

Développez une page de profil où les utilisateurs personnalisent leur expérience : Changement d'avatar, changement de pleurs infos, thème sombre/clair, taille de police, couleur d'accent, etc. Le tout regroupé par catégorie. L'idée est de pouvoir tester d'autres composants non utilités encore permettant d'améliorer la visibilité mais de commencer à travailler avec d'autres outils de nuxt et vuetify en allant plus loint dans leur configuration et usages.

**Le défi technique :** Ces préférences doivent s'appliquer instantanément à toute l'application et persister entre les sessions. Vous toucherez ici aux concepts de réactivité Vue et de persistance de données.

---


## Étape 9 - Les tests avec Vue test utils et Vitest

Finalisez votre suite de tests ! Toujours autour de tests unitaires et un fichier de test par fichiers dans le projet.

**Objectif qualité :** Vous devez pouvoir modifier votre code en confiance. Un bon test vous dit immédiatement si vous avez cassé quelque chose.

---

## Quelques conseils pratiques

La documentation Vuetify est assez bonne et leurs exemples sont directement utilisables. Prenez le temps de la parcourir plutôt que de chercher des solutions, sans oublier d'aller voir leur code pour savoir comment sont construits les composants.

Organisez votre code dès le début. Créez des composants réutilisables quand vous voyez de la duplication. Votre futur vous dira merci.

N'hésitez pas à expérimenter au-delà des consignes. Si vous avez une idée pour améliorer l'UX ou ajouter une fonctionnalité, foncez. C'est comme ça qu'on apprend. Mais plutôt en étape 10 ;)

---

**Bon développement !** Ce projet couvre l'essentiel de ce qu'on attend d'une application Nuxt 3. Une fois terminé, vous aurez une base solide pour attaquer des projets plus ambitieux.
