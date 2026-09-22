<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $m=\dim M$. Choose a homogeneous basis $e_{q,i}$ of $H^q(M;\mathbb Q)$ and its [Poincare dual](../../../../../poincare-dual.md) basis $e_{q,i}^*\in H^{m-q}(M;\mathbb Q)$, normalized by

$$
\langle e_{q,i}\smile e_{q,j}^*,[M]\rangle=\delta_{ij}.
$$

With the product orientation, the [cohomology class of the diagonal](../../../../../cohomology-class-of-the-diagonal.md) is

$$
\boxed{\varepsilon_\Delta=\sum_{q,i}(-1)^{mq}e_{q,i}^*\times e_{q,i}.}
$$

Indeed, multiplying this class by $\alpha\times\gamma$ and evaluating on $[M\times M]$ gives $\langle\alpha\smile\gamma,[M]\rangle$, which characterizes the [Poincare dual](../../../../../poincare-dual.md) of $\Delta$.

Pulling back along the graph map $(1,f):M\to M\times M$ and evaluating gives the [graph-diagonal formula for the Lefschetz number](../../../../../graph-diagonal-formula-for-the-lefschetz-number.md):

$$
\left\langle(1,f)^*\varepsilon_\Delta,[M]\right\rangle
=\sum_q(-1)^q\operatorname{tr}(f^*|H^q(M;\mathbb Q))
=L(f).
$$

If $f$ has no fixed point, its graph is disjoint from $\Delta$. Represent $\varepsilon_\Delta$ with support in a tubular neighbourhood disjoint from the graph; its pullback is zero, so $L(f)=0$. Contrapositively, **$L(f)\ne0$ implies that $f$ has a fixed point**, the [Lefschetz fixed-point theorem](../../../../../lefschetz-fixed-point-theorem.md).

Now let $M$ be three disjoint circles. A homeomorphism permutes their three components. Its action on $H^1(M;\mathbb Z)\cong\mathbb Z^3$ is a signed permutation matrix. A component fixed setwise contributes to the trace by the degree of the corresponding circle homeomorphism. An orientation-reversing circle homeomorphism has a fixed point, so fixed-point-freeness forces that degree to be $+1$. Nonfixed components contribute zero. The trace is therefore the number of fixed points of a permutation of three objects, and

$$
\boxed{\operatorname{tr}(f^*|H^1(M;\mathbb Z))\in\{0,1,3\}.}
$$

For a compact manifold $N$ with boundary, let $D(N)=N_+\cup_{\partial N}N_-$ be its double and define $F$ by applying $f$ on both copies. The [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) for this decomposition is natural under $F$. Alternating traces in a finite-dimensional exact sequence sum to zero, so the two copies of $N$ contribute twice and their intersection contributes with the opposite sign:

$$
\boxed{L(F)=2L(f)-L(f|_{\partial N}).}
$$

This is the [Lefschetz number of a doubled map](../../../../../lefschetz-number-of-a-doubled-map.md).

Finally let $N$ be a [pair of pants](../../../../../pair-of-pants-mathematics.md). If $f$ is fixed-point-free, so are its double $F$ and its boundary restriction. The [Lefschetz fixed-point theorem](../../../../../lefschetz-fixed-point-theorem.md) and the displayed identity give $L(F)=L(f|_{\partial N})=0$, hence $L(f)=0$. Since $N$ is connected and $H^i(N;\mathbb Q)$ is nonzero only for $i=0,1$,

$$
\operatorname{tr}(f^*|H^1(N;\mathbb Q))=1.
$$

Suppose the boundary permutation $\sigma$ had a fixed component. The restriction there is a fixed-point-free circle homeomorphism and thus has degree $+1$, forcing $f$ to preserve the surface orientation. The [homology action of a pair-of-pants homeomorphism](../../../../../homology-action-of-a-pair-of-pants-homeomorphism.md) would then have trace $\#\operatorname{Fix}(\sigma)-1$, which is $2$ for the identity permutation and $0$ for a transposition. Neither is $1$. Therefore $\sigma$ has no fixed component; a permutation of three objects with no fixed point is a three-cycle. Thus

$$
\boxed{f\text{ cyclically permutes the three boundary components}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
