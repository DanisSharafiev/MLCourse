супер простая модель как отправная точка для сравнения моделей

``` python 
from sklearn.dummy import DummyClassifier  

dummy_clf = DummyClassifier(strategy="most_frequent")  
dummy_clf.fit(X_train, y_train)  
y_pred = dummy_clf.predict(X_test)  
```

``` python
from sklearn.dummy import DummyRegressor

dummy = DummyRegressor(strategy="mean")
dummy.fit(X_train, y_train)
y_pred = dummy.predict(X_test)
```

