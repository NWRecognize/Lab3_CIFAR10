# Lab3_CIFAR10
На основе ноутбука из предыдущего задания (с классификацией по CIFAR10), свернуть нейросеть, используя минимум два уровня свертывания.  
Слои модели:  
<pre>keras.layers.Conv2D(32, (3, 3), padding='same', activation='relu', input_shape=(32, 32, 3)),
    keras.layers.Conv2D(64, (3, 3), padding='same', activation='relu', input_shape=(32, 32, 3)),
    keras.layers.MaxPooling2D(pool_size=(2, 2), strides=2),
    keras.layers.Conv2D(64, (3, 3), padding='same', activation="relu", input_shape=(32, 32, 3)),
    keras.layers.Conv2D(128, (3, 3), padding='same', activation="relu", input_shape=(32, 32, 3)),
    keras.layers.MaxPooling2D(pool_size=(2, 2), strides=2),
    keras.layers.Conv2D(128, (3, 3), padding='same', activation="relu", input_shape=(32, 32, 3)),
    keras.layers.MaxPooling2D(pool_size=(2, 2), strides=2),
    keras.layers.Flatten(),
    keras.layers.Dense(128, activation='relu'),
    keras.layers.Dense(10, activation="softmax")</pre>
