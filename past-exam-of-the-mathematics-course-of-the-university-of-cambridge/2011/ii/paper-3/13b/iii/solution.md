<h1 id="13b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The background has $\nabla a_0=0$, so the linear chemotaxis term is $-\chi_0n_0\nabla^2\xi$; derivatives of $\chi$ multiply products of disturbances and do not enter at first order. For a [normal mode](../../../../../../normal-mode.md) with $\nabla^2=-k^2$ and time dependence $e^{pt}$, put $q=k^2$. Then

$$
p\begin{pmatrix}\eta\\\xi\end{pmatrix}=\begin{pmatrix}-A-q&\chi_0n_0q\\\beta&-\gamma-Dq\end{pmatrix}\begin{pmatrix}\eta\\\xi\end{pmatrix},
$$

and the [characteristic polynomial](../../../../../../characteristic-polynomial.md) is

$$
\boxed{p^2+[A+\gamma+(1+D)q]p+Dq^2+(AD+\gamma-\beta\chi_0n_0)q+A\gamma=0.}
$$

Its linear coefficient is positive for every $q\geq0$. Thus instability occurs exactly when its constant term $Q(q)$ is negative: the roots are then real with opposite signs. The positive quadratic $Q$ is negative somewhere on $q>0$ precisely when

$$
\beta\chi_0n_0-AD-\gamma>2\sqrt{DA\gamma}.
$$

Therefore

$$
\boxed{\beta\chi_0n_0>2\alpha n_0^2D+\gamma+2\sqrt{2D\alpha n_0^2\gamma}.}
$$

At equality the neutral wavenumber is $q_c=\sqrt{A\gamma/D}$ and $p=0$. Above threshold the unstable band is $q_-<k^2<q_+$, where

$$
q_\pm=\frac{B\pm\sqrt{B^2-4DA\gamma}}{2D},\qquad B=\beta\chi_0n_0-AD-\gamma.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [13B](../../13b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
