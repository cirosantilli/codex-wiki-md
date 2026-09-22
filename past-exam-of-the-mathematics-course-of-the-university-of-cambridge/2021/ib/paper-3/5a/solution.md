<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

The function $f$ has zero mean and its cosine coefficients vanish:

$$
a_0=0,\qquad a_n=0.
$$

Its sine coefficients are

$$
b_n=\frac1\pi\left(\int_0^\pi\sin(n\theta)\,d\theta
-\int_\pi^{2\pi}\sin(n\theta)\,d\theta\right),
$$

so

$$
\boxed{
b_n=\begin{cases}
\dfrac4{\pi n},&n\text{ odd},\\
0,&n\text{ even}.
\end{cases}}
$$

Away from the corners, $F'=f$. Differentiating the [Fourier series](../../../../../fourier-series-split.md) shows that $nB_n=a_n$ and $-nA_n=b_n$. Also,

$$
A_0=\frac1\pi\int_0^{2\pi}F(\theta)\,d\theta=\pi.
$$

Consequently

$$
\boxed{B_n=0,\qquad
A_n=\begin{cases}
-\dfrac4{\pi n^2},&n\text{ odd},\\
0,&n\text{ even},
\end{cases}}
$$

and

$$
F(\theta)=\frac\pi2-\frac4\pi
\sum_{r=0}^\infty\frac{\cos((2r+1)\theta)}{(2r+1)^2}.
$$

Evaluating the series for $f$ at $\theta=\pi/2$ gives the [Leibniz formula for π](../../../../../leibniz-formula-for-pi.md),

$$
\boxed{\sum_{r=0}^\infty\frac{(-1)^r}{2r+1}=\frac\pi4}.
$$

Evaluating the continuous Fourier series for $F$ at $\theta=0$ gives

$$
0=\frac\pi2-\frac4\pi\sum_{r=0}^\infty\frac1{(2r+1)^2},
$$

and hence

$$
\boxed{\sum_{r=0}^\infty\frac1{(2r+1)^2}=\frac{\pi^2}{8}}.
$$

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
