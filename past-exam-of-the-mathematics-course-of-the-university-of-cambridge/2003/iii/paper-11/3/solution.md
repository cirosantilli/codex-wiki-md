<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $G$ be locally compact, Abelian and Hausdorff, and fix a [Haar measure](../../../../../haar-measure.md). Write $T_xf(y)=f(x^{-1}y)$ and use [convolution](../../../../../convolution.md)

$$
(f*g)(y)=\int_G f(x)g(x^{-1}y)\,dx.
$$

The [L1 group algebra](../../../../../l1-convolution-algebra.md) is a commutative [Banach algebra](../../../../../banach-algebra-split.md). Here a [group character](../../../../../continuous-unitary-character.md) means a continuous [homomorphism](../../../../../homomorphism.md) $\chi:G\to\mathbb T$, not the trace of an arbitrary group representation. A [Gelfand character](../../../../../character-of-an-algebra.md) is a nonzero multiplicative complex-linear functional on the [convolution](../../../../../convolution.md) algebra. We use the convention

$$
\boxed{\Phi_\chi(f)=\int_G f(x)\chi(x)\,dx}.
$$

With the alternative standard Fourier convention involving $\overline\chi$, one simply conjugates every [group character](../../../../../continuous-unitary-character.md) in this identification.

For such $\chi$, the functional is bounded by $\|f\|_1$, and [Fubini's theorem](../../../../../fubini-s-theorem.md), the substitution $y=xz$, and the [homomorphism](../../../../../homomorphism.md) law give

$$
\Phi_\chi(f*g)=\int\!\int f(x)g(z)\chi(xz)\,dz\,dx
=\Phi_\chi(f)\Phi_\chi(g).
$$

It is nonzero: if $u\ge0$ is nonzero in $C_c(G)$, then $f=\overline\chi u$ has $\Phi_\chi(f)=\int u>0$.

Conversely let $\Phi$ be an [algebra character](../../../../../character-of-an-algebra.md). It is automatically bounded, with $|\Phi(f)|\le\|f\|_1$. Indeed, extend it to the [unitization](../../../../../unitization-of-an-algebra.md) by $\widetilde\Phi(f+\lambda1)=\Phi(f)+\lambda$. If $|\Phi(f)|>\|f\|_1$, the [Neumann series](../../../../../neumann-series.md) makes $f-\Phi(f)1$ invertible, whereas its character value is zero, contradicting multiplicativity of an invertible element and its inverse.

Choose $g$ with $\Phi(g)\ne0$ and put $\chi(x)=\Phi(T_xg)/\Phi(g)$. Commutativity of the group gives $(T_xf)*g=f*(T_xg)$; applying $\Phi$ yields

$$
\Phi(T_xf)=\chi(x)\Phi(f)\quad\text{for every }f.
$$

Thus the ratio is independent of the chosen $g$. Applying the relation successively to $T_xT_yg=T_{xy}g$ gives $\chi(xy)=\chi(x)\chi(y)$, and $\chi(e)=1$. In particular it never vanishes.

The translation map $x\mapsto T_xg$ is continuous in $L^1$. For $g\in C_c(G)$, translated supports near a fixed $x$ lie in one [compact set](../../../../../compact-space.md); continuity on that set and a finite cover give [uniform convergence](../../../../../uniform-convergence.md) of the translated values, hence $L^1$ convergence because the [compact set](../../../../../compact-space.md) has finite [Haar measure](../../../../../haar-measure.md). For general $g$, approximate by $C_c(G)$ and use $\|T_xg\|_1=\|g\|_1$. Therefore $\chi$ is continuous. For all integers $n$,

$$
|\chi(x)|^n=\frac{|\Phi(T_{x^n}g)|}{|\Phi(g)|}
\le\frac{\|g\|_1}{|\Phi(g)|}.
$$

Positive powers exclude modulus greater than one; negative powers exclude modulus less than one. Hence $|\chi(x)|=1$.

Finally, the $L^1$-valued [convolution](../../../../../convolution.md) formula $f*g=\int f(x)T_xg\,dx$ and boundedness of $\Phi$ give

$$
\Phi(f)\Phi(g)=\Phi(f*g)=\int f(x)\Phi(T_xg)\,dx
=\Phi(g)\int f(x)\chi(x)\,dx.
$$

Cancel $\Phi(g)$ to obtain the displayed formula for every $f$. Different characters give different functionals: if their continuous difference is nonzero at a point, integration against a suitably phased compactly supported test function in a small [neighbourhood](../../../../../neighbourhood-mathematics.md) detects that difference. Thus the correspondence is bijective.

It also identifies the [character space of an Abelian L1 group algebra](../../../../../character-space-of-an-abelian-l1-group-algebra.md) topologically with the [Pontryagin dual group](../../../../../pontryagin-dual-group.md). For a net converging uniformly on [compact subsets](../../../../../compact-space.md) in $\widehat G$, convergence of the functionals follows first for compactly supported $f$, then for all $L^1$ functions using the common [norm](../../../../../norm.md) bound one. Conversely suppose the functionals converge in the [Gelfand topology](../../../../../gelfand-topology.md). Choose $g$ whose limiting character value is nonzero; its values are eventually bounded away from zero. For compact $K\subset G$, the set $\{T_xg:x\in K\}$ is compact in $L^1$. Convergence of uniformly bounded [linear functionals](../../../../../linear-functional.md) is uniform on this [compact set](../../../../../compact-space.md): a finite norm-net reduces it to convergence at finitely many functions, with the common bound controlling the approximation error. The ratio formula then gives [uniform convergence](../../../../../uniform-convergence.md) of the [group characters](../../../../../continuous-unitary-character.md) on $K$. This proves equality with the [compact-open topology](../../../../../compact-open-topology.md), without assuming first countability of $G$.

For later use, these transforms form a self-adjoint subalgebra dense in $C_0(\widehat G)$. The set of [algebra characters](../../../../../character-of-an-algebra.md) together with the zero functional is weak-star compact by [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) and the closed multiplicativity equations. Removing zero gives a locally compact Hausdorff [character space](../../../../../character-space-of-an-algebra.md); each evaluation $\Phi\mapsto\Phi(f)$ vanishes at infinity, since its modulus-at-least-$\epsilon$ set is compact and avoids zero. Transforms separate characters, and none vanishes identically at a given character. They are closed under [conjugation](../../../../../conjugation.md) because $f^*(x)=\overline{f(x^{-1})}$ satisfies $\Phi_\chi(f^*)=\overline{\Phi_\chi(f)}$. The locally compact [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) therefore gives the claimed density.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
