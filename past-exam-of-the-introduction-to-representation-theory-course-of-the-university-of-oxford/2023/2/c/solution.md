<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Order the [conjugacy classes](../../../../conjugacy-class.md) of the [symmetric group](../../../../symmetric-group.md) $S_4$ by representatives $1,(12),(12)(34),(123),(1234)$; their sizes are $1,6,3,8,6$. For a three-dimensional [rotation](../../../../rotation-mathematics.md) through an [angle](../../../../angle.md) $\theta$, the [eigenvalues](../../../../eigenvalue.md) are $1,e^{i\theta},e^{-i\theta}$, so the [trace of a three-dimensional rotation](../../../../trace-of-a-three-dimensional-rotation.md) is $1+2\cos\theta$.

Under the identification with the [rotational symmetry group of a cube](../../../../rotational-symmetry-group-of-a-cube.md), elements of order two give half-turns, elements of order three give turns through $\pm2\pi/3$, and elements of order four give turns through $\pm\pi/2$. A half-turn can have an axis through opposite edges or opposite faces, but both kinds have [trace](../../../../matrix-trace.md) $-1$. Thus

$$
\boxed{\begin{array}{c|rrrrr}
\text{representative}&1&(12)&(12)(34)&(123)&(1234)\\\hline
\text{class size}&1&6&3&8&6\\
\chi_C&3&-1&-1&0&1
\end{array}.}
$$

Its [character inner product](../../../../character-inner-product.md) with itself is

$$
\langle\chi_C,\chi_C\rangle_{S_4}
=\frac{9+6+3+0+6}{24}=1.
$$

By [character orthogonality](../../../../character-orthogonality.md), a nonzero [complex representation](../../../../complex-representation.md) has [character inner product](../../../../character-inner-product.md) one with itself exactly when it is an [irreducible representation](../../../../irreducible-representation.md). Therefore $C$ is an [irreducible representation](../../../../irreducible-representation.md) of [dimension](../../../../dimension-vector-space.md) three.

For comparison useful in part (e), the [standard representation of the symmetric group](../../../../standard-representation-of-the-symmetric-group.md) has [character](../../../../character-of-a-representation.md) equal to the number of fixed letters minus one, namely $(3,1,-1,0,-1)$ in this order. Multiplication by the [sign representation](../../../../sign-representation.md) changes this [character](../../../../character-of-a-representation.md) to $(3,-1,-1,0,1)$. Thus $C$ is the [tensor product](../../../../tensor-product.md) of the [standard representation of the symmetric group](../../../../standard-representation-of-the-symmetric-group.md) with the [sign representation](../../../../sign-representation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to representation theory course of the University of Oxford](../../../split.md)
5. [Introduction to representation theory course of the University of Oxford](../../../../introduction-to-representation-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
