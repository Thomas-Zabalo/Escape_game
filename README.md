# Escape Game - Projet Unity

## Organisation du Travail
Nous utilisons un système de tickets (**Issues GitHub**) pour structurer le travail. Chaque membre s'attribue un ticket et suit le workflow suivant :

1. **Création d'une branche**
   - À partir de `develop`, crée une nouvelle branche avec le nom :

![Workflow Git](https://github.com/user-attachments/assets/9fc4a40f-03b9-4199-bd9e-9587a8b6650b)
   
   - Exemple : `feature/mecanique-porte`

![Validation Process](https://github.com/user-attachments/assets/4793f2b8-7c97-4780-8de5-1b72be148831)

3. **Développement**
   - Implémente la fonctionnalité sur la branche créée.
   - Vérifie que tout fonctionne sans casser le projet.

4. **Validation**
   - Une fois terminé, passe le ticket en **"À valider"**.
   - Un autre membre teste la fonctionnalité sur sa machine.

5. **Merge vers `develop`**
   - Si tout fonctionne, fusionne la branche avec `develop`.
   - Supprime la branche une fois fusionnée.
   - Commandes :
     ```git
     git checkout develop
     git pull origin develop
     git merge feature/nom_du_ticket
     git push origin develop
     git branch -d feature/nom_du_ticket
     ```
     
## 📝 Au Niveau des Commits
On reste sur un style de commit dans le format suivant :
 
   ```git
   feat(nomdelabranche): Description de ce que tu as fait (#n° ticket)
   ```
Même si tu fait autre chose sur la meme branche garde cette structure

6. **Finalisation vers `main`**
   - Une fois toutes les features complétées et testées, on fusionne `develop` dans `main`.
   - Commandes :
     ```git
     git checkout main
     git pull origin main
     git merge develop
     git push origin main
     ```

## 🎮 État Actuel
- ✅ **First Person Controller** installé : déplacement fonctionnel.
- 🔄 Développement en cours...
