Hierarchical Clustering
This project aims to cluster a set of given images without supervision using hierarchical clustering. The clustering is performed using the glob library for image loading, HOG (Histogram of Oriented Gradients) for feature extraction, Jensen-Shannon distance matrix for similarity measurement, and the Ward method for linkage.

Problem Statement
Given a collection of images, the goal is to group them into clusters based on their visual similarities. The clustering process is unsupervised, meaning there are no pre-defined labels or categories for the images. The algorithm will analyze the images, extract their features using HOG, calculate the Jensen-Shannon distance matrix, and use the Ward method for hierarchical clustering.

Dependencies
Python 3.x
OpenCV (cv2) library
scikit-image library
scipy library
glob library
Installation
Clone the repository:

git clone https://github.com/your-username/hierarchical-clustering.git
Install the required dependencies:


pip install opencv-python
pip install scikit-image
pip install scipy
Usage
Place the images you want to cluster in the project directory.

Run the main script:

Finalheirarproj.ipynb
python hierarchical_clustering.py
The algorithm will load the images using the glob library and apply HOG feature extraction to obtain the feature vectors.

The Jensen-Shannon distance matrix will be calculated based on the feature vectors, measuring the similarity between pairs of images.

The hierarchical clustering algorithm using the Ward method will be performed on the distance matrix to group the images into clusters.

The resulting clusters will be represented using a dendrogram.

Customization
You can customize the project according to your specific needs:

Adjust the parameters of HOG feature extraction, such as cell size, block size, and number of orientations, for better feature representation.
Explore different distance metrics other than Jensen-Shannon if desired.
Modify the linkage method in the hierarchical clustering algorithm to experiment with different clustering strategies.

Acknowledgments
This project was inspired by the need to perform unsupervised clustering on images using hierarchical clustering techniques.

