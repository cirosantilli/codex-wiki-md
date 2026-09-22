<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For a [bounded linear functional](../../../../continuous-linear-functional.md) on a unital C\*-algebra, the state criterion is

$$
\boxed{x(1_A)=\|x\|=1.}
$$

Equivalently it is positive and takes the unit to one.

In the [Gelfand–Naimark–Segal construction](../../../../gelfand-naimark-segal-construction.md), set $N_x=\{b:x(b^*b)=0\}$. This is a [left ideal](../../../../left-ideal.md). Give $A/N_x$ the [inner product](../../../../inner-product-split.md) $\langle[b],[c]\rangle=x(c^*b)$, linear in the first variable, and complete it to a [Hilbert space](../../../../hilbert-space-split.md) $H_x$. Left multiplication gives the bounded \*-representation $\pi_x(a)[b]=[ab]$. The vector $\xi=[1_A]$ is cyclic and satisfies $x(a)=\langle\pi_x(a)\xi,\xi\rangle$.

The Hermitian matrix $\rho$ has eigenvalues $\lambda_\pm=1/2\pm|\alpha|$ and [trace](../../../../matrix-trace.md) one. In an [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md) $v_+,v_-$,

$$
x_\rho(a)=\lambda_+\langle av_+,v_+\rangle+\lambda_-\langle av_-,v_-\rangle.
$$

If $|\alpha|\leq1/2$, both weights are nonnegative and sum to one, so this functional is positive and normalized, hence a state. If $|\alpha|>1/2$, evaluating on the positive [rank](../../../../rank-one-quadratic-form.md)-one projection onto the negative-[eigenvalue](../../../../eigenvalue.md) eigenspace gives a negative value, so it is not a state. Therefore

$$
\boxed{x_\rho\text{ is a state}\iff|\alpha|\leq1/2.}
$$

To obtain the representation dimension, cyclicity of [trace](../../../../matrix-trace.md) gives

$$
x_\rho(b^*b)=\operatorname{Tr}(\rho b^*b)=\|b\rho^{1/2}\|_{\mathrm{HS}}^2.
$$

Thus $A/N_{x_\rho}$ identifies isometrically with the matrix space $\{b\rho^{1/2}:b\in M_2(\mathbb C)\}$, with left multiplication as the representation. If $r=\operatorname{rank}\rho$, this space consists, after a [unitary](../../../../unitary-connection.md) change of basis, of arbitrary first $r$ columns and zero remaining columns. Its complex dimension is $2r$. It is already complete because it is finite-dimensional. [Rank](../../../../rank-one-quadratic-form.md) is one at $|\alpha|=1/2$ and two at $|\alpha|<1/2$, proving

$$
\boxed{\dim H_{x_\rho}=2\text{ at }|\alpha|=1/2,\qquad\dim H_{x_\rho}=4\text{ at }|\alpha|<1/2.}
$$

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
