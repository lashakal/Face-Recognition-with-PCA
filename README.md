# Face-Recognition-with-PCA
The program uses PCA to recognize faces from a set of training images. PCA is used as a technique to reduce the dimensionality of image data and extract the most discriminative features.

This particular implementation of the face recognition program uses 10 images in total for training, which are all resized to 50 x 50 and converted to grayscale. The program then computes the mean face, subtracts it from the training faces, and calculates the covariance matrix. The eigenvectors and eigenvalues are then obtained from the covariance matrix and the top K eigenvectors are chosen.

The program then projects each training face onto the eigenspace and displays the results graphically. To recognize a new face, the program separates the face from the test image, calculates the feature vector, projects it onto the eigenspace, and calculates the Euclidean distance between the projected test face and each training face. If the distance is below a certain threshold, the face is recognized as belonging to the training set.

The face recognition program implemented using PCA provides a simple yet effective way to recognize faces from a set of training images. Although this kind of implementation is not perfect and there is a host of failures that could be associated with it, it demonstrates how PCA can be used to extract the most informative features from image data and highlights its potential applications in face recognition systems.
