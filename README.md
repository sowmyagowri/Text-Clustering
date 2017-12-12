# Text-Clustering

### Normalized Mutual Information (NMI) Score: 0.6934

## Approach:
1.	The input data containing 8580 text records in sparse format is first read into a matrix.
2.	This CSR matrix is then scaled by IDF and normalized by its L2-norm and then converted to a dense ndarray representation.
3.	This array is then separated into the desired number of clusters using bisecting k-means clustering approach.

[Calinski Harabaz Score](http://www.tandfonline.com/doi/abs/10.1080/03610927408827101) (Caliński, T., & Harabasz, J. (1974). “A dendrite method for cluster analysis”. Communications in Statistics-theory and Methods 3: 1-27.) has been calculated for the list of clusters for values of k starting from 3 to 21 in steps of 2 for the given dataset.

This metric has been plotted on the y-axis against the values for k on the x-axis

![plot](https://user-images.githubusercontent.com/25673997/33753064-33aecb48-db9a-11e7-8f24-eb86118e9827.png)
