# tp-git
Rien de description specifique  dans cette repository
# tp-git
Rien de description specifique  dans cette repository
# TP1 – Git Local

## 🎯 Objectif
Apprendre et pratiquer les commandes de base de Git : configuration, création de dépôt, commits, historique, retour en arrière, branches, fusion et gestion de conflits.

---

## 🚀 Étapes du TP

### 1. Configuration de Git
Définir votre nom et e-mail pour identifier vos commits :
```bash
git config --global user.name "VotreNom"
git config --global user.email "votre.email@example.com"


2. Initialiser un dépôt
git init tp-git
cd tp-git

3. Ajouter des commits

Créer trois fichiers et les committer :

echo "Ligne 1" >> fichier1
echo "Ligne 1" >> fichier2
echo "Ligne 1" >> fichier3
git add fichier1 fichier2 fichier3
git commit -m "Ajout des fichiers initiaux"

4. Visualiser l’historique

git log → affiche les commits

git log --oneline --graph --decorate → résumé visuel

git show HEAD → détail du dernier commit

5. Modifier des fichiers
echo "Ligne 2" >> fichier1
git diff              # voir les changements
git add fichier1
git commit -m "Ajout de Ligne 2 dans fichier1"

6. Revenir en arrière

git checkout fichier2 → revenir à la dernière version du fichier

git revert HEAD → annuler le dernier commit (inverse)

git reset --hard HEAD~1 → supprimer le dernier commit

7. Utiliser des branches
git branch develop
git checkout develop
echo "Contenu dev" >> fichierdev
git add fichierdev
git commit -m "Nouveau fichier dev"

8. Fusionner des branches

Depuis master :

git merge develop

9. Gérer un conflit de merge

Modifier le même fichier dans deux branches

Lancer un git merge develop → conflit ⚡

Résoudre manuellement le fichier

Puis valider :

git add fichierconflit
git commit --no-edit

✅ Résumé

Ce TP vous a permis de :

Configurer Git

Initialiser un dépôt

Créer et gérer des commits

Visualiser l’historique et les différences

Revenir en arrière

Travailler avec des branches

Fusionner et résoudre des conflits
