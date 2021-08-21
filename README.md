# Auto_Drive_Learning
I would record important ideas and inspirations in this repository which are related with machine learning, deep learning and their applications on auto-drive and ADAS.

## 1. Traditional Edge detection on image processing 

## 2. Machine Learning on lane detection

### K_means algorithm:
Descriptions: K-means clustering was chosen as it provided a natural principle (Euclidean Distance) to go about for a lane detection

steps: 
1. Preprocessing Image

          (1) White Color Thresholding, {Image I<R,G,B> >= <200, 200, 200>} => {Image I<R,G,B> = <255, 255, 255>}
          
          (2) Area Thresholding, remove non-target contours
          
          (3) Hough Transform [normal form](https://en.wikipedia.org/wiki/Hough_transform)
          Probabilistic Hough Transform does give us the lane marking position, but it also do the same process to all clusters and unkown points
          
2. Application of K-means to get Line Data
       
          (1) Silhouette Coefficient is the measuring standard
          if the coefficient is positive and close to 1, which is indicative of good clustering.
