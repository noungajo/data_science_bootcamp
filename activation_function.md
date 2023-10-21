# Fonction d'activation
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

