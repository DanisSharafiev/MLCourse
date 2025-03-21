Фильтрационные методы
``` python
from sklearn.feature_selection import SelectKBest, f_classif

X_new = SelectKBest(f_classif, k=5).fit_transform(X, y) 
```

Обёрточные методы
``` python
from sklearn.feature_selection import RFE
from sklearn.ensemble import RandomForestClassifier

model = RandomForestClassifier()
selector = RFE(model, n_features_to_select=5)
X_new = selector.fit_transform(X, y)
```

Embedded Methods
``` python
from sklearn.linear_model import Lasso

model = Lasso(alpha=0.01)  
model.fit(X, y)
important_features = X.columns[model.coef_ != 0] 
```














