Dans ce projet, je travaillais pour une entreprise appelée **Place de Marché**, qui souhaitait lancer un marketplace e-commerce.

Au moment du projet, une plateforme de vente était déjà en place, dans laquelle les vendeurs remplissaient manuellement les informations du produits, et peu de produits étaient proposés. Dans un souci de fiabilité 
et de simplicité pour l'utilisateur, l'entreprise souhaitait mettre en place une automatisation de la catégorisation des produits.

La première partie de ce projet consistait donc à vérifier la faisabilité de cette tâche, à travers les features textuelles (Nom du produit, description fournie par l'utilisateur) et les features images (photos du produits
fournies par l'utilisateur). Pour analyser ces différentes features, j'ai donc effectué un pré-traitement, une extraction de features à l'aide de divers modèles et une réduction de dimension, afin d'évaluer graphiquement 
les résultats, puis une comparaison à l'aide d'un kmeans pour chiffrer réellement la performance de notre modèle.

Le procédé était le même pour les textes et les images, en utilisant évidemment des méthodes et modèles différents. Pour les features textuelles, j'ai notamment mis en place des approches simple telles qu'un bag of words,
jusqu'à des modèles plus complexes de réseau de neurones tels que Word2Vec ou USE. Concernant les features images, j'ai principalement travaillé avec des modèles de Transfer Learning comme vgg16, mais aussi avec des
descripteurs SIFT pour comparer les performances.

Après avoir réalisé cette étude et déduit de la faisabilité de notre projet, j'ai réemployé le modèle le plus efficace que j'ai trouvé auparavant pour effectuer une classification supervisée directement sur les features
images. J'ai également mis en place une data augmentation sur le dataset d'entraînement afin d'améliorer au mieux l'optimisation du modèle.

Enfin, dans un but d'élargissement de la gamme de produits sur le site, j'ai crée un rapide appel vers une API contenant une base de données sur des produits de consommation afin de tester son utilisation.
