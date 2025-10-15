# Brain Tumor Segmentation

## Dataset Link: https://www.kaggle.com/datasets/mateuszbuda/lgg-mri-segmentation

## Kaggle Notebook: https://www.kaggle.com/code/shasan7/brain-mri-segmentation-unet-base

With help of TensorFlow and its high-level API Keras, we defined the U-Net architecture from scratch for Brain Tumor Segmentation , and also defined the metrics to monitor loss and performance.

The model was trained for 100 epochs using a batch size of 8, achieving Dice Socre of 90.14 % along with a 82.94 IoU. We also augmented the training set with random shift, shear, zoom and horizontal flip before feeding to the model. Following are some training samples after augmentation:

![Augmented Images: ](Images.png)

## Model's Mask Predictions:

![Prediction 1: ](Prediction_1.png)
![Prediction 2: ](Prediction_2.png)
![Prediction 3: ](Prediction_3.png)
![Prediction 4: ](Prediction_4.png)
![Prediction 5: ](Prediction_5.png)
![Prediction 6: ](Prediction_6.png)

## Training & Validation Dice, IoU and Loss:

![Acc_Loss: ](Acc_Loss.png)

## Training Summary:

Epoch 1/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 181s 368ms/step - accuracy: 0.8951 - dice_coef: 0.1085 - iou_coef: 0.0602 - loss: -0.1085 - val_accuracy: 0.9914 - val_dice_coef: 0.1048 - val_iou_coef: 0.0580 - val_loss: -0.1048
Epoch 2/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 226ms/step - accuracy: 0.9853 - dice_coef: 0.2207 - iou_coef: 0.1315 - loss: -0.2207 - val_accuracy: 0.9939 - val_dice_coef: 0.2683 - val_iou_coef: 0.1658 - val_loss: -0.2683
Epoch 3/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 92s 234ms/step - accuracy: 0.9921 - dice_coef: 0.3283 - iou_coef: 0.2082 - loss: -0.3283 - val_accuracy: 0.9947 - val_dice_coef: 0.4053 - val_iou_coef: 0.2761 - val_loss: -0.4080
Epoch 4/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 226ms/step - accuracy: 0.9943 - dice_coef: 0.4616 - iou_coef: 0.3183 - loss: -0.4615 - val_accuracy: 0.9951 - val_dice_coef: 0.5666 - val_iou_coef: 0.4201 - val_loss: -0.5646
Epoch 5/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 226ms/step - accuracy: 0.9953 - dice_coef: 0.5497 - iou_coef: 0.4086 - loss: -0.5505 - val_accuracy: 0.9963 - val_dice_coef: 0.6136 - val_iou_coef: 0.4798 - val_loss: -0.6170
Epoch 6/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9962 - dice_coef: 0.6278 - iou_coef: 0.4882 - loss: -0.6276 - val_accuracy: 0.9959 - val_dice_coef: 0.6486 - val_iou_coef: 0.5241 - val_loss: -0.6515
Epoch 7/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9966 - dice_coef: 0.6769 - iou_coef: 0.5509 - loss: -0.6767 - val_accuracy: 0.9960 - val_dice_coef: 0.6875 - val_iou_coef: 0.5641 - val_loss: -0.6859
Epoch 8/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9968 - dice_coef: 0.7255 - iou_coef: 0.6055 - loss: -0.7256 - val_accuracy: 0.9962 - val_dice_coef: 0.7374 - val_iou_coef: 0.6153 - val_loss: -0.7360
Epoch 9/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9968 - dice_coef: 0.7588 - iou_coef: 0.6408 - loss: -0.7586 - val_accuracy: 0.9964 - val_dice_coef: 0.7119 - val_iou_coef: 0.5987 - val_loss: -0.7134
Epoch 10/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9970 - dice_coef: 0.7567 - iou_coef: 0.6437 - loss: -0.7565 - val_accuracy: 0.9968 - val_dice_coef: 0.7835 - val_iou_coef: 0.6710 - val_loss: -0.7851
Epoch 11/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9971 - dice_coef: 0.7908 - iou_coef: 0.6832 - loss: -0.7908 - val_accuracy: 0.9967 - val_dice_coef: 0.7371 - val_iou_coef: 0.6253 - val_loss: -0.7355
Epoch 12/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9974 - dice_coef: 0.7873 - iou_coef: 0.6840 - loss: -0.7872 - val_accuracy: 0.9972 - val_dice_coef: 0.8259 - val_iou_coef: 0.7284 - val_loss: -0.8250
Epoch 13/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9973 - dice_coef: 0.7894 - iou_coef: 0.6882 - loss: -0.7899 - val_accuracy: 0.9974 - val_dice_coef: 0.8315 - val_iou_coef: 0.7321 - val_loss: -0.8314
Epoch 14/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9972 - dice_coef: 0.8185 - iou_coef: 0.7188 - loss: -0.8185 - val_accuracy: 0.9970 - val_dice_coef: 0.8089 - val_iou_coef: 0.7129 - val_loss: -0.8081
Epoch 15/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9974 - dice_coef: 0.8222 - iou_coef: 0.7215 - loss: -0.8221 - val_accuracy: 0.9968 - val_dice_coef: 0.7888 - val_iou_coef: 0.6834 - val_loss: -0.7887
Epoch 16/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 90s 230ms/step - accuracy: 0.9974 - dice_coef: 0.8320 - iou_coef: 0.7372 - loss: -0.8320 - val_accuracy: 0.9972 - val_dice_coef: 0.8147 - val_iou_coef: 0.7211 - val_loss: -0.8143
Epoch 17/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 87s 223ms/step - accuracy: 0.9966 - dice_coef: 0.7712 - iou_coef: 0.6743 - loss: -0.7712 - val_accuracy: 0.9975 - val_dice_coef: 0.8355 - val_iou_coef: 0.7452 - val_loss: -0.8355
Epoch 18/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9974 - dice_coef: 0.8363 - iou_coef: 0.7417 - loss: -0.8362 - val_accuracy: 0.9976 - val_dice_coef: 0.8263 - val_iou_coef: 0.7372 - val_loss: -0.8255
Epoch 19/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9975 - dice_coef: 0.8220 - iou_coef: 0.7258 - loss: -0.8220 - val_accuracy: 0.9976 - val_dice_coef: 0.8416 - val_iou_coef: 0.7568 - val_loss: -0.8414
Epoch 20/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9975 - dice_coef: 0.8160 - iou_coef: 0.7201 - loss: -0.8160 - val_accuracy: 0.9975 - val_dice_coef: 0.8504 - val_iou_coef: 0.7592 - val_loss: -0.8562
Epoch 21/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9975 - dice_coef: 0.8349 - iou_coef: 0.7414 - loss: -0.8349 - val_accuracy: 0.9977 - val_dice_coef: 0.8235 - val_iou_coef: 0.7372 - val_loss: -0.8269
Epoch 22/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9976 - dice_coef: 0.8289 - iou_coef: 0.7404 - loss: -0.8288 - val_accuracy: 0.9974 - val_dice_coef: 0.8367 - val_iou_coef: 0.7500 - val_loss: -0.8385
Epoch 23/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9978 - dice_coef: 0.8445 - iou_coef: 0.7585 - loss: -0.8445 - val_accuracy: 0.9969 - val_dice_coef: 0.7951 - val_iou_coef: 0.6931 - val_loss: -0.7943
Epoch 24/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9977 - dice_coef: 0.8447 - iou_coef: 0.7601 - loss: -0.8447 - val_accuracy: 0.9976 - val_dice_coef: 0.8522 - val_iou_coef: 0.7662 - val_loss: -0.8524
Epoch 25/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9976 - dice_coef: 0.8410 - iou_coef: 0.7504 - loss: -0.8410 - val_accuracy: 0.9967 - val_dice_coef: 0.7970 - val_iou_coef: 0.6972 - val_loss: -0.7961
Epoch 26/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9979 - dice_coef: 0.8390 - iou_coef: 0.7532 - loss: -0.8391 - val_accuracy: 0.9975 - val_dice_coef: 0.8373 - val_iou_coef: 0.7488 - val_loss: -0.8370
Epoch 27/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9977 - dice_coef: 0.8509 - iou_coef: 0.7677 - loss: -0.8510 - val_accuracy: 0.9975 - val_dice_coef: 0.8209 - val_iou_coef: 0.7368 - val_loss: -0.8202
Epoch 28/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9979 - dice_coef: 0.8655 - iou_coef: 0.7850 - loss: -0.8655 - val_accuracy: 0.9977 - val_dice_coef: 0.8745 - val_iou_coef: 0.7920 - val_loss: -0.8741
Epoch 29/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9978 - dice_coef: 0.8637 - iou_coef: 0.7778 - loss: -0.8636 - val_accuracy: 0.9978 - val_dice_coef: 0.8757 - val_iou_coef: 0.7963 - val_loss: -0.8753
Epoch 30/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9978 - dice_coef: 0.8439 - iou_coef: 0.7605 - loss: -0.8438 - val_accuracy: 0.9975 - val_dice_coef: 0.8539 - val_iou_coef: 0.7759 - val_loss: -0.8533
Epoch 31/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9979 - dice_coef: 0.8578 - iou_coef: 0.7742 - loss: -0.8578 - val_accuracy: 0.9977 - val_dice_coef: 0.8452 - val_iou_coef: 0.7609 - val_loss: -0.8445
Epoch 32/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9977 - dice_coef: 0.8453 - iou_coef: 0.7613 - loss: -0.8452 - val_accuracy: 0.9978 - val_dice_coef: 0.8564 - val_iou_coef: 0.7798 - val_loss: -0.8558
Epoch 33/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9980 - dice_coef: 0.8669 - iou_coef: 0.7849 - loss: -0.8668 - val_accuracy: 0.9977 - val_dice_coef: 0.8545 - val_iou_coef: 0.7671 - val_loss: -0.8539
Epoch 34/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9980 - dice_coef: 0.8701 - iou_coef: 0.7899 - loss: -0.8701 - val_accuracy: 0.9976 - val_dice_coef: 0.8291 - val_iou_coef: 0.7409 - val_loss: -0.8282
Epoch 35/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9979 - dice_coef: 0.8679 - iou_coef: 0.7876 - loss: -0.8679 - val_accuracy: 0.9975 - val_dice_coef: 0.8673 - val_iou_coef: 0.7810 - val_loss: -0.8669
Epoch 36/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9979 - dice_coef: 0.8591 - iou_coef: 0.7777 - loss: -0.8591 - val_accuracy: 0.9977 - val_dice_coef: 0.8775 - val_iou_coef: 0.7941 - val_loss: -0.8772
Epoch 37/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9981 - dice_coef: 0.8730 - iou_coef: 0.7958 - loss: -0.8730 - val_accuracy: 0.9979 - val_dice_coef: 0.8705 - val_iou_coef: 0.7953 - val_loss: -0.8698
Epoch 38/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9978 - dice_coef: 0.8652 - iou_coef: 0.7863 - loss: -0.8653 - val_accuracy: 0.9976 - val_dice_coef: 0.8385 - val_iou_coef: 0.7536 - val_loss: -0.8376
Epoch 39/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9981 - dice_coef: 0.8772 - iou_coef: 0.8024 - loss: -0.8772 - val_accuracy: 0.9978 - val_dice_coef: 0.8593 - val_iou_coef: 0.7797 - val_loss: -0.8585
Epoch 40/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9980 - dice_coef: 0.8724 - iou_coef: 0.7959 - loss: -0.8729 - val_accuracy: 0.9981 - val_dice_coef: 0.8827 - val_iou_coef: 0.8066 - val_loss: -0.8821
Epoch 41/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9982 - dice_coef: 0.8821 - iou_coef: 0.8075 - loss: -0.8821 - val_accuracy: 0.9979 - val_dice_coef: 0.8908 - val_iou_coef: 0.8128 - val_loss: -0.8902
Epoch 42/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9982 - dice_coef: 0.8822 - iou_coef: 0.8058 - loss: -0.8822 - val_accuracy: 0.9979 - val_dice_coef: 0.8619 - val_iou_coef: 0.7829 - val_loss: -0.8611
Epoch 43/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9981 - dice_coef: 0.8828 - iou_coef: 0.8082 - loss: -0.8828 - val_accuracy: 0.9978 - val_dice_coef: 0.8623 - val_iou_coef: 0.7890 - val_loss: -0.8668
Epoch 44/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9979 - dice_coef: 0.8610 - iou_coef: 0.7830 - loss: -0.8609 - val_accuracy: 0.9978 - val_dice_coef: 0.8823 - val_iou_coef: 0.8018 - val_loss: -0.8816
Epoch 45/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9981 - dice_coef: 0.8839 - iou_coef: 0.8089 - loss: -0.8839 - val_accuracy: 0.9982 - val_dice_coef: 0.8673 - val_iou_coef: 0.7883 - val_loss: -0.8668
Epoch 46/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9981 - dice_coef: 0.8775 - iou_coef: 0.8021 - loss: -0.8775 - val_accuracy: 0.9974 - val_dice_coef: 0.8482 - val_iou_coef: 0.7640 - val_loss: -0.8474
Epoch 47/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9980 - dice_coef: 0.8734 - iou_coef: 0.7981 - loss: -0.8733 - val_accuracy: 0.9981 - val_dice_coef: 0.8816 - val_iou_coef: 0.8118 - val_loss: -0.8811
Epoch 48/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9981 - dice_coef: 0.8759 - iou_coef: 0.8030 - loss: -0.8760 - val_accuracy: 0.9978 - val_dice_coef: 0.8473 - val_iou_coef: 0.7629 - val_loss: -0.8513
Epoch 49/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9981 - dice_coef: 0.8862 - iou_coef: 0.8079 - loss: -0.8862 - val_accuracy: 0.9976 - val_dice_coef: 0.8763 - val_iou_coef: 0.7992 - val_loss: -0.8761
Epoch 50/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9980 - dice_coef: 0.8768 - iou_coef: 0.7981 - loss: -0.8767 - val_accuracy: 0.9982 - val_dice_coef: 0.8909 - val_iou_coef: 0.8175 - val_loss: -0.8923
Epoch 51/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9981 - dice_coef: 0.8956 - iou_coef: 0.8251 - loss: -0.8956 - val_accuracy: 0.9978 - val_dice_coef: 0.8801 - val_iou_coef: 0.8061 - val_loss: -0.8845
Epoch 52/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9979 - dice_coef: 0.8850 - iou_coef: 0.8100 - loss: -0.8850 - val_accuracy: 0.9979 - val_dice_coef: 0.8677 - val_iou_coef: 0.7905 - val_loss: -0.8668
Epoch 53/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9981 - dice_coef: 0.8878 - iou_coef: 0.8136 - loss: -0.8878 - val_accuracy: 0.9981 - val_dice_coef: 0.8956 - val_iou_coef: 0.8255 - val_loss: -0.8950
Epoch 54/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9981 - dice_coef: 0.8796 - iou_coef: 0.8020 - loss: -0.8797 - val_accuracy: 0.9978 - val_dice_coef: 0.8816 - val_iou_coef: 0.8050 - val_loss: -0.8815
Epoch 55/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9981 - dice_coef: 0.8729 - iou_coef: 0.8007 - loss: -0.8732 - val_accuracy: 0.9973 - val_dice_coef: 0.8513 - val_iou_coef: 0.7689 - val_loss: -0.8502
Epoch 56/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9982 - dice_coef: 0.8939 - iou_coef: 0.8186 - loss: -0.8938 - val_accuracy: 0.9979 - val_dice_coef: 0.8764 - val_iou_coef: 0.7983 - val_loss: -0.8769
Epoch 57/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9980 - dice_coef: 0.8903 - iou_coef: 0.8165 - loss: -0.8903 - val_accuracy: 0.9976 - val_dice_coef: 0.8589 - val_iou_coef: 0.7772 - val_loss: -0.8588
Epoch 58/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 87s 221ms/step - accuracy: 0.9983 - dice_coef: 0.8824 - iou_coef: 0.8095 - loss: -0.8823 - val_accuracy: 0.9980 - val_dice_coef: 0.8215 - val_iou_coef: 0.7498 - val_loss: -0.8203
Epoch 59/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 89s 226ms/step - accuracy: 0.9980 - dice_coef: 0.8866 - iou_coef: 0.8101 - loss: -0.8866 - val_accuracy: 0.9980 - val_dice_coef: 0.8872 - val_iou_coef: 0.8103 - val_loss: -0.8866
Epoch 60/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 87s 221ms/step - accuracy: 0.9974 - dice_coef: 0.8377 - iou_coef: 0.7620 - loss: -0.8376 - val_accuracy: 0.9979 - val_dice_coef: 0.8575 - val_iou_coef: 0.7829 - val_loss: -0.8569
Epoch 61/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 89s 226ms/step - accuracy: 0.9983 - dice_coef: 0.9007 - iou_coef: 0.8306 - loss: -0.9007 - val_accuracy: 0.9974 - val_dice_coef: 0.8588 - val_iou_coef: 0.7689 - val_loss: -0.8600
Epoch 62/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 87s 221ms/step - accuracy: 0.9980 - dice_coef: 0.8907 - iou_coef: 0.8178 - loss: -0.8907 - val_accuracy: 0.9980 - val_dice_coef: 0.8824 - val_iou_coef: 0.8097 - val_loss: -0.8816
Epoch 63/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 226ms/step - accuracy: 0.9981 - dice_coef: 0.8974 - iou_coef: 0.8243 - loss: -0.8974 - val_accuracy: 0.9980 - val_dice_coef: 0.9036 - val_iou_coef: 0.8329 - val_loss: -0.9032
Epoch 64/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 87s 221ms/step - accuracy: 0.9984 - dice_coef: 0.8913 - iou_coef: 0.8205 - loss: -0.8913 - val_accuracy: 0.9978 - val_dice_coef: 0.8605 - val_iou_coef: 0.7767 - val_loss: -0.8595
Epoch 65/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 87s 221ms/step - accuracy: 0.9982 - dice_coef: 0.8955 - iou_coef: 0.8267 - loss: -0.8955 - val_accuracy: 0.9976 - val_dice_coef: 0.8732 - val_iou_coef: 0.7936 - val_loss: -0.8725
Epoch 66/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9981 - dice_coef: 0.8977 - iou_coef: 0.8258 - loss: -0.8977 - val_accuracy: 0.9978 - val_dice_coef: 0.8793 - val_iou_coef: 0.7982 - val_loss: -0.8804
Epoch 67/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9981 - dice_coef: 0.8915 - iou_coef: 0.8185 - loss: -0.8916 - val_accuracy: 0.9980 - val_dice_coef: 0.8707 - val_iou_coef: 0.7973 - val_loss: -0.8702
Epoch 68/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9983 - dice_coef: 0.8990 - iou_coef: 0.8271 - loss: -0.8990 - val_accuracy: 0.9979 - val_dice_coef: 0.8895 - val_iou_coef: 0.8141 - val_loss: -0.8894
Epoch 69/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9981 - dice_coef: 0.8842 - iou_coef: 0.8064 - loss: -0.8843 - val_accuracy: 0.9978 - val_dice_coef: 0.8846 - val_iou_coef: 0.8102 - val_loss: -0.8846
Epoch 70/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9983 - dice_coef: 0.8954 - iou_coef: 0.8267 - loss: -0.8953 - val_accuracy: 0.9979 - val_dice_coef: 0.8731 - val_iou_coef: 0.7943 - val_loss: -0.8722
Epoch 71/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9984 - dice_coef: 0.8908 - iou_coef: 0.8228 - loss: -0.8908 - val_accuracy: 0.9982 - val_dice_coef: 0.8896 - val_iou_coef: 0.8171 - val_loss: -0.8894
Epoch 72/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9982 - dice_coef: 0.8922 - iou_coef: 0.8198 - loss: -0.8921 - val_accuracy: 0.9977 - val_dice_coef: 0.8809 - val_iou_coef: 0.8002 - val_loss: -0.8800
Epoch 73/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9983 - dice_coef: 0.9023 - iou_coef: 0.8322 - loss: -0.9023 - val_accuracy: 0.9981 - val_dice_coef: 0.8863 - val_iou_coef: 0.8098 - val_loss: -0.8857
Epoch 74/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9982 - dice_coef: 0.8909 - iou_coef: 0.8266 - loss: -0.8909 - val_accuracy: 0.9978 - val_dice_coef: 0.8747 - val_iou_coef: 0.7955 - val_loss: -0.8738
Epoch 75/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 226ms/step - accuracy: 0.9984 - dice_coef: 0.9049 - iou_coef: 0.8351 - loss: -0.9049 - val_accuracy: 0.9981 - val_dice_coef: 0.8809 - val_iou_coef: 0.8084 - val_loss: -0.8800
Epoch 76/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9982 - dice_coef: 0.8923 - iou_coef: 0.8203 - loss: -0.8923 - val_accuracy: 0.9975 - val_dice_coef: 0.8409 - val_iou_coef: 0.7636 - val_loss: -0.8398
Epoch 77/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9979 - dice_coef: 0.8617 - iou_coef: 0.7857 - loss: -0.8617 - val_accuracy: 0.9980 - val_dice_coef: 0.8627 - val_iou_coef: 0.7866 - val_loss: -0.8617
Epoch 78/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9983 - dice_coef: 0.9058 - iou_coef: 0.8373 - loss: -0.9059 - val_accuracy: 0.9979 - val_dice_coef: 0.8644 - val_iou_coef: 0.7891 - val_loss: -0.8634
Epoch 79/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9983 - dice_coef: 0.8968 - iou_coef: 0.8287 - loss: -0.8968 - val_accuracy: 0.9981 - val_dice_coef: 0.8722 - val_iou_coef: 0.7977 - val_loss: -0.8715
Epoch 80/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 225ms/step - accuracy: 0.9984 - dice_coef: 0.9107 - iou_coef: 0.8449 - loss: -0.9107 - val_accuracy: 0.9978 - val_dice_coef: 0.8631 - val_iou_coef: 0.7852 - val_loss: -0.8691
Epoch 81/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9984 - dice_coef: 0.8946 - iou_coef: 0.8235 - loss: -0.8946 - val_accuracy: 0.9980 - val_dice_coef: 0.8773 - val_iou_coef: 0.8008 - val_loss: -0.8764
Epoch 82/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9982 - dice_coef: 0.9040 - iou_coef: 0.8363 - loss: -0.9039 - val_accuracy: 0.9980 - val_dice_coef: 0.8871 - val_iou_coef: 0.8088 - val_loss: -0.8868
Epoch 83/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9983 - dice_coef: 0.9042 - iou_coef: 0.8377 - loss: -0.9042 - val_accuracy: 0.9980 - val_dice_coef: 0.9014 - val_iou_coef: 0.8294 - val_loss: -0.9006
Epoch 84/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9984 - dice_coef: 0.9102 - iou_coef: 0.8444 - loss: -0.9102 - val_accuracy: 0.9977 - val_dice_coef: 0.8681 - val_iou_coef: 0.7877 - val_loss: -0.8691
Epoch 85/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9984 - dice_coef: 0.8935 - iou_coef: 0.8241 - loss: -0.8935 - val_accuracy: 0.9981 - val_dice_coef: 0.8822 - val_iou_coef: 0.8066 - val_loss: -0.8813
Epoch 86/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9982 - dice_coef: 0.9041 - iou_coef: 0.8370 - loss: -0.9041 - val_accuracy: 0.9980 - val_dice_coef: 0.8998 - val_iou_coef: 0.8273 - val_loss: -0.8991
Epoch 87/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9984 - dice_coef: 0.9026 - iou_coef: 0.8327 - loss: -0.9026 - val_accuracy: 0.9980 - val_dice_coef: 0.8773 - val_iou_coef: 0.8039 - val_loss: -0.8764
Epoch 88/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9983 - dice_coef: 0.9051 - iou_coef: 0.8372 - loss: -0.9051 - val_accuracy: 0.9980 - val_dice_coef: 0.8838 - val_iou_coef: 0.8073 - val_loss: -0.8829
Epoch 89/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9983 - dice_coef: 0.9054 - iou_coef: 0.8362 - loss: -0.9054 - val_accuracy: 0.9978 - val_dice_coef: 0.8868 - val_iou_coef: 0.8146 - val_loss: -0.8859
Epoch 90/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9984 - dice_coef: 0.8967 - iou_coef: 0.8270 - loss: -0.8967 - val_accuracy: 0.9982 - val_dice_coef: 0.8775 - val_iou_coef: 0.7985 - val_loss: -0.8777
Epoch 91/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9983 - dice_coef: 0.8884 - iou_coef: 0.8151 - loss: -0.8884 - val_accuracy: 0.9980 - val_dice_coef: 0.8920 - val_iou_coef: 0.8190 - val_loss: -0.8916
Epoch 92/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9983 - dice_coef: 0.8958 - iou_coef: 0.8302 - loss: -0.8958 - val_accuracy: 0.9981 - val_dice_coef: 0.8938 - val_iou_coef: 0.8202 - val_loss: -0.8935
Epoch 93/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9983 - dice_coef: 0.8978 - iou_coef: 0.8310 - loss: -0.8978 - val_accuracy: 0.9982 - val_dice_coef: 0.8830 - val_iou_coef: 0.8140 - val_loss: -0.8830
Epoch 94/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 226ms/step - accuracy: 0.9984 - dice_coef: 0.9183 - iou_coef: 0.8546 - loss: -0.9183 - val_accuracy: 0.9979 - val_dice_coef: 0.8887 - val_iou_coef: 0.8169 - val_loss: -0.8883
Epoch 95/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9983 - dice_coef: 0.8953 - iou_coef: 0.8276 - loss: -0.8953 - val_accuracy: 0.9980 - val_dice_coef: 0.8813 - val_iou_coef: 0.8071 - val_loss: -0.8804
Epoch 96/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 88s 226ms/step - accuracy: 0.9982 - dice_coef: 0.9128 - iou_coef: 0.8460 - loss: -0.9128 - val_accuracy: 0.9981 - val_dice_coef: 0.9004 - val_iou_coef: 0.8321 - val_loss: -0.8996
Epoch 97/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9983 - dice_coef: 0.8996 - iou_coef: 0.8285 - loss: -0.8996 - val_accuracy: 0.9978 - val_dice_coef: 0.8733 - val_iou_coef: 0.7931 - val_loss: -0.8729
Epoch 98/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9982 - dice_coef: 0.9097 - iou_coef: 0.8423 - loss: -0.9097 - val_accuracy: 0.9978 - val_dice_coef: 0.8722 - val_iou_coef: 0.7952 - val_loss: -0.8726
Epoch 99/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 220ms/step - accuracy: 0.9983 - dice_coef: 0.9046 - iou_coef: 0.8351 - loss: -0.9045 - val_accuracy: 0.9979 - val_dice_coef: 0.8780 - val_iou_coef: 0.8023 - val_loss: -0.8787
Epoch 100/100
392/392 ━━━━━━━━━━━━━━━━━━━━ 86s 221ms/step - accuracy: 0.9982 - dice_coef: 0.8942 - iou_coef: 0.8225 - loss: -0.8941 - val_accuracy: 0.9980 - val_dice_coef: 0.8756 - val_iou_coef: 0.8047 - val_loss: -0.8756


