# Amazon SageMaker

## Creation de compte

- Aller sur le site [amazon.com/console/](amazon.com/console/)
- Creer un compte puis se loger
- Sur le formfield de services mettre la recherche -sagemaker-
- A gauche les diffrents services rendu par sagemaker
- De la on oeut creer un -notebook instance-
- Modifier le nom, et changer -IAM Role- en creant un nouveau
- Choisir un -any s3 bucket-
- Le status sera en -pending- il faudra attendre que l'etat change avant de l'ouvrir
- Pour debuter il faut televerser le dataset. pour notre cas il s'agit de -diabeties.csv-
- Puis -conda python3 notebook-
- De la il est possible de creer un model de machine learning

## Exemple de code
```python
import pandas as pd
df = pd.read_csv('diabetes.csv')
df.head()#show the data
df.isnull().sum()
#supprimer la colonne Outcome
x = df.drop('Outcome',axis=1)
x.head()
y = df['Outcome']
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2)
from sklearn.ensemble import RandomForestClassifier
rfc = RandomForestClassifier()
rfc.fit(x_train,y_train)
rf_pred = rfc.predict(x_test)
from sklearn.metrics import accuracy_score
accuracy_score(y_test,rf_pred)
```

## Implementation pratique de SageMaker
pour cela il va falloir utiliser deux services aws :
- S3 : pour sauvegarder les donnees
- Amazon SageMaker : pour les algorithme d'apprentissage

Etape d'implementation:
### Creer un service S3

### Creer un service SageMaker
Cela se fait via la creation d'un notebook vu precedemment.



```
