<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

Reading the coefficients of the [linear map](../../../../../linear-map.md) gives

$$
\boxed{A=\begin{pmatrix}e^{i\theta}&1\\1&e^{-i\phi}\end{pmatrix},\qquad
\det A=e^{i(\theta-\phi)}-1
=2i\sin\!\left(\frac{\theta-\phi}2\right)e^{i(\theta-\phi)/2}.}
$$

Under the inverse identification, the four standard real basis vectors map respectively to $(1,0)$, $(i,0)$, $(0,1)$ and $(0,i)$ in $\mathbb C^2$. Applying $A$ and taking real and imaginary parts therefore gives the columns

$$
\begin{aligned}
\mathcal B e_1&=(\cos\theta,\sin\theta,1,0)^T,\\
\mathcal B e_2&=(-\sin\theta,\cos\theta,0,1)^T,\\
\mathcal B e_3&=(1,0,\cos\phi,-\sin\phi)^T,\\
\mathcal B e_4&=(0,1,\sin\phi,\cos\phi)^T.
\end{aligned}
$$

Thus **the real [matrix](../../../../../matrix.md) is**

$$
\boxed{B=\begin{pmatrix}
\cos\theta&-\sin\theta&1&0\\
\sin\theta&\cos\theta&0&1\\
1&0&\cos\phi&\sin\phi\\
0&1&-\sin\phi&\cos\phi
\end{pmatrix}.}
$$

For verification, write its blocks as $\begin{pmatrix}R_\theta&I\\I&R_{-\phi}\end{pmatrix}$, where $R_\psi$ is the planar rotation [matrix](../../../../../matrix.md). Block elimination gives $\det B=\det(R_{\theta-\phi}-I)=2-2\cos(\theta-\phi)$. Therefore **the determinant identity is**

$$
\boxed{\det B=4\sin^2\!\left(\frac{\theta-\phi}2\right)=|\det A|^2.}
$$

This is an instance of the [realification determinant identity](../../../../../realification-determinant-identity.md). The identification is real-linear; it is not an identification of complex vector-space dimensions.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
