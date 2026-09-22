<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [modular discriminant](../../../../../../modular-discriminant.md) has the convergent product

$$
\Delta(\tau)=q\prod_{n\geq1}(1-q^n)^{24},\qquad q=e^{2\pi i\tau},
$$

is a weight-twelve level-one [cusp form](../../../../../../cusp-form.md), and has order one at infinity. Applying the [degeneracy map for cusp forms](../../../../../../degeneracy-map-for-cusp-forms.md) with $M=1,N=D=p$ gives $\boxed{\Delta(p\tau)\in S_{12}(\Gamma_0(p))}$. The original form $\Delta$ is also a [cusp form](../../../../../../cusp-form.md) on this subgroup.

There are precisely two [modular cusps](../../../../../../cusp-of-a-modular-group.md) for prime level, represented by infinity and zero. To see this directly, write a rational cusp as $a/c$ in lowest terms. If $p\mid c$, completing $(a,c)^T$ to a determinant-one matrix gives a member of $\Gamma_0(p)$ taking infinity there. If $p\nmid c$, the equation $Ac-aC=1$ has a solution with $p\mid C$: adjust a Bézout solution modulo $p$, using the invertibility of $c$. The matrix $\begin{pmatrix}A&a\\C&c\end{pmatrix}$ then lies in $\Gamma_0(p)$ and takes zero there. The two classes are distinct because their denominator divisibility is preserved by the group.

At infinity the [cusp width](../../../../../../width-of-a-cusp.md) is one, so $q$ is the local parameter. The products start with $q$ and $q^p$, giving orders one and $p$. At zero use $S=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$. Since $ST^hS^{-1}=\begin{pmatrix}1&0\\-h&1\end{pmatrix}$, the [cusp width](../../../../../../width-of-a-cusp.md) is $p$ and the parameter is $q_0=e^{2\pi i\tau/p}$. The weight-twelve inversion law of the [modular discriminant](../../../../../../modular-discriminant.md) gives

$$
\Delta[ S]_{12}(\tau)=\Delta(\tau),\qquad
\big(\Delta(p\tau)\big)[ S]_{12}=\tau^{-12}\Delta(-p/\tau)=p^{-12}\Delta(\tau/p).
$$

Here determinant one makes the printed and ordinary [slash operators for modular forms](../../../../../../slash-operator-for-modular-forms.md) agree. In terms of $q_0$, the leading terms are $q_0^p$ and $p^{-12}q_0$. Hence the [prime-level cusp orders of discriminant degeneracy forms](../../../../../../prime-level-cusp-orders-of-discriminant-degeneracy-forms.md) are

$$
\boxed{\begin{array}{c|cc}&\Delta(\tau)&\Delta(p\tau)\\\hline\infty&1&p\\0&p&1\end{array}.}
$$

The scalar $p^{-12}$ changes no order of vanishing.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
