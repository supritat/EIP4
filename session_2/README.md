
* Strategy to  achieve the following result:
  1. Changed the number of kernels (to 16)so that total number of parameters are within 15k.
  2. Inclded BatchNormalization after each convoluted layer.
  3. Included Dropout after BatchNormalization to reduce the gap between taraining and test accuracy.
  4. Train the model until we reach mentioned (99.4%) accuracy within 20 epochs.

* Result of model.evaluate (on test data) = [0.0362217591198546, 0.993]

* Logs for 20 epochs:

Train on 60000 samples, validate on 10000 samples
Epoch 1/20
 2560/60000 [>.............................] - ETA: 4s - loss: 6.1790e-04 - acc: 1.0000/usr/local/lib/python3.6/dist-packages/ipykernel_launcher.py:1: UserWarning: The `nb_epoch` argument in `fit` has been renamed `epochs`.
  """Entry point for launching an IPython kernel.
60000/60000 [==============================] - 3s 53us/step - loss: 0.0024 - acc: 0.9991 - val_loss: 0.0335 - val_acc: 0.9927
Epoch 2/20
60000/60000 [==============================] - 3s 51us/step - loss: 0.0037 - acc: 0.9987 - val_loss: 0.0319 - val_acc: 0.9935
Epoch 3/20
60000/60000 [==============================] - 3s 52us/step - loss: 0.0031 - acc: 0.9989 - val_loss: 0.0351 - val_acc: 0.9935
Epoch 4/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0029 - acc: 0.9988 - val_loss: 0.0293 - val_acc: 0.9938
Epoch 5/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0032 - acc: 0.9989 - val_loss: 0.0323 - val_acc: 0.9934
Epoch 6/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0035 - acc: 0.9987 - val_loss: 0.0293 - val_acc: 0.9939
Epoch 7/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0044 - acc: 0.9986 - val_loss: 0.0305 - val_acc: 0.9932
Epoch 8/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0036 - acc: 0.9989 - val_loss: 0.0303 - val_acc: 0.9941
Epoch 9/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0029 - acc: 0.9989 - val_loss: 0.0300 - val_acc: 0.9940
Epoch 10/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0033 - acc: 0.9988 - val_loss: 0.0359 - val_acc: 0.9933
Epoch 11/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0034 - acc: 0.9987 - val_loss: 0.0368 - val_acc: 0.9929
Epoch 12/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0037 - acc: 0.9988 - val_loss: 0.0346 - val_acc: 0.9934
Epoch 13/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0032 - acc: 0.9989 - val_loss: 0.0343 - val_acc: 0.9929
Epoch 14/20
60000/60000 [==============================] - 3s 52us/step - loss: 0.0033 - acc: 0.9989 - val_loss: 0.0284 - val_acc: 0.9937
Epoch 15/20
60000/60000 [==============================] - 3s 52us/step - loss: 0.0035 - acc: 0.9988 - val_loss: 0.0389 - val_acc: 0.9926
Epoch 16/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0031 - acc: 0.9990 - val_loss: 0.0330 - val_acc: 0.9931
Epoch 17/20
60000/60000 [==============================] - 3s 53us/step - loss: 0.0031 - acc: 0.9988 - val_loss: 0.0347 - val_acc: 0.9935
Epoch 18/20
60000/60000 [==============================] - 3s 52us/step - loss: 0.0035 - acc: 0.9987 - val_loss: 0.0385 - val_acc: 0.9930
Epoch 19/20
60000/60000 [==============================] - 3s 54us/step - loss: 0.0040 - acc: 0.9986 - val_loss: 0.0310 - val_acc: 0.9942
Epoch 20/20
60000/60000 [==============================] - 3s 52us/step - loss: 0.0029 - acc: 0.9988 - val_loss: 0.0362 - val_acc: 0.9930