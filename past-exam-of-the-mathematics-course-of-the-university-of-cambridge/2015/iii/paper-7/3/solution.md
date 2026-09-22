<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a densely defined operator $A$ on a complex [Hilbert space](../../../../../hilbert-space-split.md), [unbounded self-adjointness](../../../../../unbounded-self-adjoint-operator.md) means equality $A=A^*$ including equality of the [operator domains](../../../../../operator-domain.md). Symmetry alone asserts only $A\subseteq A^*$ and is insufficient. Use an [inner product](../../../../../inner-product.md) linear in its first argument. If $\operatorname{Im}z\ne0$, symmetry gives

$$
\|(A-z)u\|\,\|u\|\geq|\operatorname{Im}\langle(A-z)u,u\rangle|=|\operatorname{Im}z|\|u\|^2.
$$

Thus $A-z$ is bounded below. Since $A$ is closed, its range is closed; its orthogonal complement is $\ker(A^*-\overline z)=\ker(A-\overline z)=0$, so the range is also dense and therefore all of $H$. The inverse is bounded by $|\operatorname{Im}z|^{-1}$. The [nonreal resolvent estimate for a self-adjoint operator](../../../../../nonreal-resolvent-estimate-for-a-self-adjoint-operator.md) proves **$\sigma(A)\subseteq\mathbb R$**.

For bounded [self-adjoint](../../../../../self-adjoint-operator.md) $T$, its [numerical range of an operator](../../../../../numerical-range-of-an-operator.md) and [numerical radius](../../../../../numerical-radius.md) are

$$
W(T)=\{\langle Tu,u\rangle:\|u\|=1\},\qquad w(T)=\sup_{\|u\|=1}|\langle Tu,u\rangle|.
$$

Every number in $W(T)$ is real. If $z\notin\overline{W(T)}$, its distance $\delta$ from that closed set is positive, and $\|(T-z)u\|\geq\delta\|u\|$. The same bound applies to $T-\overline z$, so the range is dense as well as closed and $T-z$ has a bounded inverse. Hence the [numerical-range spectral enclosure](../../../../../numerical-range-spectral-enclosure.md) is

$$
\boxed{\sigma(T)\subseteq\overline{W(T)}\subseteq\mathbb R.}
$$

The closure is necessary in infinite dimension: the endpoints of the numerical range need not themselves be attained.

Put $\beta=\sup W(T)$ and $B=\beta I-T$, a bounded [positive semidefinite operator](../../../../../positive-operator.md). Choose [unit vectors](../../../../../unit-vector.md) $u_n$ with $\langle Bu_n,u_n\rangle\to0$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) for the positive form $\langle B\cdot,\cdot\rangle$ implies

$$
\|Bu_n\|^2=\sup_{\|v\|=1}|\langle Bu_n,v\rangle|^2\leq\|B\|\langle Bu_n,u_n\rangle\longrightarrow0.
$$

Therefore $\beta$ is an [approximate eigenvalue](../../../../../approximate-eigenvalue.md). Apply the same argument to $T-\alpha I$, where $\alpha=\inf W(T)$, to get the other endpoint. This proves the [numerical-range endpoint approximate-eigenvalue theorem](../../../../../numerical-range-endpoint-approximate-eigenvalue-theorem.md). Each endpoint is in the [spectrum](../../../../../spectrum-functional-analysis.md): a bounded inverse would forbid [unit vectors](../../../../../unit-vector.md) with vanishing residual.

If an [unbounded self-adjoint operator](../../../../../unbounded-self-adjoint-operator.md) $A$ is positive semidefinite, then for every real $z<0$, $\|(A-z)u\|\geq(-z)\|u\|$. The range argument above again proves invertibility, excluding negative values from the [spectrum](../../../../../spectrum-functional-analysis.md). For the converse, suppose $\sigma(A)\subseteq[0,\infty)$. Its [resolvent operator](../../../../../resolvent-of-an-operator.md) $R=(I+A)^{-1}$ is bounded and self-adjoint. The [resolvent spectral mapping identity](../../../../../resolvent-spectral-mapping-identity.md) puts $\sigma(R)\subseteq[0,1]$: for $w\ne0$, the relevant spectral parameter of $A$ is $1/w-1$, and nonreal values are excluded by self-adjointness. By the endpoint result just proved, $W(R)\subseteq[0,1]$. Positive-form [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) then gives

$$
\|Rf\|^2\leq\langle Rf,f\rangle\sup_{\|v\|=1}\langle Rv,v\rangle\leq\langle Rf,f\rangle.
$$

For $u=Rf\in D(A)$ this yields $\langle Au,u\rangle=\langle f-Rf,Rf\rangle\geq0$. Thus the [spectral positivity criterion for a self-adjoint operator](../../../../../spectral-positivity-criterion-for-a-self-adjoint-operator.md) is

$$
\boxed{A\geq0\quad\Longleftrightarrow\quad\sigma(A)\subseteq[0,\infty).}
$$

This resolvent proof uses the bounded numerical-range result to handle the full unbounded domain.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
