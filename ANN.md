# Réseaux de neurones artificiels
Les réseaux de neurones artificiels, également appelés réseaux de neurones profonds ou réseaux neuronaux profonds (DNN), sont un type de modèle d'apprentissage automatique inspiré du fonctionnement du cerveau humain.
Ils sont utilisés pour résoudre des problèmes complexes de classification, de prédiction, de traitement du langage naturel, de vision par ordinateur et bien d'autres. Voici une explication claire des réseaux de neurones artificiels :

1. **Neurones artificiels :** Les neurones artificiels sont les unités de base des réseaux de neurones. Chaque neurone prend un ensemble de valeurs en entrée, effectue un calcul, puis produit une valeur en sortie. 
Ces neurones sont connectés les uns aux autres pour former un réseau.
2. **Architecture du réseau :** Les réseaux de neurones sont organisés en couches. Il y a généralement trois types de couches :
   - **Couche d'entrée :** Cette couche reçoit les données brutes en entrée, par exemple des images, des textes, des chiffres, etc.
   - **Couches cachées :** Ces couches intermédiaires effectuent des calculs complexes. Les réseaux de neurones profonds ont plusieurs de ces couches, d'où le terme "profonds".
   - **Couche de sortie :** Cette couche produit la sortie du réseau, qui peut être une classification, une valeur numérique, une séquence de texte, etc., en fonction du type de problème que le réseau résout.

3. **Connexions pondérées :** Chaque connexion entre les neurones a un poids. Ces poids contrôlent l'importance de l'entrée pour le neurone. Les poids sont appris pendant l'entraînement du réseau pour optimiser les performances.

4. **Fonction d'activation :** Chaque neurone utilise une fonction d'activation pour transformer sa somme pondérée d'entrées en une sortie.
 Des fonctions courantes incluent la fonction sigmoïde(), la fonction ReLU (Rectified Linear Unit), et la fonction tangente hyperbolique (tanh).

5. **Propagation avant :** Lorsque des données sont introduites dans le réseau, elles se propagent de couche en couche, avec des calculs et des transformations successives. La couche d'entrée ne fait que recevoir les données, tandis que les couches cachées extraient des caractéristiques importantes.

6. **Apprentissage :** Les réseaux de neurones apprennent à partir de données d'entraînement. Ils ajustent les poids de manière itérative pour minimiser l'erreur entre les prédictions du réseau et les valeurs attendues. Ceci est généralement réalisé à l'aide d'algorithmes d'optimisation tels que la descente de gradient.

7. **Fonction de perte :** Pour évaluer les performances du réseau pendant l'entraînement, une fonction de perte est utilisée pour mesurer la différence entre les prédictions du réseau et les véritables valeurs cibles. L'objectif est de minimiser cette perte.

8. **Réseaux profonds :** Les réseaux de neurones profonds sont capables de capturer des modèles complexes grâce à leurs multiples couches cachées. Cependant, ils nécessitent souvent de grandes quantités de données d'entraînement et de puissance de calcul pour obtenir de bons résultats.

9. **Utilisation :** Les réseaux de neurones artificiels sont utilisés dans de nombreuses applications, telles que la vision par ordinateur, la reconnaissance vocale, la traduction automatique, la recommandation de contenu, la médecine, la finance, et bien plus encore.

## Pourquoi utiliser une fonctin d'activation?
La fonction d'activation est une composante essentielle des réseaux de neurones artificiels. Elle est utilisée pour introduire de la non-linéarité dans le modèle, ce qui permet au réseau de capturer des modèles et des relations complexes dans les données. Voici pourquoi on utilise une fonction d'activation dans les réseaux de neurones :

1. **Introduction de la non-linéarité :** Sans fonction d'activation, un réseau de neurones serait essentiellement une combinaison linéaire de ses entrées pondérées par les poids. Cela signifie que le réseau ne serait capable de modéliser que des relations linéaires simples entre les données. En introduisant des fonctions d'activation non linéaires, le réseau peut apprendre des relations non linéaires dans les données, ce qui est souvent crucial pour des tâches complexes comme la reconnaissance d'images ou la compréhension du langage naturel.

2. **Capacité à apprendre des représentations hiérarchiques :** Les fonctions d'activation permettent aux réseaux de neurones de créer des représentations hiérarchiques des données. Cela signifie que les couches supérieures du réseau peuvent apprendre des caractéristiques abstraites basées sur les caractéristiques apprises dans les couches inférieures. Par exemple, dans une tâche de vision par ordinateur, les premières couches peuvent apprendre des bords, les couches intermédiaires des formes, et les couches supérieures des objets complets.

