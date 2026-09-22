<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the [hyperbolic toral automorphism](../../../../../../hyperbolic-toral-automorphism.md) as $T_A([v])=[Av]$ on $\mathbb T^2=\mathbb R^2/\mathbb Z^2$, where $A\in\mathrm{GL}(2,\mathbb Z)$. Its [determinant](../../../../../../determinant.md) is $\pm1$. The [eigenvalues](../../../../../../eigenvalue.md) cannot be a nonreal conjugate pair: their product would have [absolute value](../../../../../../absolute-value.md) one, forcing each to have [absolute value](../../../../../../absolute-value.md) one, contrary to hyperbolicity. The same product condition and hyperbolicity imply two distinct real [eigenvalues](../../../../../../eigenvalue.md), labelled so that

$$
0<|\lambda_s|<1<|\lambda_u|,qquad |\lambda_s\lambda_u|=1.
$$

We will prove

$$
\boxed{h_{\mathrm{top}}(T_A)=\log|\lambda_u|.}
$$

This is the [entropy of a hyperbolic toral automorphism](../../../../../../entropy-of-a-hyperbolic-toral-automorphism.md); the [absolute value](../../../../../../absolute-value.md) is important when the expanding [eigenvalue](../../../../../../eigenvalue.md) is negative.

Choose real [eigenvectors](../../../../../../eigenvector.md) $v_s,v_u$ and the adapted [norm](../../../../../../norm.md) $\|a v_s+b v_u\|_*=\max(|a|,|b|)$. Its quotient [metric](../../../../../../metric.md) on the [torus](../../../../../../torus.md) is

$$
d([v],[w])=\min_{\ell\in\mathbb Z^2}\|v-w-\ell\|_*.
$$

It is a [compatible metric](../../../../../../compatible-metric.md), so part (a) allows its use. Let $\rho=\min_{0\ne\ell\in\mathbb Z^2}\|\ell\|_*>0$ and $D=\|A\|_*=|\lambda_u|$. Fix $\epsilon>0$ small enough that $2\epsilon<\rho$ and $(D+1)\epsilon<\rho$.

If $[v]$ lies in the [Bowen ball](../../../../../../bowen-ball.md) $B_n(0,\epsilon)$, each $T_A^k[v]$ has a unique lift $z_k$ with $\|z_k\|_*<\epsilon$. Uniqueness follows because two such lifts differ by a lattice vector of [norm](../../../../../../norm.md) less than $2\epsilon<\rho$. Moreover, $z_{k+1}-Az_k$ is a lattice vector, and

$$
\|z_{k+1}-Az_k\|_*<(D+1)\epsilon<\rho.
$$

It must be zero. Thus $z_k=A^kz_0$: there is no hidden lattice jump between successive lifted iterates.

Write $z_0=a v_s+b v_u$. The simultaneous bounds $\|A^kz_0\|_*<\epsilon$ for $0\leq k<n$ are exactly

$$
|a|<\epsilon,qquad |b|<\epsilon|\lambda_u|^{-(n-1)}.
$$

The stable coordinate is largest at time zero and the unstable coordinate at time $n-1$. Conversely, every vector in this rectangle satisfies all the [Bowen ball](../../../../../../bowen-ball.md) bounds. The quotient is injective on this rectangle by $2\epsilon<\rho$. If $J=|\det(v_s,v_u)|$, its normalized [Haar measure](../../../../../../haar-measure.md) is therefore

$$
\nu(B_n(0,\epsilon))=4J\epsilon^2|\lambda_u|^{-(n-1)}.
$$

The quotient [metric](../../../../../../metric.md) is translation invariant and $T_A$ is linear, so $d_n(x,y)=d_n(0,y-x)$; every [Bowen ball](../../../../../../bowen-ball.md) has this same [measure](../../../../../../measure.md), independently of its centre.

Take an $\epsilon$-[separated set](../../../../../../separated-subset-of-a-metric-space.md) of largest cardinality $s_n(d,\epsilon)$. It is maximal under inclusion, so its radius-$\epsilon$ [Bowen balls](../../../../../../bowen-ball.md) cover the [torus](../../../../../../torus.md): a point outside all these balls could be added. The covering bound gives

$$
s_n(d,\epsilon)\geq\frac1{4J\epsilon^2}|\lambda_u|^{n-1}.
$$

Its radius-$\epsilon/2$ [Bowen balls](../../../../../../bowen-ball.md) are disjoint, by the [triangle inequality](../../../../../../triangle-inequality.md) for $d_n$. Their measures sum to at most one, giving

$$
s_n(d,\epsilon)\leq\frac1{J\epsilon^2}|\lambda_u|^{n-1}.
$$

Taking logarithms, dividing by $n$, and letting $n\to\infty$ yields $h_d(T_A,\epsilon)=\log|\lambda_u|$ for every sufficiently small $\epsilon$. The limit as $\epsilon\downarrow0$ proves the answer. Contraction in the stable direction contributes no exponential growth; only expansion in the unstable direction does.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
