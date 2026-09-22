<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Along the affine null geodesic write $\Phi'=U^a\nabla_a\Phi$. Contracting the scalar stress tensor with $U^aU^b$ removes every term proportional to $g_{ab}$. Since $G_{ab}=T_{ab}$ and

$$
U^aU^b\nabla_a(\Phi\nabla_b\Phi)
=\frac d{d\lambda}(\Phi\Phi')
=(\Phi')^2+\Phi\Phi'',
$$

one obtains

$$
(1-\xi\Phi^2)T_{ab}U^aU^b
=(1-2\xi)(\Phi')^2-2\xi\Phi\Phi''.
$$

Put $D=1-\xi\Phi^2$. An integration by parts gives

$$
\int_{-\infty}^{\infty}T_{ab}U^aU^b\,d\lambda
=\left[-\frac{2\xi\Phi\Phi'}D\right]_{-\infty}^{\infty}
+\int_{-\infty}^{\infty}
\frac{1+\xi(4\xi-1)\Phi^2}{D^2}(\Phi')^2\,d\lambda.
$$

The stated endpoint condition kills the boundary term. If $\xi<0$, then $D>0$ and $\xi(4\xi-1)>0$, so the remaining integrand is nonnegative. Consequently this nonminimally coupled scalar satisfies the [averaged null energy condition](../../../../../../../averaged-null-energy-condition.md):

$$
\boxed{\int_{-\infty}^{\infty}T_{ab}U^aU^b\,d\lambda\geq0}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 311](../../../../paper-311-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
