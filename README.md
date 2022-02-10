# K-Nearest Neighbor Density Estimation
k-nearest neighbor (k-NN) is a cool and powerful idea for nonparametric estimation. The kNN method estimates the density value at point x based on the distance between x and its k-th nearest neighbor. Compared with other methods, the kNN density estimation method has several advantages. It is purely nonparametric and hence can flexibly adapt to any underlying pdf, as long as the pdf is continuous. Moreover, the kNN method is convenient to use and has desirable time complexity. The parameter tuning is simple since the only parameter we need to adjust is k. The general expression for nonparametric density estimation is:

![image](https://user-images.githubusercontent.com/23229539/153466005-ab4380a7-0997-4403-a89f-06376f106c89.png)

Fixing 𝑘 and determining the minimum volume 𝑉 that encompasses 𝑘 points in the dataset, we grow the volume surrounding the estimation point 𝑥 until it encloses a total of k data points.

![image](https://user-images.githubusercontent.com/23229539/153465859-05d021df-c286-49dd-b84f-bf11d114de39.png)

To find 𝑃(𝑥) with KNN:
- Consider a hypersphere around 𝑥
- Enlarge the radius of the hypersphere until it contains 𝑘 data points
- The volume 𝑉 is determined by calculating the volume of the hypersphere. Then, we have:

![image](https://user-images.githubusercontent.com/23229539/153465893-6cb69297-157c-4fde-ae3c-a862992f5f2c.png)
