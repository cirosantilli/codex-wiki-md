<h1 id="section-a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the nodes $c_1=\alpha$ and $c_2=1$, the [Lagrange basis](../../../../../../../lagrange-polynomial.md) is

$$
\ell_1(t)=\frac{1-t}{1-\alpha},
\qquad
\ell_2(t)=\frac{t-\alpha}{1-\alpha}.
$$

Direct integration gives

$$
a_{ij}=\int_0^{c_i}\ell_j(t)\,dt
$$

and therefore

$$
A=\begin{pmatrix}
\dfrac{\alpha(2-\alpha)}{2(1-\alpha)}&-\dfrac{\alpha^2}{2(1-\alpha)}\\[6pt]
\dfrac1{2(1-\alpha)}&\dfrac{1-2\alpha}{2(1-\alpha)}
\end{pmatrix}.
$$

The [collocation Runge-Kutta method](../../../../../../../collocation-runge-kutta-method.md) also requires

$$
b_j=\int_0^1\ell_j(t)\,dt,
\qquad
b^T=\left(\frac1{2(1-\alpha)},\frac{1-2\alpha}{2(1-\alpha)}\right).
$$

This exposes a sign error in the printed tableau: its lower-right entry is shown as $(-1+2\alpha)/[2(1-\alpha)]$. With $1-2\alpha$ in that position, the tableau is exactly the claimed collocation method. Taken literally, the printed weights satisfy $b^T\mathbf1=\alpha/(1-\alpha)$, so the method is not even consistent unless $\alpha=1/2$ and cannot be a collocation method for general $\alpha$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Section A](../../../section-a.md)
4. [Paper 341](../../../../paper-341-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
