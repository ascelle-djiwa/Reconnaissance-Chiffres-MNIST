# Reconnaissance-Chiffres-MNIST
Ce projet consiste à entraîner un réseau de neurones multicouche (MLP) pour reconnaître les chiffres manuscrits à partir du dataset MNIST. Il a été développé entièrement en Python, sans utiliser de frameworks de deep learning comme TensorFlow ou PyTorch, afin de mieux comprendre le fonctionnement interne des réseaux de neurones (forward pass, rétropropagation, etc.).

📌 Objectifs du projet
Implémenter un réseau de neurones simple (une couche cachée)

Entraîner ce réseau sur les images du dataset MNIST

Évaluer la précision du modèle et visualiser son évolution

Tester le modèle sur des images externes dessinées par l’utilisateur

📁 Contenu du projet
main.py : script principal contenant le code d’entraînement, de test et de visualisation

utils.py : fonctions utilitaires (chargement des données, affichage, vectorisation d’images, etc.)

img.png : image manuscrite à tester (à dessiner et importer manuellement)

🧰 Bibliothèques utilisées
numpy : opérations numériques et matricielles

matplotlib.pyplot : visualisation des images et des résultats

idx2numpy : conversion des fichiers IDX du dataset MNIST

PIL (Pillow) : traitement d’image pour la prédiction externe

os : gestion des fichiers

⚙️ Fonctionnalités
Chargement et affichage de 36 images aléatoires du dataset

Vectorisation des labels en sortie attendue (one-hot)

Implémentation manuelle du forward pass et de la backpropagation

Suivi de la précision pendant l'entraînement

Test automatique du réseau sur des données inconnues

Prédiction d’une image externe dessinée à la main (fonction test_paint())

Préréquis pour utilisation
Le dataset MNIST doit être préalablement téléchargé et placé dans le bon dossier.

L’image utilisée dans test_paint() doit être en niveau de gris, 28x28 pixels, fond noir, écriture claire. Et pour utiliser votre image, veuillez remplacer le chemin d'accès par celui correspondant au chemin d'accès complet à votre image dans votre PC dans les lignes 192 et 197.

Le projet est conçu à des fins pédagogiques, pour comprendre les bases du deep learning sans utiliser de bibliothèques haut niveau.
