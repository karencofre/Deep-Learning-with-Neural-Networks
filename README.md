# Red Neuronal con keras - Deep Learning

Ficha Técnica: Proyecto de Análisis de Datos Predictivo

Título del Proyecto: Deep Learning con Redes Neuronales

Objetivo:
Construir una red neuronal.

Equipo:
Trabajo Grupal.

Herramientas y Tecnologías:
- Python
- sklearn
- tensorflow
- Google Colab

Procesamiento y análisis:
- limpieza de datos
- exploración de datos
- consultas SQL
- Técnica de Análisis de datos
  
Resultados y Conclusiones:
se realizo una red neuronal secuencial con keras.

Red Neuronal:

```python

model = Sequential()
model.add(Embedding(input_dim=max_words, output_dim=32, input_length=max_length))
model.add(LSTM(100))
model.add(Dense(1, activation='sigmoid'))

# Compilar el modelo
model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])

# Entrenar el modelo
model.fit(X_train, y_train, epochs=5, batch_size=32, validation_split=0.2)

# Evaluar el modelo en el conjunto de prueba
accuracy = model.evaluate(X_test, y_test)[1]
print(f'Accuracy on test set: {accuracy}')
```



Limitaciones/Próximos Pasos:
Identifica y describe cualquier limitación o desafío encontrado durante el proyecto.
Sugiere posibles próximos pasos para extender o mejorar el proyecto de análisis de datos.


