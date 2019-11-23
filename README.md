# EIP_SESSION_2
EIP session 2

# logs for epochs(20):

Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.002.
60000/60000 [==============================] - 13s 223us/step - loss: 0.6263 - acc: 0.8289 - val_loss: 0.1332 - val_acc: 0.9817
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0015163002.
60000/60000 [==============================] - 9s 145us/step - loss: 0.3123 - acc: 0.9074 - val_loss: 0.0802 - val_acc: 0.9865
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0012210012.
60000/60000 [==============================] - 8s 140us/step - loss: 0.2479 - acc: 0.9282 - val_loss: 0.0594 - val_acc: 0.9875
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0010219724.
60000/60000 [==============================] - 8s 132us/step - loss: 0.2117 - acc: 0.9381 - val_loss: 0.0471 - val_acc: 0.9910
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0008787346.
60000/60000 [==============================] - 8s 135us/step - loss: 0.1869 - acc: 0.9447 - val_loss: 0.0422 - val_acc: 0.9897
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0007707129.
60000/60000 [==============================] - 8s 138us/step - loss: 0.1706 - acc: 0.9475 - val_loss: 0.0345 - val_acc: 0.9922
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0006863418.
60000/60000 [==============================] - 8s 138us/step - loss: 0.1606 - acc: 0.9484 - val_loss: 0.0317 - val_acc: 0.9922
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0006186205.
60000/60000 [==============================] - 8s 140us/step - loss: 0.1494 - acc: 0.9512 - val_loss: 0.0297 - val_acc: 0.9929
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0005630631.
60000/60000 [==============================] - 8s 135us/step - loss: 0.1429 - acc: 0.9515 - val_loss: 0.0287 - val_acc: 0.9930
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0005166624.
60000/60000 [==============================] - 8s 137us/step - loss: 0.1363 - acc: 0.9522 - val_loss: 0.0259 - val_acc: 0.9938
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.000477327.
60000/60000 [==============================] - 8s 137us/step - loss: 0.1298 - acc: 0.9536 - val_loss: 0.0247 - val_acc: 0.9942
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.0004435573.
60000/60000 [==============================] - 8s 137us/step - loss: 0.1274 - acc: 0.9534 - val_loss: 0.0239 - val_acc: 0.9930
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0004142502.
60000/60000 [==============================] - 8s 141us/step - loss: 0.1215 - acc: 0.9551 - val_loss: 0.0228 - val_acc: 0.9937
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0003885759.
60000/60000 [==============================] - 8s 135us/step - loss: 0.1201 - acc: 0.9543 - val_loss: 0.0249 - val_acc: 0.9931
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0003658983.
60000/60000 [==============================] - 8s 133us/step - loss: 0.1169 - acc: 0.9555 - val_loss: 0.0232 - val_acc: 0.9940
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0003457217.
60000/60000 [==============================] - 8s 133us/step - loss: 0.1133 - acc: 0.9556 - val_loss: 0.0211 - val_acc: 0.9944
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000327654.
60000/60000 [==============================] - 9s 143us/step - loss: 0.1124 - acc: 0.9554 - val_loss: 0.0208 - val_acc: 0.9940
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.000311381.
60000/60000 [==============================] - 8s 137us/step - loss: 0.1099 - acc: 0.9561 - val_loss: 0.0214 - val_acc: 0.9945
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0002966479.
60000/60000 [==============================] - 8s 138us/step - loss: 0.1070 - acc: 0.9565 - val_loss: 0.0209 - val_acc: 0.9942
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000283246.
60000/60000 [==============================] - 8s 133us/step - loss: 0.1050 - acc: 0.9575 - val_loss: 0.0207 - val_acc: 0.9947
<keras.callbacks.History at 0x7f76fd4b4b70>




# score of model.evaluate on test data:
[0.020681965337414294, 0.9947]



# strategy:
To reduce the number of parameters I tried using kernels with less channels as the dataset is MNIST I tried using 14x14 filter rather than 16x16 which reduced my params.


Also I could see my model overfitting hence I tried a learning rate of 0.02 rather than 0.03, which helped me to acheive desired accuracy.
