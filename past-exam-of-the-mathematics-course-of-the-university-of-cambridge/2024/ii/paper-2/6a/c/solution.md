<h1 id="6a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a positive equilibrium, $Y'=0$ gives $X^*=N_c$. The equations $Z'=0$ and $X^*+Y^*+Z^*=N$ then give the [Endemic equilibrium of the SIR model with demography](../../../../../../endemic-equilibrium-of-the-sir-model-with-demography.md)

$$
X^*=N_c,
\qquad
Y^*=\frac{\mu}{\mu+\nu}(N-N_c),
\qquad
Z^*=\frac{\nu}{\mu+\nu}(N-N_c),
$$

which is strictly positive when $N>N_c$.

Use $Z=N-X-Y$ to reduce to the $(X,Y)$ system. At the endemic equilibrium its Jacobian is

$$
J=\begin{pmatrix}
-\mu-\beta Y^*&-(\mu+\nu)\\
\beta Y^*&0
\end{pmatrix}.
$$

Its trace is negative and its [determinant](../../../../../../determinant.md) is $\beta Y^*(\mu+\nu)>0$. The two [eigenvalues](../../../../../../eigenvalue.md) therefore have negative real part, so the endemic equilibrium is locally asymptotically stable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6A](../../6a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
