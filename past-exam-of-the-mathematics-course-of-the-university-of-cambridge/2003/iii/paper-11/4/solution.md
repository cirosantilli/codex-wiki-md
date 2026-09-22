<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a locally compact Hausdorff Abelian group $G$, [Bochner's theorem](../../../../../bochner-s-theorem.md) states that a continuous [positive-definite function](../../../../../positive-definite-function.md) $p$ has a unique representation

$$
\boxed{p(x)=\int_{\widehat G}\chi(x)\,d\nu(\chi),\qquad
\nu\ge0,\quad\nu(\widehat G)=p(e)},
$$

where $\nu$ is a finite [Radon measure](../../../../../radon-measure.md) on the [Pontryagin dual group](../../../../../pontryagin-dual-group.md). Conversely every such measure gives a continuous [positive-definite function](../../../../../positive-definite-function.md). Here positive definiteness means $\sum_{i,j}c_i\overline{c_j}p(x_ix_j^{-1})\ge0$ for all finite choices. The Abelian and continuity hypotheses are part of the theorem; the representation is not claimed for arbitrary non-Abelian groups or discontinuous functions.

First prove existence without presupposing the representation. The elementary consequences of positive definiteness give $p(x^{-1})=\overline{p(x)}$, $p(e)\ge0$ and $|p(x)|\le p(e)$. If $p(e)=0$, then $p=0$ and take $\nu=0$. Otherwise form finite formal linear combinations of symbols $[x]$, with sesquilinear form

$$
\langle[x],[y]\rangle=p(xy^{-1}),
$$

linear in its first variable. Positive definiteness makes this form [positive semidefinite](../../../../../positive-semidefinite-matrix.md). The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) for such a form shows that null vectors are orthogonal to everything, so quotienting by them gives an [inner product space](../../../../../inner-product-space.md). Complete it to a [Hilbert space](../../../../../hilbert-space-split.md) $H$. Since $G$ is Abelian, translation $U_a[x]=[ax]$ preserves the form and extends to a [unitary operator](../../../../../unitary-operator.md). Its inverse is $U_{a^{-1}}$, so $(U_a)$ is a [unitary representation](../../../../../unitary-representation.md). With $v=[e]$,

$$
p(x)=\langle U_xv,v\rangle,\qquad\|v\|^2=p(e).
$$

The translated copies of $v$ span a dense subspace. Moreover

$$
\|U_a[y]-[y]\|^2=2[p(e)-\operatorname{Re}p(a)]\longrightarrow0\quad(a\to e).
$$

Finite sums and density, together with $\|U_a\|=1$, give [strong continuity](../../../../../strong-continuity.md) on all of $H$. This constructs the [cyclic unitary representation of a positive-definite function](../../../../../cyclic-unitary-representation-of-a-positive-definite-function.md) directly.

For $f\in L^1(G)$ define the [integrated unitary representation](../../../../../integrated-unitary-representation.md) $\pi(f)=\int f(x)U_x\,dx$, with the integral applied to each vector. Its [norm](../../../../../norm.md) is at most $\|f\|_1$. Fubini gives $\pi(f*g)=\pi(f)\pi(g)$, and inversion in the Abelian group gives $\pi(f^*)=\pi(f)^*$. Thus

$$
\mathcal A=\overline{\pi(L^1(G))}^{\|\cdot\|}
$$

is a commutative [C-star algebra](../../../../../c-star-algebra.md). It is nondegenerate: choose nonnegative compactly supported functions $u_V$ of Haar integral one with supports shrinking to the [identity element](../../../../../identity-element.md). [Strong continuity](../../../../../strong-continuity.md) implies

$$
\|\pi(u_V)w-w\|\le\sup_{x\in V}\|U_xw-w\|\longrightarrow0
$$

for every $w\in H$. These form an [approximate identity](../../../../../approximate-identity.md) in the representation. [Neighbourhoods](../../../../../neighbourhood-mathematics.md) may form a net, since no metrizability is being assumed here.

The [Commutative Gelfand--Naimark theorem](../../../../../commutative-gelfand-naimark-theorem.md) identifies $\mathcal A$ with $C_0(X)$, where $X$ is its [character space](../../../../../character-space-of-an-algebra.md). The positive vector functional $\omega(B)=\langle Bv,v\rangle$ becomes a bounded positive functional on $C_0(X)$, so the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) supplies a finite positive [Radon measure](../../../../../radon-measure.md) $\rho$ with

