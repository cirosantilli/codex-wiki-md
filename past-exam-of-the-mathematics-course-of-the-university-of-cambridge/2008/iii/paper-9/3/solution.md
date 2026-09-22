<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use additive notation and fix [Haar measure](../../../../../haar-measure.md) $m$ on $G$. A [continuous unitary character](../../../../../continuous-unitary-character.md) is a continuous homomorphism $\chi:G\to\mathbb T$. With the convention

$$
\widehat f(\chi)=\int_G f(t)\overline{\chi(t)}\,dm(t),\qquad (f*g)(t)=\int_G f(y)g(t-y)\,dm(y),
$$

the [Fubini theorem](../../../../../fubini-s-theorem.md) and the character identity imply $\widehat{f*g}(\chi)=\widehat f(\chi)\widehat g(\chi)$. Also $|\widehat f(\chi)|\leq\|f\|_1$, and choosing $f=\chi a$ for a nonzero nonnegative $a\in C_c(G)$ shows that evaluation at $\chi$ is a nonzero functional. Thus each character gives a [character of an algebra](../../../../../character-of-an-algebra.md) on the [L1 convolution algebra](../../../../../l1-convolution-algebra.md). Here a multiplicative linear functional means a [nonzero multiplicative linear functional](../../../../../character-of-an-algebra.md); the zero functional must be excluded for the claimed bijection.

Conversely, let $\varphi$ be such a functional. It is automatically bounded with $|\varphi(f)|\leq\|f\|_1$: extend it to the [unitization of an algebra](../../../../../unitization-of-an-algebra.md) by $\widetilde\varphi(f+z1)=\varphi(f)+z$. If $|z|>\|f\|_1$, the [Neumann series](../../../../../neumann-series.md) makes $z1-f$ invertible, so its image under the unital homomorphism cannot be zero. Hence $\varphi(f)$ cannot lie outside the norm disc.

Choose $a\in L^1(G)$ with $\varphi(a)\neq0$, and let $T_xa(t)=a(t-x)$. The Abelian translation identities $(T_xa)*b=a*(T_xb)$ give

$$
\varphi(T_xa)\varphi(b)=\varphi(a)\varphi(T_xb).
$$

Therefore, defining $c(x)=\varphi(T_xa)/\varphi(a)$, one has $\varphi(T_xb)=c(x)\varphi(b)$ for every $b$. Applying this to two successive translations gives $c(x+y)=c(x)c(y)$ and $c(0)=1$. By [translation continuity in Lp on a locally compact group](../../../../../translation-continuity-in-lp-on-a-locally-compact-group.md), $c$ is continuous. It is uniformly bounded by $\|a\|_1/|\varphi(a)|$; applying this bound to $c(nx)=c(x)^n$ for positive and negative integers forces $|c(x)|=1$. Thus $\chi(x)=\overline{c(x)}$ is a [continuous unitary character](../../../../../continuous-unitary-character.md).

The [Bochner integral](../../../../../bochner-integral.md) identity $a*b=\int_G b(y)T_ya\,dm(y)$ holds in $L^1$, since $\|T_ya\|_1=\|a\|_1$. Applying the bounded functional yields

$$
\varphi(a)\varphi(b)=\varphi(a*b)=\varphi(a)\int_G b(y)c(y)\,dm(y).
$$

Cancel $\varphi(a)\neq0$ to obtain the required correspondence

$$
\boxed{\varphi(b)=\int_Gb(y)\overline{\chi(y)}\,dm(y)=\widehat b(\chi).}
$$

The recovery formula $\overline{\chi(x)}=\varphi(T_xa)/\varphi(a)$ proves uniqueness. These functionals have norm exactly one, since $b=\chi a$ with $a\geq0$ and $\int a=1$ has $\|b\|_1=\varphi(b)=1$.

For the topology, identify the [Pontryagin dual group](../../../../../pontryagin-dual-group.md) with these functionals and give it the [Gelfand topology](../../../../../gelfand-topology.md), namely pointwise convergence of $\widehat f(\chi)$ for every $f\in L^1$. If a net $\chi_\lambda$ converges to $\gamma$ uniformly on every compact subset of $G$, then for $f\in C_c(G)$,

$$
|\widehat f(\chi_\lambda)-\widehat f(\gamma)|\leq\|f\|_1\sup_{x\in\operatorname{supp}f}|\chi_\lambda(x)-\gamma(x)|\longrightarrow0.
$$

Density of $C_c$ in $L^1$ and the uniform functional norm bound one extend this convergence to every $f\in L^1$.

Conversely, suppose convergence in the [Gelfand topology](../../../../../gelfand-topology.md) and choose $a$ with $\widehat a(\gamma)\neq0$. For compact $K\subseteq G$, the set $\{T_xa:x\in K\}$ is compact in $L^1$ by [translation continuity in Lp on a locally compact group](../../../../../translation-continuity-in-lp-on-a-locally-compact-group.md). Evaluation convergence is uniform on this compact set: a finite $\delta$-net reduces its supremum to finitely many convergent evaluations plus $2\delta$, using the common functional norm one. Thus

$$
\sup_{x\in K}|\widehat{T_xa}(\chi_\lambda)-\widehat{T_xa}(\gamma)|\longrightarrow0.
$$

Now $\widehat{T_xa}(\chi)=\overline{\chi(x)}\widehat a(\chi)$, and $\widehat a(\chi_\lambda)\to\widehat a(\gamma)\neq0$. Dividing this identity proves $\sup_{x\in K}|\chi_\lambda(x)-\gamma(x)|\to0$. Hence the [Gelfand topology](../../../../../gelfand-topology.md) is exactly the [compact-open topology](../../../../../compact-open-topology.md), with the requested [neighbourhood basis](../../../../../neighbourhood-basis.md)

$$
\boxed{U(\gamma;K,\epsilon)=\{\chi\in\widehat G:|\chi(x)-\gamma(x)|<\epsilon\text{ for every }x\in K\}.}
$$

For compact $K$, the continuous difference attains its maximum, so this strict pointwise inequality on $K$ is equivalent to a strict uniform bound. Finite intersections contain another such set by taking the union of the compact sets and the minimum of the tolerances.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
