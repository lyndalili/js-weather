# Projet "Application météo"

## Objectif
- Lorsque l'utilisateur envoie le formulaire, effectue une requête HTTP vers une API permettant d'obtenir la météo actuelle de la ville choisie par l'utilisateur. À la réception de la réponse, met à jour toutes les données affichées sur la page (jour, heure, température, description de la météo, etc.)

## Aller plus loin
- Entre le moment où l'utilisateur envoie le formulaire et le moment où la réponse à la requête HTTP est reçue, affiche lui l'animation de chargement (fais apparaître / disparaître l'élément ayant la classe `js-loading` aux bons moments).
- Optimise l'utilisation de l'API en faisant en sorte que la requête HTTP ne se refasse pas si l'utilisateur envoie le formulaire avec le même nom de ville à moins de 10 minutes d'interval *(il n'y a pas besoin de setInterval)*
- Refais la requête HTTP et met à jour les données affichées automatiquement toutes les 10 minutes
- Rajoute un bouton "Sauvegarder la ville" qui sauvegarde le nom de la ville dans le sessionStorage. À l'arrivée sur la page, si un nom de ville est stocké en sessionStorage, effectue immédiatement une requête