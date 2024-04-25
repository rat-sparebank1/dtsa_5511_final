# Final project for DTSA 5511 - Using RNNs to recognize digits from the MNIST dataset
The goal to this project is to recognize digits using diffent NN architectures. 
I have compared a classic CNN, a hybrid CNN-LSTM, an unidirectional LSMT, a bidirectional LSTM and a bidirectional GRU

I have used TensorFlow for this project. 

## How was this done?
I used TensorFlow to create simple sequential models where the inputs were the images, in form as normalized arrays and then the models were trained 5 epochs using accuracy as a metric and Adam as optimizer. 
Then the models were compared using their validation accuracy and by confusion matrix. 

## What was the conclusions?
* The Recursive NN do a good job classifying digits, but CNNs did an even better job
* Some digits are naturally harder to classify due to their similarities, but misclassification happened differently for a CNN 4 was often misclassified as 9 but for an LSTM was 9 that ended been misclassified as 3. 
* Recursive NN were significantly faster to train, mostly because they were smaller than CNNs in this project. 
* Another important observation this that the dataset was comprised of images that were centered, homogeneous and with similar background. 
* I am almost sure that if the images were more complex like dog picture, the recursive NN would have perfomed a lot worse, especially since I implemented them only looking at horizontal sequences (meaning only loooking at rows). Translational invariance is an important advantage for CNN.



