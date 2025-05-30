Linear algebra 2 : matrix application

seesion : use tensors  in python and solve the system of equations and indentity meaninful patterns in data 

### review introductory linear algebra
1. Linear Algebra is a branch of mathematics that solves **linear equations**, dealing with **vectors, matrices, eigenvalues**, and **eigenvectors**, essential in computational fields.

2. Applications of Linear Algebra  
   2.1 **Machine Learning**: Supports optimization, **matrix operations**, and high-dimensional data manipulation.  
   2.2 **Dimensionality Reduction**: **PCA** transforms data into a lower-dimensional space.  
   2.3 **Ranking**: **Eigenvector calculations**, used in **Google's PageRank**, determine importance in search results.  
   2.4 **Recommender Systems**: **SVD** identifies user preference patterns for personalized recommendations.  
   2.5 **Natural Language Processing (NLP)**  
       - **Topic Modeling**: **LSA** extracts hidden topics.  
       - **Semantic Analysis**: Matrix factorization improves language understanding.  

  matrix inversion: aovids overdetermination, underdetermination, no solutions, infinite solutions
4. Eigen decomposition
  1. applying matrices
  2. affine transformations
34. ### What are Affine Transformations?
Affine transformations are a set of functions that preserve points, straight lines, and planes. These transformations also maintain the relative proportions of figures, though angles and lengths might not always stay the same. In simpler terms, affine transformations ensure that "straightness" and "parallelism" are preserved.

### Types of Affine Transformations
Affine transformations include several familiar operations:
1. **Translation:** Shifting an object from one location to another (like moving an image across a screen).
2. **Scaling:** Enlarging or shrinking an object while keeping its shape proportional.
3. **Rotation:** Rotating an object around a fixed point or axis.
4. **Reflection:** Flipping an object over a line or plane (like a mirror image).
5. **Shear:** Skewing an object in one direction, like tilting a rectangle into a parallelogram.

### Mathematical Representation
Affine transformations can be represented using matrices. In 2D, it often looks like this:

![image](https://github.com/user-attachments/assets/7397e3eb-00b5-4206-bb8e-ab94d9876219)


Here:
- (a, b, c, d): Define how the shape is scaled, rotated, or sheared.
- (e, f): Represent translation (shifting the object).

In 3D, affine transformations use 4x4 matrices and include operations in the \(z\)-axis.

### Applications
Affine transformations are widely used in:
- **Computer Graphics:** For scaling, rotating, and translating images or 3D models.
- **Image Processing:** Aligning or transforming images.
- **Robotics:** Mapping movements in space.
- **Machine Learning:** Working with data transformations in certain algorithms.

    check blog post: affine transformations in python, including how apply them on images as well as vectors

  4. Eigenvector: A vector that doesn't change its direction during a transformation, only its magnitude (scaled by the eigenvalue).
  - eigen in german typical in english translation: charateristics vector
   red vector : vertical
   blue vector: horizontal
   Flipping matrix: red and blue vector is eigen vector 
   Shearing matrix: blue vector is eigen vector for shearing matrix => blue vector having eigen value = 1
   eigen values can also have negative sign, having same eigen vector but it's eigen value = -1
  5. Eigenvalue: A scalar value that shows how much a vector is stretched or squished during a transformation.
  - is scalar that simply scales the eigen vector v
    Eigenvectors and eigenvalues can be derived algebraically (e.g., with the QR algorithm, which was independently developed in the 1950s by both Vera Kublanovskaya and John Francis), however this is outside scope of the ML Foundations series. We'll cheat with NumPy eig() method, which returns a tuple of:

a vector of eigenvalues
a matrix of eigenvectors
![image](https://github.com/user-attachments/assets/8b35dd4c-0fda-46eb-a9a2-24d6d58d264c)

![{C8E1DBA3-154D-4BA9-8983-ECA8D7337540}](https://github.com/user-attachments/assets/4dc954d5-99a4-4978-a347-55aa11fb4da7)

      
   
   36. **matrix determinants**
      - Map square Matrix to scalar
      - Enable us to determine wheather the matrix can be inverted
      - if det(X) = 0 => Matrix X-1(inverse) can't be computed because X-1 has 1/dex(X) = 1/0 => will result in No solution or Infinite solution
      - Easy to calculate 2*2 Matrix
         - Determinant of 2*2 Matrix
         - |a   b|
         - |c   d|
         - |X| = a * d - b * c
   37. **Determinants of larger matrices**
      - Genralizing Determinants: Recursion
   39. **Determinants and Eigen values**
      - dex(X) = product of all eigenvalues of X
      - Determinand & Eigen values relationship: if any one of the eigen values in zero then the product of the eigen values must be zero and determinant also must be zero
   40. **Eigen decomposition**
      - formula:  
   41. **applications of eigen decomposition**
      -  

