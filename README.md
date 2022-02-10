# K-Nearest Neighbor Density Estimation
k-nearest neighbor (k-NN) is a cool and powerful idea for nonparametric estimation. The kNN method estimates the density value at point x based on the distance between x and its k-th nearest neighbor. Compared with other methods, the kNN density estimation method has several advantages. It is purely nonparametric and hence can flexibly adapt to any underlying pdf, as long as the pdf is continuous. Moreover, the kNN method is convenient to use and has desirable time complexity. The parameter tuning is simple since the only parameter we need to adjust is k. The general expression for nonparametric density estimation is:

![image](https://user-images.githubusercontent.com/23229539/153462308-fbabf64e-b970-4493-aa41-d959fe528d48.png)

Fixing 𝑘 and determining the minimum volume 𝑉 that encompasses 𝑘 points in the dataset, we grow the volume surrounding the estimation point 𝑥 until it encloses a total of k data points.

![image](https://user-images.githubusercontent.com/23229539/153463487-b3fd91ce-c3ad-4aed-8183-a537156e686d.png)

To find 𝑃(𝑥) with KNN:
- Consider a hypersphere around 𝑥
- Enlarge the radius of the hypersphere until it contains 𝑘 data points
- The volume 𝑉 is determined by calculating the volume of the hypersphere. Then, we have:

![image](https://user-images.githubusercontent.com/23229539/153463712-8982b857-eb10-4011-9539-6d48864948c5.png)


