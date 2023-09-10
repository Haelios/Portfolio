Pour ce projet, je travaillais pour une startup de l'agro-alimentaire, qui souhaite proposer des solutions innovantes pour la récolte de fruits. Dans ce projet, afin de sensibiliser à la biodiversité fruitière,
l'intérêt était de mettre en place une application permettant à l'utilisateur d'identifier et d'obtenir des informations sur un fruit dont il fournirait une photo.

L'objectif du projet était donc de mettre en place un environnement Big Data, car le volume des images va rapidement augmenter avec l'utilisation de l'application, permettant le traitement des images avec 
un script en PySpark afin de traiter ce volume important de données grâce au calcul distribué. Le dataset de base se nomme Fruits 360 et contient des photos de plus de 130 variétés de fruits et légumes.

J'ai utilisé pour ce projet un échantillon de quelques images afin de limiter les coûts lors de la mise en place. J'ai fait appel à un bucket S3 afin de stocker les différents fichiers du projet, puis j'ai crée une instance
EMR qui utilise les fichiers présents dans le Bucket. Le notebook contenant le script en PySpark est ensuite lancé via le cluster afin de traiter les images, à l'aide d'un modèle de Transfer Learning.
Suite au traitement des images par ce modèle, j'ai également procédé à une reduction de dimension avec un PCA en Spark.