$$
\omega(B)=\int_X\theta(B)\,d\rho(\theta).
$$

These general representation theorems are applied to the explicitly constructed algebra; they are not an assumption of Bochner's conclusion.

For each $\theta\in X$, the functional $f\mapsto\theta(\pi(f))$ is a nonzero [algebra character](../../../../../character-of-an-algebra.md) of $L^1(G)$, since $\pi(L^1(G))$ is dense in $\mathcal A$. By Question 3 it has the form $\int f(x)\chi_\theta(x)\,dx$. The resulting map $\iota:X\to\widehat G$ is continuous: pointwise convergence of $\theta$ on $\mathcal A$ gives convergence on all $\pi(f)$, and the topological character identification in Question 3 gives compact-open convergence of $\chi_\theta$. Push $\rho$ forward under $\iota$ to obtain $\nu$. This [finite measure](../../../../../finite-measure.md) is Radon: [compact subsets](../../../../../compact-space.md) approximating the measure of any inverse-image [Borel set](../../../../../borel-set.md) have compact images, giving inner regularity; finiteness and complements then give outer regularity.

To recover $p(x)$, note that $U_x\pi(u_V)=\pi(T_xu_V)\in\mathcal A$. Hence

$$
\langle U_x\pi(u_V)v,v\rangle
=\int_X\chi_\theta(x)\Phi_{\chi_\theta}(u_V)\,d\rho(\theta).
$$

The left side tends to $p(x)$. On the right, $|\Phi_\chi(u_V)|\le1$ and $\Phi_\chi(u_V)\to1$ uniformly on [compact subsets](../../../../../compact-space.md) of $\widehat G$. For completeness, the evaluation $(\chi,x)\mapsto\chi(x)$ is jointly continuous: near $x_0$ restrict $x$ to a compact [neighbourhood](../../../../../neighbourhood-mathematics.md), control the character uniformly there, and use continuity of the fixed character. A finite cover of a [compact set](../../../../../compact-space.md) of characters then makes those characters equicontinuous at $e$, proving the stated [uniform convergence](../../../../../uniform-convergence.md). Continuity of $\iota$ gives [uniform convergence](../../../../../uniform-convergence.md) on [compact subsets](../../../../../compact-space.md) of $X$, and the finite [Radon measure](../../../../../radon-measure.md) $\rho$ makes the remaining tails arbitrarily small. Thus passage to the limit is valid even for a net, and

$$
p(x)=\int_X\chi_\theta(x)\,d\rho(\theta)=\int_{\widehat G}\chi(x)\,d\nu(\chi).
$$

Taking $x=e$ also gives the required total mass $p(e)$.

Conversely, a finite positive [Radon measure](../../../../../radon-measure.md) gives

$$
\sum_{i,j}c_i\overline{c_j}p(x_ix_j^{-1})
=\int_{\widehat G}\left|\sum_i c_i\chi(x_i)\right|^2d\nu(\chi)\ge0.
$$

Its transform is continuous. Indeed, choose a [compact set](../../../../../compact-space.md) of characters with arbitrarily small measure outside it; joint continuity of evaluation gives uniform continuity in $x$ near the specified point on that [compact set](../../../../../compact-space.md), while the outside contribution is bounded by twice its measure. This proves continuity without using an unjustified dominated-convergence assertion for arbitrary nets.

Finally suppose two finite [Radon measures](../../../../../radon-measure.md) have the same transform. Multiply by $f\in L^1(G)$ and integrate over $G$. Fubini shows that the measures agree on every function $\chi\mapsto\Phi_\chi(f)$. Question 3 showed that these functions are uniformly dense in $C_0(\widehat G)$. Boundedness of both measure functionals extends equality to all of $C_0(\widehat G)$; uniqueness in the Riesz representation theorem gives equality of the measures. This proves existence, uniqueness and the converse, completing Bochner's theorem. In particular **$p(e)=1$ corresponds exactly to a [probability measure](../../../../../probability-measure.md)** on the dual group.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
