<h1 id="41c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $H$ is diagonalizable, write $H=V\Lambda V^{-1}$. Then

$$
z^{(k)}=H^kz^{(0)}=V\Lambda^kV^{-1}z^{(0)}.
$$

If the [spectral radius](../../../../../../spectral-radius.md) $\rho(H)<1$, every eigenvalue satisfies $|\lambda_i|<1$, so $\Lambda^k\to0$ and hence $z^{(k)}\to0$ for every initial vector. Conversely, taking $z^{(0)}$ to be an eigenvector of any eigenvalue $\lambda$ shows that convergence for every initial vector forces $\lambda^k\to0$, hence $|\lambda|<1$. Therefore

$$
\boxed{z^{(k)}\to0\text{ for all }z^{(0)}
\quad\Longleftrightarrow\quad \rho(H)<1}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41C](../../41c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
