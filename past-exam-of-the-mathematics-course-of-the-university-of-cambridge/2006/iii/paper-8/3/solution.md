<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the [Volterra integration operator](../../../../../volterra-operator.md), [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
|Jf(x)|^2=\left|\int_0^x f(t)\,dt\right|^2
\leq x\int_0^x|f(t)|^2\,dt.
$$

Integrating and reversing the order yields

$$
\|Jf\|_2^2\leq\int_0^1\frac{1-t^2}{2}|f(t)|^2\,dt
\leq\frac12\|f\|_2^2.
$$

Thus $J$ is bounded, with $\|J\|\leq1/\sqrt2$. Since $f\in L^2(0,1)\subseteq L^1(0,1)$, $Jf$ is absolutely continuous and $(Jf)'=f$ almost everywhere. If $Jf=0$ as an $L^2$ element, its continuous representative is zero everywhere, so its [derivative](../../../../../derivative.md) is zero almost everywhere. Hence **$J$ is one-to-one**.

Its range is exactly $\{u\in H^1(0,1):u(0)=0\}$, and $Au=iu'$. This contains the smooth compactly supported functions in $(0,1)$, so $A$ is a [densely defined operator](../../../../../densely-defined-operator.md). Closedness can also be seen directly: if $u_n\to u$ and $Au_n\to v$ in $L^2$, then $u_n=J(-iAu_n)\to J(-iv)$, giving $u=J(-iv)\in D(A)$ and $Au=v$.

For every $\lambda\in\mathbb C$,

$$
(\lambda I-A)J=\lambda J-iI.
$$

If $\lambda\ne0$, the allowed fact $\sigma(J)=\{0\}$ makes $J-(i/\lambda)I$ invertible. At $\lambda=0$, $\lambda J-iI=-iI$ is invertible too. Thus the [bounded operator](../../../../../continuous-linear-operator.md)

$$
R_\lambda=J(\lambda J-iI)^{-1}
$$

has range in $D(A)$ and is a two-sided inverse of $\lambda I-A$. Equivalently, solving the initial-value differential equation gives

$$
R_\lambda h(x)=i\int_0^x e^{-i\lambda(x-s)}h(s)\,ds.
$$

This is bounded for every fixed $\lambda$ on the finite interval. Therefore [Volterra inverse differentiation has empty spectrum](../../../../../volterra-inverse-differentiation-has-empty-spectrum.md):

$$
\boxed{\sigma(A)=\varnothing.}
$$

The familiar nonempty-spectrum theorem for bounded operators does not apply to this unbounded operator.

The subspace $H_0$ is the kernel of the bounded functional $f\mapsto Jf(1)=\int_0^1f$, so it is closed. Its image under $J$ is

$$
D(A_0)=\{u\in H^1(0,1):u(0)=u(1)=0\}=H_0^1(0,1),
$$

the [zero-trace Sobolev space](../../../../../zero-trace-sobolev-space.md). If $u_n\in D(A_0)$, $u_n\to u$ and $A_0u_n\to v$, then $-iA_0u_n\in H_0$ converges to $-iv\in H_0$, and $u=J(-iv)\in D(A_0)$. Thus $A_0$ is closed. It is densely defined because it also contains the smooth compactly supported functions.

For $u,v\in D(A_0)$, [integration by parts](../../../../../integration-by-parts.md) and their zero endpoint traces give

$$
\langle A_0u,v\rangle
=i\int_0^1u'\overline v
=i[u\overline v]_0^1-i\int_0^1u\overline{v'}
=\langle u,A_0v\rangle.
$$

Hence **$A_0$ is closed and symmetric**.

For any $v\in C^1([0,1])$, the same formula gives $\langle A_0u,v\rangle=\langle u,iv'\rangle$, with no endpoint term because $u$ vanishes there. Consequently $v\in D(A_0^*)$ and $A_0^*v=iv'$, proving the requested inclusion. In fact, testing against compactly supported smooth $u$ shows that every element of $D(A_0^*)$ has [weak derivative](../../../../../weak-derivative.md) in $L^2$; conversely the integration-by-parts formula applies to every $v\in H^1(0,1)$. Thus

$$
D(A_0^*)=H^1(0,1),\qquad A_0^*v=iv',
$$

with no boundary restrictions.

For any $\lambda\in\mathbb C$, the nonzero function $v_\lambda(x)=e^{-i\lambda x}$ belongs to this domain and satisfies $iv_\lambda'=\lambda v_\lambda$. Conversely this first-order equation has only scalar multiples of that exponential. Therefore

$$
\boxed{\sigma_p(A_0^*)=\mathbb C,\qquad
\ker(A_0^*-\lambda I)=\operatorname{span}\{e^{-i\lambda x}\}.}
$$

For any $\lambda$, the adjoint eigenfunction with [eigenvalue](../../../../../eigenvalue.md) $\overline\lambda$ annihilates $\operatorname{Ran}(\lambda I-A_0)$, so this range is not all of $H$. Explicitly the resolvent equation with zero initial value has the solution $R_\lambda h$ above, and its endpoint value is zero exactly when

$$
\int_0^1e^{i\lambda s}h(s)\,ds=0.
$$

Thus the range is a proper closed hyperplane for every $\lambda$. This proves that the [two-endpoint symmetric derivative has whole complex spectrum](../../../../../two-endpoint-symmetric-derivative-has-whole-complex-spectrum.md):

$$
\boxed{\sigma(A_0)=\mathbb C.}
$$

There are no [eigenvalues](../../../../../eigenvalue.md) of $A_0$ itself: the eigenfunction equation together with $u(0)=0$ forces the exponential coefficient to vanish. The operator is symmetric but not self-adjoint, since its adjoint has a strictly larger domain; symmetry alone does not force a real [spectrum](../../../../../spectrum-functional-analysis.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
