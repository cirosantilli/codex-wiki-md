<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) are

$$
\rho(\zeta)=\zeta^2-(1+a)\zeta+a=(\zeta-1)(\zeta-a)
$$

and

$$
\sigma(\zeta)=\frac1{12}\bigl((5+a)\zeta^2+8(1-a)\zeta-(1+5a)\bigr).
$$

For the [order conditions for a linear multistep method](../../../../../../order-conditions-for-a-linear-multistep-method.md), put $\alpha=(a,-1-a,1)$ and $\beta=(-(1+5a)/12,,8(1-a)/12,,(5+a)/12)$. The defects

$$
C_q=\sum_{j=0}^2\alpha_jj^q-q\sum_{j=0}^2\beta_jj^{q-1}
$$

vanish for $q=0,1,2,3$, while

$$
C_4=-(a+1),
\qquad
C_5=-\frac{13a+17}{3}.
$$

Therefore

$$
\boxed{
\text{order}=\begin{cases}
4,&a=-1,\\
3,&a\ne-1.
\end{cases}}
$$

Indeed, at $a=-1$ one has $C_4=0$ but $C_5=-4/3\ne0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
