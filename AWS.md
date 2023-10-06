# AWS

## C'est quoi AWS
AWS, ou Amazon Web Services, est une plateforme de cloud computing proposée par Amazon.com. Il s'agit d'une suite de services et d'outils informatiques à la demande qui permettent aux entreprises et aux individus de déployer et de gérer des applications, des sites web, des bases de données et d'autres ressources informatiques dans le cloud. AWS offre une grande variété de services, notamment le stockage, le calcul, la mise en réseau, la base de données, l'analyse, la sécurité, la gestion des conteneurs et bien d'autres encore.

Voici quelques-uns des services les plus couramment utilisés proposés par AWS :

1. Amazon EC2 (Elastic Compute Cloud) : Il s'agit d'un service d'infrastructure cloud qui permet de créer et de gérer des machines virtuelles (instances) pour exécuter des applications.

2. Amazon S3 (Simple Storage Service) : Il s'agit d'un service de stockage évolutif qui permet de stocker et de récupérer des données, que ce soit pour des sites web, des applications mobiles ou des sauvegardes.

3. Amazon RDS (Relational Database Service) : Il offre la possibilité de déployer et de gérer des bases de données relationnelles, telles que MySQL, PostgreSQL, Oracle et SQL Server.

4. Amazon Lambda : Il s'agit d'un service de calcul sans serveur qui permet d'exécuter du code en réponse à des événements sans avoir à gérer des serveurs.

5. Amazon VPC (Virtual Private Cloud) : Il offre une isolation réseau virtuelle pour les ressources AWS, permettant aux utilisateurs de créer des réseaux privés virtuels personnalisés dans le cloud.

6. AWS Elastic Beanstalk : Il permet de déployer et de gérer facilement des applications web dans le cloud, sans se soucier de l'infrastructure sous-jacente.

7. AWS CloudFormation : Il permet d'automatiser le déploiement et la gestion de l'infrastructure et des ressources AWS à l'aide de modèles.

8. AWS SNS (Simple Notification Service) : Il permet de gérer la diffusion de notifications par e-mail, SMS, ou d'autres moyens.

AWS est utilisé par de nombreuses entreprises du monde entier en raison de sa flexibilité, de sa fiabilité et de sa capacité à évoluer en fonction des besoins de l'entreprise. Il permet aux utilisateurs de payer uniquement pour les ressources qu'ils utilisent, ce qui en fait une option économique pour l'hébergement et la gestion d'applications et de services en ligne.


