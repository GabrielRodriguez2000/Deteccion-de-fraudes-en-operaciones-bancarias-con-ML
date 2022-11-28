### 1.	INTRODUCCIÓN
Uno de los problemas más sonados en el ámbito económico tiene que ver con los fraudes en operaciones comerciales, específicamente en el sector bancario existe un problema cuya solución es crucial y por esta razón se ofrecen puestos muy bien pagados a los profesionales científicos de datos.

Este problema es el de las operaciones bancarias fraudulentas, identificadas con movimientos inusuales de dinero, las causas de esto pueden ser muy variadas, van desde estafas hasta operaciones comerciales de grupos que se dedican a actividades sospechosas.

Para este trabajo se empleó como dataset el nombrado “Online Payments Fraud Detection Dataset” proveniente de la página Kaggle en la siguiente ubicación: https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset.
Este dataset contiene las columnas step, type, amount, nameOrig, oldbalanceOrg, newbalanceOrig, nameDest, oldbalanceDest, newbalanceDest, isFraud, isFlaggedFraud.

Este dataset lo que contiene es un registro de las operaciones bancarias realizadas por clientes de un banco, se tiene información como el tipo de operación realizada, la procedencia y el destino de la operación, el balance anterior y nuevo posterior a la operación tanto de la cuenta destino como de la cuenta origen, y finalmente, una bandera que indica si la operación es clasificada como fraudulenta o no.

### 2. Desarrollo

El dataset se encuentra desbalanceado, pues se encontró que la clase "es fraude" tan solo comprende un 0.129% de las muestras.

En este trabajo se emplearon las técnicas de aprendizaje K-Nearest Neighbors, Árboles de decisión y Regresión logística.   y como métricas de desempeño se utilizaron el coeficiente de correlación de Matthews, F1-Score y la curva ROC.          Adicionalmente, se empleó el Análisis de Componentes Principales, y se realizó reducción dimensional.

### 3. Conclusiones

Se encontró que la técnica con mejor desempeño fue árboles de decisión, utilizando métricas como Coeficiente de Correlación de Matthews, F1-Score y Curva ROC.    Estas fueron seleccionadas debido a que el conjunto de datos se encuentra desbalanceado y otras métricas como la precisión no toman en consideración este aspecto dando resultados muy positivos pero que no corresponden del todo con la realidad.