3. **Non-linéarités complexes :** Différentes fonctions d'activation introduisent différentes non-linéarités. Par exemple, la fonction ReLU (Rectified Linear Unit) est une non-linéarité simple qui devient linéaire pour des valeurs positives et 0 pour des valeurs négatives. La fonction sigmoïde est une non-linéarité en forme de S qui comprime les valeurs entre 0 et 1. Ces non-linéarités complexes permettent au réseau de modéliser une grande variété de relations dans les données.

4. **Résolution du problème de classification :** Les fonctions d'activation sont essentielles dans les couches de sortie des réseaux de neurones pour des tâches de classification. Elles convertissent les scores bruts en probabilités ou en catégories de classe, en utilisant des fonctions telles que la fonction softmax pour la classification multiclasse.

5. **Éviter la saturation :** Les fonctions d'activation aident à éviter la saturation des neurones, ce qui se produit lorsque les valeurs d'entrée sont trop grandes ou trop petites, ce qui peut entraîner un ralentissement de l'apprentissage. Les fonctions d'activation introduisent une saturation limitée, ce qui permet au réseau de continuer à apprendre efficacement.

En résumé, les fonctions d'activation dans les réseaux de neurones introduisent de la non-linéarité, permettant ainsi au réseau de capturer des modèles complexes dans les données. Elles sont un élément clé pour la flexibilité et la puissance des réseaux de neurones dans diverses tâches d'apprentissage automatique.
### Fonction sïgmoid
La fonction sigmoïde est l'une des fonctions d'activation classiques utilisées dans les réseaux de neurones. Elle a été largement utilisée dans les premiers jours de l'apprentissage automatique et des réseaux de neurones, bien qu'elle ait été en grande partie remplacée par des fonctions d'activation plus efficaces comme ReLU (Rectified Linear Unit) dans de nombreux cas. Cependant, la fonction sigmoïde a encore des applications et des particularités qui la rendent pertinente dans certains contextes. Voici pourquoi la fonction sigmoïde est utilisée et quelles sont ses particularités :

1. **Transformation des valeurs en un intervalle restreint :** La fonction sigmoïde transforme les valeurs d'entrée en un intervalle compris entre 0 et 1. Cela peut être utile dans des contextes où l'on souhaite modéliser des probabilités, car les valeurs dans cet intervalle peuvent être interprétées comme des probabilités.

2. **Utilisation dans les couches de sortie :** La fonction sigmoïde est souvent utilisée dans les couches de sortie des réseaux de neurones pour des tâches de classification binaire, où le but est de déterminer si quelque chose est vrai ou faux, oui ou non. La sortie de la fonction sigmoïde peut être interprétée comme la probabilité d'appartenir à la classe positive.

3. **Dérivée simple :** La dérivée de la fonction sigmoïde est relativement simple à calculer. Cela peut être avantageux lors de l'entraînement de réseaux de neurones, car il est nécessaire de calculer des dérivées pour mettre à jour les poids. Cependant, la simplicité de la dérivée n'est pas toujours un avantage significatif par rapport à d'autres fonctions d'activation comme ReLU.

4. **Utilisation dans des réseaux récurrents :** La fonction sigmoïde est parfois utilisée dans des réseaux de neurones récurrents (RNN) pour modéliser des séquences de données, car elle peut aider à modéliser des états cachés qui évoluent avec le temps.

Cependant, la fonction sigmoïde présente également des inconvénients, notamment le problème de la disparition du gradient, où la dérivée de la fonction sigmoïde devient très proche de zéro pour des valeurs d'entrée très élevées ou très basses. Cela peut entraîner des difficultés lors de l'apprentissage de réseaux profonds, car le gradient peut devenir trop petit pour entraîner efficacement le réseau. Pour cette raison, la fonction ReLU est souvent préférée, car elle atténue le problème de la disparition du gradient.
### La fonction tangente hyperbolique
La fonction tangente hyperbolique, souvent abrégée sous le nom de "tanh," est une autre fonction d'activation couramment utilisée dans les réseaux de neurones. Elle partage certaines caractéristiques avec la fonction sigmoïde, mais elle a aussi des particularités qui la rendent pertinente dans certains contextes. Voici pourquoi la fonction tanh est utilisée et quelles sont ses particularités :

1. **Transformation des valeurs en un intervalle restreint :** Tout comme la fonction sigmoïde, la fonction tanh transforme les valeurs d'entrée en un intervalle restreint, mais dans le cas de la tanh, cet intervalle est [-1, 1]. Cela peut être utile lorsque vous souhaitez normaliser les données ou modéliser des sorties avec des valeurs positives et négatives.

