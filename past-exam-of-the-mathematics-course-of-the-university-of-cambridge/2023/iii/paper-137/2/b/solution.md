<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Extend the [slash operator for modular forms](../../../../../../slash-operator-for-modular-forms.md) to positive-determinant matrices by

$$
(f|_k\alpha)(\tau)
=\det(\alpha)^{k/2}(c\tau+d)^{-k}f(\alpha\tau).
$$

The [double coset](../../../../../../double-coset.md)

$$
\Gamma(1)\begin{pmatrix}p&0\\0&1\end{pmatrix}\Gamma(1)
$$

has left-coset representatives

$$
\begin{pmatrix}p&0\\0&1\end{pmatrix},
\qquad
\begin{pmatrix}1&b\\0&p\end{pmatrix}
\quad(0\leq b<p).
$$

Therefore the sum of the corresponding slashes, multiplied by $p^{k/2-1}$, is exactly

$$
T_p(f)(\tau)
=p^{k-1}f(p\tau)
+\frac1p\sum_{b=0}^{p-1}f\left(\frac{\tau+b}{p}\right).
$$

Right multiplication by an element of $\Gamma(1)$ permutes these left cosets. The cocycle law for the slash operator consequently gives

$$
T_p(f)|_k\gamma=T_p(f)
\qquad(\gamma\in\Gamma(1)),
$$

so $T_p(f)$ is a weight-$k$ level-one modular function. Each displayed summand is holomorphic on $\mathfrak h$, hence so is their finite sum. This is the [Hecke operator on modular forms](../../../../../../hecke-operator.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
