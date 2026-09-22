<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $f(A)=\mu_0A+\alpha A^3-A^5$ and $V(A)=\mu_0A^2/2+\alpha A^4/4-A^6/6$. Multiplication of the stationary [reaction-diffusion equation](../../../../../../reaction-diffusion-system.md) by $A_x$ gives the first integral $A_x^2/2+V(A)=E$. A regular [front](../../../../../../front-solution.md) with finite endpoint limits has $A_x\to0$ there, and its nonzero endpoint must satisfy $f(C)=0$. Since $V(0)=0$, the first integral gives $E=0$ and $V(C)=0$. Write $q=C^2>0$. The two endpoint conditions are

$$
\mu_0+\alpha q-q^2=0,\qquad
\frac{\mu_0}{2}+\frac{\alpha q}{4}-\frac{q^2}{6}=0.
$$

Eliminating $\mu_0$ gives the [Maxwell balance for a scalar reaction-diffusion front](../../../../../../maxwell-balance-for-a-scalar-reaction-diffusion-front.md):

$$
\boxed{q=C^2=\frac{3\alpha}{4},\qquad \mu_0=-\frac{3\alpha^2}{16}.}
$$

This is a necessary condition for a stationary front, because the two spatially homogeneous states must have equal potential. It is also sufficient here. With these values, $-2V(A)=A^2(A^2-q)^2/3$. For the increasing positive front choose

$$
A_0'=\frac{1}{\sqrt3}A_0(q-A_0^2),\qquad
s=A_0^2,\qquad s'=\frac{2}{\sqrt3}s(q-s).
$$

Integrating this logistic equation and writing $\beta=2q/\sqrt3=\sqrt3\alpha/2$ gives

$$
\boxed{A_0^2(\xi)=\frac{q}{1+q e^{-\beta\xi}},\qquad \xi=x-X_0.}
$$

The positive constant multiplying the exponential is arbitrary and can be absorbed into $X_0$; choosing it to be $q$ gives the printed normalization exactly. The profile tends to zero and $q$ at the two ends and its first-order equation implies $A_0''+f(A_0)=0$. Its negative is the front to $-\sqrt q$, with the same squared profile.

Differentiation of the stationary equation produces the translation mode

$$
\mathcal L A_0'=0,\qquad
\mathcal L=\partial_x^2+\mu_0+3\alpha A_0^2-5A_0^4.
$$

The operator $\mathcal L$ is [self-adjoint](../../../../../../self-adjoint-operator.md). Twice applying [integration by parts](../../../../../../integration-by-parts.md) gives, for $R$ with vanishing boundary Wronskian,

$$
\int_{-\infty}^{\infty}A_0'\mathcal LR\,dx
=\left[A_0'R'-A_0''R\right]_{-\infty}^{\infty}
+\int_{-\infty}^{\infty}R\mathcal LA_0'\,dx=0.
$$

Bounded $R,R'$ suffice, because the derivatives of the front decay exponentially. This proves the identity as a [Fredholm solvability condition](../../../../../../fredholm-solvability-condition.md) associated with translation invariance.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