## Services de AWS
Amazon Web Services (AWS) propose une vaste gamme de services cloud couvrant divers domaines de l'informatique, de la gestion de données, de l'analyse, de l'Internet des objets (IoT), de la sécurité, de l'intelligence artificielle (IA), du machine learning (ML), et bien plus encore. Voici une liste des catégories de services AWS couramment utilisées, ainsi que quelques exemples de services dans chaque catégorie (veuillez noter que cette liste n'est pas exhaustive) :

1. **Services de calcul** :
   - Amazon EC2 (Elastic Compute Cloud) : Machines virtuelles évolutives.
   - AWS Lambda : Calcul sans serveur.
   - Amazon Elastic Container Service (ECS) : Gestion de conteneurs.

2. **Services de stockage** :
   - Amazon S3 (Simple Storage Service) : Stockage d'objets évolutif.
   - Amazon EBS (Elastic Block Store) : Stockage de blocs pour les instances EC2.
   - Amazon Glacier : Archivage de données à long terme.

3. **Services de bases de données** :
   - Amazon RDS (Relational Database Service) : Bases de données relationnelles gérées.
   - Amazon DynamoDB : Base de données NoSQL entièrement gérée.
   - Amazon Redshift : Data warehousing.

4. **Services de mise en réseau et de contenu** :
   - Amazon VPC (Virtual Private Cloud) : Réseau privé virtuel.
   - Amazon CloudFront : Service de distribution de contenu (CDN).
   - AWS Direct Connect : Connexions réseau dédiées à AWS.

5. **Services de sécurité et d'identité** :
   - AWS Identity and Access Management (IAM) : Gestion des identités et des autorisations.
   - AWS Key Management Service (KMS) : Gestion des clés de chiffrement.
   - Amazon GuardDuty : Service de détection de menaces.

6. **Services d'analyse et d'IA/ML** :
   - Amazon EMR (Elastic MapReduce) : Traitement et analyse de données.
   - Amazon SageMaker : Plateforme de machine learning.
   - Amazon Comprehend : Traitement automatique du langage naturel (NLP).

7. **Services de développement et de déploiement** :
   - AWS CodeDeploy : Déploiement d'applications.
   - AWS CodeBuild : Compilation de code.
   - AWS Elastic Beanstalk : Déploiement d'applications sans gestion d'infrastructure.

8. **Services IoT** :
   - AWS IoT Core : Gestion des objets connectés.
   - AWS IoT Analytics : Analyse des données IoT.

9. **Services de gestion et de surveillance** :
   - Amazon CloudWatch : Surveillance et gestion des ressources AWS.
   - AWS CloudTrail : Journalisation des activités AWS.
   - AWS Systems Manager : Gestion des instances EC2.

10. **Services de conteneurs et d'orchestration** :
    - Amazon EKS (Elastic Kubernetes Service) : Orchestration de conteneurs Kubernetes.
    - Amazon ECS (Elastic Container Service) : Orchestration de conteneurs.

Ces catégories et services AWS offrent une flexibilité et une évolutivité exceptionnelles pour répondre aux besoins des entreprises dans le cloud, que ce soit pour l'hébergement d'applications, la gestion de données, l'analyse, la sécurité, le développement ou d'autres cas d'utilisation. Les clients peuvent choisir et combiner ces services en fonction de leurs besoins spécifiques pour créer des solutions cloud personnalisées.
### Amazon SageMaker 
Amazon SageMaker est un service cloud proposé par Amazon Web Services (AWS) qui simplifie et accélère le processus de création, de formation et de déploiement de modèles d'apprentissage automatique (machine learning ou ML) pour les entreprises. Il est conçu pour permettre aux développeurs, aux scientifiques des données et aux ingénieurs d'effectuer plus facilement des tâches liées à l'IA et au ML sans avoir à se soucier des détails complexes de l'infrastructure sous-jacente. Voici une explication claire des principales fonctionnalités d'Amazon SageMaker :

1. **Construction de modèles ML** : SageMaker propose un environnement de développement intégré (IDE) basé sur Jupyter Notebook qui permet aux utilisateurs de créer, de prototyper et de tester leurs modèles ML en utilisant des langages de programmation courants tels que Python.

2. **Formation de modèles** : SageMaker facilite la formation des modèles ML en utilisant des instances d'apprentissage préconfigurées. Il prend en charge une variété de frameworks ML, notamment TensorFlow, PyTorch, scikit-learn, et XGBoost. Les utilisateurs peuvent également accéder à des ensembles de données préparés pour l'apprentissage.

3. **Optimisation automatique** : Le service propose des fonctionnalités d'optimisation automatique des modèles (AutoML) qui permettent de rechercher automatiquement les hyperparamètres optimaux pour améliorer les performances du modèle.

4. **Déploiement de modèles** : Une fois que le modèle ML est entraîné, SageMaker permet de le déployer facilement en tant qu'API RESTful ou en tant qu'application web hébergée. Cela permet aux développeurs d'intégrer facilement des modèles ML dans leurs applications.

5. **Gestion des modèles** : SageMaker offre des outils pour gérer, surveiller et suivre les modèles déployés, y compris la détection des dégradations de performances afin de garantir que les modèles fonctionnent correctement dans des environnements de production.

6. **Évolutivité et facilité d'utilisation** : Amazon SageMaker gère automatiquement les ressources sous-jacentes, ce qui permet aux utilisateurs de se concentrer sur le développement de modèles plutôt que sur la gestion de l'infrastructure. Il peut également s'intégrer facilement à d'autres services AWS pour tirer parti de la puissance du cloud.

7. **Sécurité et conformité** : SageMaker propose des fonctionnalités de sécurité avancées, telles que le chiffrement des données en transit et au repos, ainsi que l'accès basé sur les rôles pour contrôler qui peut accéder aux ressources.

En résumé, Amazon SageMaker est un service de machine learning entièrement géré qui simplifie l'ensemble du processus de développement, de formation, de déploiement et de gestion des modèles ML. Il permet aux organisations de tirer parti de l'apprentissage automatique pour résoudre des problèmes complexes sans nécessiter une expertise approfondie en infrastructure ou en apprentissage automatique.

### Exemple
Bien sûr ! Voici un exemple concret de mise en œuvre d'Amazon SageMaker pour créer, former et déployer un modèle d'apprentissage automatique :

**Exemple : Prédiction de la fraude de cartes de crédit**

Supposons que vous travaillez pour une société de cartes de crédit et que vous souhaitez développer un modèle de machine learning pour détecter les transactions frauduleuses. Voici comment vous pourriez utiliser Amazon SageMaker pour réaliser cette tâche :

1. **Collecte de données** : Tout d'abord, vous collectez un ensemble de données historiques de transactions de cartes de crédit, comprenant à la fois des transactions légitimes et frauduleuses. Ces données contiennent des informations telles que le montant de la transaction, la date, l'heure, la localisation, etc.

2. **Préparation des données** : Vous préparez les données en effectuant des opérations de nettoyage, de transformation et de normalisation. Vous divisez également les données en ensembles d'entraînement et de test.

3. **Création du modèle** : Vous utilisez Amazon SageMaker Studio pour créer un environnement de développement Jupyter Notebook. Dans ce notebook, vous développez et expérimentez différents modèles de machine learning, tels que des modèles d'arbres de décision, de forêts aléatoires ou de réseaux de neurones, en utilisant des bibliothèques comme scikit-learn ou TensorFlow.

4. **Formation du modèle** : Une fois que vous avez sélectionné le modèle le plus prometteur, vous utilisez SageMaker pour former ce modèle en utilisant l'ensemble d'entraînement. SageMaker gère automatiquement la mise à l'échelle et la distribution du calcul pour la formation.

5. **Optimisation du modèle** : Vous pouvez utiliser la fonctionnalité d'optimisation automatique de SageMaker pour rechercher les meilleurs hyperparamètres du modèle, ce qui peut améliorer ses performances.

6. **Déploiement du modèle** : Après avoir entraîné le modèle, vous pouvez le déployer facilement en tant qu'API RESTful à l'aide de SageMaker Endpoints. Cette API peut être intégrée à votre système de gestion des transactions pour évaluer la fraude en temps réel.

7. **Surveillance et maintenance** : Vous utilisez SageMaker Model Monitor pour surveiller les performances du modèle en production. Si les performances se dégradent ou si de nouvelles données sont collectées, vous pouvez réentraîner le modèle pour le maintenir à jour.

8. **Évolutivité** : Si votre volume de transactions augmente, SageMaker vous permet de redimensionner automatiquement les ressources de calcul pour répondre à la demande croissante.

9. **Sécurité** : Vous utilisez les fonctionnalités de sécurité de SageMaker pour protéger les données et le modèle, y compris le chiffrement des données et la gestion des accès.

Dans cet exemple, Amazon SageMaker simplifie l'ensemble du cycle de vie du modèle ML, de la préparation des données à la mise en production, en passant par la formation et la maintenance. Il vous permet de développer rapidement et efficacement un modèle de détection de fraude de cartes de crédit tout en gérant les aspects techniques complexes de l'apprentissage automatique.
 
