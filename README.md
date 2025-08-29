# 2D-Transformations
Implementation of 2D geometric transformations (Translation, Rotation, Scaling, Shearing, Affine, Similarity, and Projective) in Python with mathematical explanations and visualization.
# 2D Geometric Transformations

This project demonstrates *2D geometric transformations* in Python, including:

- *Translation*
- *Scaling*
- *Rotation*
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

**Rotation Transformation**

![Rotation](https://latex.codecogs.com/svg.latex?\begin%7Bbmatrix%7Dx%27%5C%5Cy%27%5C%5C1%5Cend%7Bbmatrix%7D=%5Cbegin%7Bbmatrix%7D\cos\theta&\sin\theta&0%5C%5C-\sin\theta&\cos\theta&0%5C%5C0&0&1%5Cend%7Bbmatrix%7D\begin%7Bbmatrix%7Dx%5C%5Cy%5C%5C1%5Cend%7Bbmatrix%7D)


**Shear Transformation**

![Shear](https://latex.codecogs.com/svg.latex?\begin%7Bbmatrix%7Dx%27%5C%5Cy%27%5C%5C1%5Cend%7Bbmatrix%7D=%5Cbegin%7Bbmatrix%7D1&k_x&0%5C%5Ck_y&1&0%5C%5C0&0&1%5Cend%7Bbmatrix%7D\begin%7Bbmatrix%7Dx%5C%5Cy%5C%5C1%5Cend%7Bbmatrix%7D)

**Similarity Transformation**

![Similarity](https://latex.codecogs.com/svg.latex?\begin%7Bbmatrix%7Dx%27%5C%5Cy%27%5C%5C1%5Cend%7Bbmatrix%7D=%5Cbegin%7Bbmatrix%7Ds\cos\theta&s\sin\theta&t_x%5C%5C-s\sin\theta&s\cos\theta&t_y%5C%5C0&0&1%5Cend%7Bbmatrix%7D\begin%7Bbmatrix%7Dx%5C%5Cy%5C%5C1%5Cend%7Bbmatrix%7D)

**Affine Transformation**

![Affine](https://latex.codecogs.com/svg.latex?\begin%7Bbmatrix%7Dx%27%5C%5Cy%27%5C%5C1%5Cend%7Bbmatrix%7D=%5Cbegin%7Bbmatrix%7Da_%7B11%7D&a_%7B12%7D&t_x%5C%5Ca_%7B21%7D&a_%7B22%7D&t_y%5C%5C0&0&1%5Cend%7Bbmatrix%7D\begin%7Bbmatrix%7Dx%5C%5Cy%5C%5C1%5Cend%7Bbmatrix%7D)


**Projective Transformation**

![Projective](https://latex.codecogs.com/svg.latex?\begin%7Bbmatrix%7Dx%27%5C%5Cy%27%5C%5Cw%5Cend%7Bbmatrix%7D=%5Cbegin%7Bbmatrix%7Dh_%7B11%7D&h_%7B12%7D&h_%7B13%7D%5C%5Ch_%7B21%7D&h_%7B22%7D&h_%7B23%7D%5C%5Ch_%7B31%7D&h_%7B32%7D&h_%7B33%7D%5Cend%7Bbmatrix%7D\begin%7Bbmatrix%7Dx%5C%5Cy%5C%5C1%5Cend%7Bbmatrix%7D)

**Normalization:**  
![Normalization](https://latex.codecogs.com/svg.latex?x%27=\frac{x%27}{w},%5Cquad%20y%27=\frac{y%27}{w})


**Final coordinates after normalization:**

![Normalization](https://latex.codecogs.com/svg.latex?x%27=\frac{x%27}{w},\quad%20y%27=\frac{y%27}{w})


---

## 📂 Project Structure

2D-Geometric-Transformations/
│
├── IPA_Pythoncode.ipynb # Jupyter Notebook with implementations
├── README.md # Project documentation
└── requirements.txt # Dependencies


---


---

## How to Run

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/2D-Geometric-Transformations.git
cd 2D-Geometric-Transformations
```

**2. Install dependencies:**

pip install -r requirements.txt

**3. Run with Jupyter Notebook**

jupyter notebook IPA_Pythoncode.ipynb


**Requirements** :

numpy

matplotlib

jupyter