2. **Ressemblance à une fonction linéaire centrée :** La fonction tanh ressemble à une fonction linéaire centrée autour de zéro. Cela signifie qu'elle peut être plus appropriée pour modéliser des données dont les valeurs sont centrées autour de zéro. Elle est souvent utilisée dans des contextes où la normalisation des données est importante.

3. **Dérivée simple :** La dérivée de la fonction tanh est également relativement simple à calculer. Cela peut être un avantage lors de l'entraînement de réseaux de neurones, car le calcul des dérivées est nécessaire pour mettre à jour les poids du réseau.

4. **Réduction du problème de la disparition du gradient :** Bien que la fonction tanh souffre également du problème de la disparition du gradient pour des valeurs d'entrée très élevées ou très basses, ce problème est atténué par rapport à la fonction sigmoïde, car la tangente hyperbolique est centrée autour de zéro, ce qui signifie que la dérivée est plus éloignée de zéro dans la plage de sortie.

Cependant, la fonction tanh a également des inconvénients, notamment la sensibilité aux valeurs d'entrée extrêmes, qui peuvent causer des problèmes de saturation et de disparition du gradient. Elle n'est pas aussi largement utilisée que la fonction ReLU (Rectified Linear Unit) dans les réseaux de neurones modernes, car ReLU a tendance à offrir de meilleures performances et à surmonter certains des inconvénients de la tanh.
### La fonction ReLU (Rectified Linear Unit)
La fonction ReLU (Rectified Linear Unit) est une fonction d'activation largement utilisée dans les réseaux de neurones modernes en raison de ses nombreuses particularités et avantages. Voici pourquoi la fonction ReLU est populaire et quelles sont ses caractéristiques clés :

1. **Non-linéarité :** La fonction ReLU est une fonction non linéaire qui introduit de la non-linéarité dans les réseaux de neurones. Cela permet au réseau de capturer des modèles complexes et de représenter des relations non linéaires dans les données.

2. **Simplicité :** La fonction ReLU est très simple à calculer. Elle est définie comme f(x) = max(0, x), ce qui signifie que si l'entrée est positive, la sortie est égale à l'entrée, et si l'entrée est négative, la sortie est 0. Cette simplicité de calcul permet aux réseaux de neurones de s'entraîner plus rapidement.

3. **Réduction du problème de la disparition du gradient :** Contrairement à la fonction sigmoïde et à la fonction tanh, la fonction ReLU ne souffre pas du problème de la disparition du gradient pour des valeurs d'entrée positives. Lorsque l'entrée est positive, la dérivée de la fonction ReLU est 1, ce qui permet de propager efficacement le gradient à travers le réseau.

4. **Sparsité :** La fonction ReLU introduit une certaine sparsité dans les activations du réseau. Si l'entrée d'un neurone est négative, l'activation est nulle, ce qui signifie que le neurone ne contribue pas à la sortie. Cela peut avoir des avantages en termes de réduction de la surapprentissage (overfitting) et de complexité du modèle.

5. **Efficacité :** La fonction ReLU est très efficace en termes de calcul, ce qui la rend adaptée aux réseaux de neurones profonds qui nécessitent un grand nombre de calculs. Elle a contribué à l'essor de l'apprentissage profond (deep learning) en permettant l'entraînement de réseaux de neurones profonds de manière plus efficace.

Cependant, il est important de noter que la fonction ReLU a également des inconvénients, notamment le problème de la "mort des neurones" (dying ReLU), où un neurone peut rester inactif pour des valeurs d'entrée négatives, ne contribuant donc pas à l'apprentissage. Pour surmonter ce problème, des variantes de la fonction ReLU ont été proposées, comme Leaky ReLU, Parametric ReLU, et Exponential Linear Unit (ELU), qui atténuent le problème de la "mort des neurones" en permettant une activation partielle pour les valeurs négatives.

## Un optimiseur
Un optimiseur, en termes simples, est un outil mathématique utilisé pour aider un algorithme d'apprentissage automatique, comme un réseau de neurones, à ajuster ses paramètres (comme les poids des connexions entre les neurones) de manière à minimiser une erreur ou une fonction de perte, c'est-à-dire à rendre les prédictions du modèle plus précises.

