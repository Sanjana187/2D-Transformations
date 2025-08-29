# 2D-Transformations
Implementation of 2D geometric transformations (Translation, Rotation, Scaling, Shearing, Affine, Similarity, and Projective) in Python with mathematical explanations and visualization.
# 2D Geometric Transformations

This project demonstrates *2D geometric transformations* in Python, including:

- *Translation*
- *Scaling*
- *Rotation*
- *Reflection*
- *Shear*
- *Similarity Transformation*
- *Affine Transformation*
- *Projective Transformation*

The transformations are implemented using *NumPy* and *Matplotlib* for visualization, making it easy to understand how each transformation modifies a given shape.

---

## 🔹 Mathematical Background
**Translation Matrix**

![Translation](https://latex.codecogs.com/svg.latex?\begin%7Bbmatrix%7Dx%27%5C%5Cy%27%5C%5C1%5Cend%7Bbmatrix%7D=%5Cbegin%7Bbmatrix%7D1&0&t_x%5C%5C0&1&t_y%5C%5C0&0&1%5Cend%7Bbmatrix%7D\begin%7Bbmatrix%7Dx%5C%5Cy%5C%5C1%5Cend%7Bbmatrix%7D)



**Scaling Transformation**

![Scaling](https://latex.codecogs.com/svg.latex?\begin%7Bbmatrix%7Dx%27%5C%5Cy%27%5C%5C1%5Cend%7Bbmatrix%7D=%5Cbegin%7Bbmatrix%7Ds_x&0&0%5C%5C0&s_y&0%5C%5C0&0&1%5Cend%7Bbmatrix%7D\begin%7Bbmatrix%7Dx%5C%5Cy%5C%5C1%5Cend%7Bbmatrix%7D)

### 3. Rotation
$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
=
\begin{bmatrix}
\cos\theta & \sin\theta & 0 \\
-\sin\theta & \cos\theta & 0 \\
0 & 0 & 1
\end{bmatrix}
\cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

### 4. Reflection
Reflection across the x-axis:
$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
=
\begin{bmatrix}
1 & 0 & 0 \\
0 & -1 & 0 \\
0 & 0 & 1
\end{bmatrix}
\cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

### 5. Shear
$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
=
\begin{bmatrix}
1 & k_x & 0 \\
k_y & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
\cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

### 6. Similarity Transformation
Combination of scaling, rotation, and translation:
$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
=
\begin{bmatrix}
s\cos\theta & s\sin\theta & t_x \\
-s\sin\theta & s\cos\theta & t_y \\
0 & 0 & 1
\end{bmatrix}
\cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

### 7. Affine Transformation
$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
=
\begin{bmatrix}
a_{11} & a_{12} & t_x \\
a_{21} & a_{22} & t_y \\
0 & 0 & 1
\end{bmatrix}
\cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

### 8. Projective Transformation
$$
\begin{bmatrix}
x' \\ y' \\ w
\end{bmatrix}
=
\begin{bmatrix}
h_{11} & h_{12} & h_{13} \\
h_{21} & h_{22} & h_{23} \\
h_{31} & h_{32} & h_{33}
\end{bmatrix}
\cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

Final coordinates after normalization:
$$
x' = \frac{x'}{w}, \quad y' = \frac{y'}{w}
$$

---

## 🔹 Project Structure