Pour illustrer cela, imaginez un modèle d'apprentissage automatique qui essaie d'apprendre à reconnaître des chiffres manuscrits. Au début, il fait des prédictions incorrectes. L'optimiseur est l'outil qui guide le processus d'ajustement des paramètres du modèle pour rendre ses prédictions plus proches des chiffres réels. L'optimiseur cherche à "optimiser" ou à "améliorer" les performances du modèle en ajustant ses paramètres de manière itérative.
### La descente de gradient
Imaginez que vous êtes au sommet d'une colline, mais vous ne savez pas où se trouve le point le plus bas. Vous voulez descendre le plus bas possible en prenant de petits pas, mais vous ne pouvez sentir que le terrain sous vos pieds pour savoir dans quelle direction aller. Vous faites un petit pas dans la direction où le terrain semble le plus bas à cet endroit précis.

C'est un peu comme ça que fonctionne la descente de gradient dans l'apprentissage automatique. L'idée est de trouver le point le plus bas (le minimum) d'une fonction mathématique (qui mesure l'erreur du modèle) en ajustant les paramètres du modèle de manière itérative.

Voici comment cela fonctionne :
1. Vous commencez avec des paramètres de modèle initiaux.
2. Vous calculez la pente (ou le gradient) de la fonction par rapport à ces paramètres à cet endroit.
3. Vous déplacez les paramètres dans la direction où la pente est la plus raide, mais en prenant de petits pas (le taux d'apprentissage).
4. Vous répétez ce processus jusqu'à ce que vous trouviez un point où la pente est presque plate, ce qui signifie que vous êtes arrivé à un minimum.

Cela permet au modèle d'apprendre à partir des données, d'ajuster ses paramètres pour minimiser l'erreur et de devenir plus précis dans ses prédictions. La descente de gradient est un concept fondamental de l'entraînement des modèles d'apprentissage automatique.
La descente de gradient est une technique essentielle dans l'entraînement des modèles d'apprentissage automatique, mais elle présente à la fois des avantages et des inconvénients. Voici une liste des principaux avantages et inconvénients de la descente de gradient :

**Avantages de la descente de gradient :**

1. **Optimisation efficace :** La descente de gradient est un algorithme efficace pour trouver les paramètres d'un modèle qui minimisent une fonction de coût, ce qui permet d'entraîner des modèles d'apprentissage automatique.

2. **Adaptabilité :** La descente de gradient peut être utilisée pour optimiser une grande variété de fonctions de coût, ce qui la rend très polyvalente.

3. **Évolutivité :** Elle peut être appliquée à des problèmes de grande dimension, avec un grand nombre de paramètres, tels que les réseaux de neurones profonds.

4. **Itératif :** La descente de gradient fonctionne par des mises à jour itératives des paramètres du modèle, ce qui lui permet d'apprendre progressivement à partir des données.

5. **Stabilité numérique :** Elle est numériquement stable et permet de trouver des solutions précises dans des environnements numériques.

**Inconvénients de la descente de gradient :**

1. **Sensibilité au taux d'apprentissage :** Le choix du taux d'apprentissage est crucial, car un taux d'apprentissage inapproprié peut entraîner une convergence lente ou une divergence de l'algorithme.

2. **Sensibilité à l'initialisation :** Les performances de la descente de gradient dépendent souvent des valeurs initiales des paramètres du modèle.

3. **Possibilité de rester bloqué dans un minimum local :** La descente de gradient peut converger vers un minimum local de la fonction de coût, ce qui peut ne pas être le minimum global. Cela dépend de la forme de la fonction de coût.

4. **Temps de calcul :** Pour de grands ensembles de données et des modèles complexes, la descente de gradient peut être computationnellement coûteuse.

5. **Problème de la disparition du gradient :** Dans les réseaux de neurones profonds, la descente de gradient peut souffrir du problème de la disparition du gradient, où les gradients deviennent très petits, rendant l'apprentissage difficile.

6. **Variétés non convexes :** Dans certains cas, la fonction de coût peut avoir des surfaces non convexes, ce qui peut rendre la convergence vers un minimum difficile.

Malgré ces inconvénients, la descente de gradient est largement utilisée et est la base de nombreuses techniques d'optimisation plus avancées. Des variantes de la descente de gradient, telles que la descente de gradient stochastique (SGD) et d'autres méthodes d'optimisation, ont été développées pour atténuer certains de ces inconvénients.
### La descente de gradient stochastique (SGD) 
La descente de gradient stochastique (SGD, pour Stochastic Gradient Descent) est une variante de l'algorithme de descente de gradient standard utilisée pour entraîner des modèles d'apprentissage automatique, tels que les réseaux de neurones. La principale différence entre le SGD et la descente de gradient standard réside dans la manière dont les mises à jour des paramètres du modèle sont effectuées. Voici une explication de la descente de gradient stochastique :

1. **Échantillonnage stochastique :** Contrairement à la descente de gradient standard, qui calcule la mise à jour des paramètres en utilisant l'ensemble complet des données d'entraînement, le SGD effectue des mises à jour en utilisant un seul exemple (ou un petit échantillon, appelé mini-lot) à la fois. Cette approche rend le processus plus stochastique, c'est-à-dire qu'il comporte une part d'aléatoire.

2. **Calcul du gradient partiel :** Pour chaque exemple d'entraînement, le SGD calcule le gradient partiel de la fonction de coût par rapport aux paramètres du modèle. Le gradient partiel est une estimation de la direction dans laquelle les paramètres doivent être ajustés pour minimiser la fonction de coût en fonction de cet exemple spécifique.

3. **Mise à jour des paramètres :** Après avoir calculé le gradient partiel, le SGD ajuste immédiatement les paramètres du modèle en se déplaçant dans la direction opposée du gradient. Cela signifie que si le gradient est positif, les paramètres sont réduits, et s'il est négatif, les paramètres sont augmentés.

4. **Répétition :** Ces étapes sont répétées pour chaque exemple dans l'ensemble d'entraînement, et cela constitue une itération. Une itération complète à travers tout l'ensemble d'entraînement est souvent appelée une "époque". Le processus d'entraînement se poursuit pendant plusieurs époques, avec des mises à jour de paramètres à chaque itération.

**Avantages du SGD :**
- Le SGD est plus rapide et nécessite moins de mémoire que la descente de gradient standard, car il ne nécessite que la manipulation d'un seul exemple (ou mini-lot) à la fois.
- Il peut être utilisé pour l'entraînement en ligne, ce qui signifie que les modèles peuvent s'ajuster aux nouvelles données au fur et à mesure qu'elles arrivent.

**Inconvénients du SGD :**
- Le SGD est plus bruité en raison de son échantillonnage stochastique, ce qui peut le rendre moins stable et nécessite parfois un taux d'apprentissage adaptatif.
- Il peut prendre plus de temps pour converger vers une solution optimale par rapport à la descente de gradient standard, car il effectue des mises à jour plus fréquentes.

Le SGD est largement utilisé dans l'entraînement des modèles d'apprentissage automatique en raison de sa capacité à gérer des ensembles de données volumineux et de sa flexibilité. Il est souvent utilisé en combinaison avec des taux d'apprentissage adaptatifs pour obtenir de meilleurs résultats.
### Adam
Adam est un algorithme d'optimisation couramment utilisé dans l'entraînement des modèles d'apprentissage automatique, en particulier dans le contexte des réseaux de neurones profonds. Le nom "Adam" est une abréviation de "Adaptive Moment Estimation," ce qui reflète le fait que l'algorithme utilise des estimations adaptatives des moments du gradient. Voici comment fonctionne l'optimiseur Adam :

1. **Momentum :** Adam utilise un concept appelé "momentum," qui est une technique d'accélération de la descente de gradient. Le momentum permet de maintenir l'élan lors de la mise à jour des paramètres du modèle. Il accumule un terme exponentiellement décroissant du gradient précédent.

2. **Adaptation du taux d'apprentissage :** Adam adapte automatiquement le taux d'apprentissage pour chaque paramètre du modèle. Cela signifie qu'il utilise un taux d'apprentissage différent pour chaque paramètre, en fonction de son histoire récente de mises à jour. Les paramètres qui ont reçu des mises à jour plus importantes auront un taux d'apprentissage réduit, tandis que les paramètres qui ont reçu des mises à jour moins importantes auront un taux d'apprentissage plus élevé.

3. **Correction des biais :** Pour corriger les biais introduits par l'initialisation des moments (momentum) à zéro, Adam effectue une étape de correction. Cela garantit que les moments sont correctement estimés, en particulier au début de l'entraînement.

4. **Paramètres :** Adam utilise deux paramètres principaux, bêta_1 (habituellement proche de 0.9) et bêta_2 (habituellement proche de 0.999), qui contrôlent le taux d'oubli des moments précédents et du carré du gradient, respectivement. Il utilise également un petit terme d'évitement numérique pour éviter la division par zéro.

5. **Avantages :** Adam est efficace pour l'entraînement de réseaux de neurones profonds, car il est capable de gérer des taux d'apprentissage adaptatifs pour différents paramètres, ce qui accélère la convergence. Il est également peu sensible aux problèmes de l'initialisation des paramètres et peut fonctionner efficacement avec un taux d'apprentissage initial relativement élevé.

6. **Inconvénients :** Adam peut être plus lent que d'autres optimiseurs tels que la descente de gradient stochastique (SGD) sans momentum pour des petits ensembles de données. En outre, il peut être sensible au choix des hyperparamètres tels que les taux d'apprentissage.


