<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [Riemann surface](../../../../../riemann-surfaces.md) is a connected one-complex-dimensional [complex manifold](../../../../../complex-manifold.md): it has local complex coordinates with holomorphic transition maps. These coordinates induce an orientation and a [conformal structure](../../../../../conformal-structure.md). Fix a closed oriented topological surface $S_g$ of [genus](../../../../../genus-of-a-surface.md) $g$. A point of [Teichmüller space](../../../../../teichmuller-space.md) is a marked [Riemann surface](../../../../../riemann-surfaces.md) $(X,f)$, where $f:S_g\to X$ is an orientation-preserving marking. Two pairs are equivalent if there is a [biholomorphism](../../../../../biholomorphism.md) $h:X\to X'$ with $h\circ f$ isotopic to $f'$. Thus the marking remembers how curves on the reference surface sit in $X$; forgetting it gives the [moduli space of Riemann surfaces](../../../../../moduli-space-of-riemann-surfaces.md), obtained by quotienting by the [mapping class group](../../../../../mapping-class-group.md).

For $g\geq2$, the [uniformization theorem](../../../../../uniformization-theorem.md) supplies a unique curvature-$-1$ [hyperbolic metric](../../../../../hyperbolic-metric.md) in each conformal class. A [pants decomposition](../../../../../pants-decomposition.md) has $3g-3$ cuffs, and their positive lengths together with their real twists give [Fenchel–Nielsen coordinates](../../../../../fenchel-nielsen-coordinates.md). Hence

$$
\boxed{\mathcal T_g\cong\mathbb R^{6g-6},\qquad\dim_{\mathbb C}\mathcal T_g=3g-3\quad(g\geq2).}
$$

For completeness, $\mathcal T_0$ is a point, whereas $\mathcal T_1$ is the upper half-plane, parametrizing marked complex tori $\mathbb C/(\mathbb Z+\tau\mathbb Z)$ with $\operatorname{Im}\tau>0$.

The [Wolpert generic spectral rigidity theorem](../../../../../wolpert-generic-spectral-rigidity-theorem.md) says that, for fixed $g\geq2$, there is a closed proper real-analytic exceptional subset of $\mathcal T_g$ such that a [hyperbolic surface](../../../../../hyperbolic-surface.md) outside that subset is determined up to [isometry](../../../../../isometry.md) by its unmarked [length spectrum](../../../../../length-spectrum.md), equivalently its [Laplacian](../../../../../laplacian.md) [spectrum](../../../../../spectrum-functional-analysis.md). This is an unoriented [isometry](../../../../../isometry.md) statement: reversing orientation cannot be detected by either [spectrum](../../../../../spectrum-functional-analysis.md).

The [Huber spectral equivalence theorem](../../../../../huber-spectral-equivalence-theorem.md) says that two closed curvature-$-1$ [hyperbolic surfaces](../../../../../hyperbolic-surface.md) have the same [Laplacian](../../../../../laplacian.md) [spectrum](../../../../../spectrum-functional-analysis.md), with multiplicities, if and only if they have the same unmarked [length spectrum](../../../../../length-spectrum.md), with multiplicities. One may consistently count unoriented closed [geodesics](../../../../../geodesic.md) including their iterates; alternatively, the primitive multiset determines the multiset with iterates and conversely. This equivalence comes from the [Selberg trace formula](../../../../../selberg-trace-formula.md).

The [Buser finite length spectrum theorem](../../../../../buser-finite-length-spectrum-theorem.md) is the finite-determination ingredient: for each $g\geq2$ and $\varepsilon>0$ there is a finite number $L(g,\varepsilon)$ such that, for any two closed [hyperbolic surfaces](../../../../../hyperbolic-surface.md) of [genus](../../../../../genus-of-a-surface.md) $g$ with [hyperbolic systole](../../../../../hyperbolic-systole.md) at least $\varepsilon$, equality of their length multisets through $L(g,\varepsilon)$ implies equality of their entire [length spectra](../../../../../length-spectrum.md). The finite-length statement is used in [Buser's chapter on Wolpert's theorem](https://link.springer.com/chapter/10.1007/978-0-8176-4992-0_10). It determines the full [spectrum](../../../../../spectrum-functional-analysis.md), not necessarily the [isometry](../../../../../isometry.md) class.

Here is a proof of the [Buser finite length spectrum theorem](../../../../../buser-finite-length-spectrum-theorem.md) through [finite spectral matching by polynomial invariants](../../../../../finite-spectral-matching-by-polynomial-invariants.md). We use the following subsidiary results, stating the required content. First, [Mumford's compactness theorem](../../../../../mumford-s-compactness-theorem.md) makes the part of the genus-$g$ [moduli space of Riemann surfaces](../../../../../moduli-space-of-riemann-surfaces.md) with [hyperbolic systole](../../../../../hyperbolic-systole.md) at least $\varepsilon$ compact. Second, marked [hyperbolic holonomy representations](../../../../../hyperbolic-holonomy-representation.md) of a closed oriented surface lift from $\operatorname{PSL}_2(\mathbb R)$ to $\operatorname{SL}_2(\mathbb R)$, and normalized representatives can be chosen continuously on sufficiently small parameter charts. Their [hyperbolic translation length](../../../../../hyperbolic-translation-length.md) satisfies

$$
q_\gamma(\rho):=\operatorname{tr}(\rho(\gamma))^2=4\cosh^2\bigl(\ell_\gamma(\rho)/2\bigr).
$$

Third, the [length spectrum](../../../../../length-spectrum.md) of a compact [hyperbolic surface](../../../../../hyperbolic-surface.md) is locally finite, and metrics on compact marked parameter charts are uniformly [bilipschitz equivalent](../../../../../bilipschitz-equivalence.md). Finally, the [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md) implies that a descending sequence of [algebraic sets](../../../../../algebraic-set.md) in a finite-dimensional affine space stabilizes. These are compactness, holonomy, elementary geometric finiteness and algebraic finiteness results; none is the finite unmarked-spectrum assertion we are proving.

By compactness, finitely many relatively compact marked charts cover the thick [moduli space of Riemann surfaces](../../../../../moduli-space-of-riemann-surfaces.md). Choose normalized lifted [hyperbolic holonomy representations](../../../../../hyperbolic-holonomy-representation.md) on these charts and take their compact closures. Their finite union $K$ is a compact set of determinant-one matrix tuples representing every surface in the thick part, possibly more than once. Each tuple records the images of the $2g$ generators of the [fundamental group](../../../../../fundamental-group.md). Thus $K$ sits in a fixed finite-dimensional real matrix space. Every group word is a polynomial in these matrix entries: multiplication is polynomial, and for a determinant-one two-by-two matrix its inverse is its adjugate, also polynomial. Consequently each $q_\gamma$ is a [polynomial](../../../../../polynomial-split.md) on the ambient space. Squared traces remove the sign ambiguity of the lift, and $4\cosh^2(\ell/2)$ is strictly increasing for positive $\ell$.

Enumerate the unoriented nontrivial [free homotopy](../../../../../free-homotopy.md) classes as $\gamma_1,\gamma_2,\ldots$, including the iterates, and write $\ell_j(x)$ for their [geodesic](../../../../../geodesic.md) lengths at $x\in K$. The [uniform finiteness of short geodesic classes](../../../../../uniform-finiteness-of-short-geodesic-classes.md) follows here directly: on each of the finitely many compact marked charts, choose a fixed reference metric $h$ and a uniform bilipschitz constant $C$. A class with $\ell_j(x)\leq R$ somewhere on that chart has reference length at most $CR$. Only finitely many classes have that reference length, and a finite union of these finite collections is finite. In particular, for every $j$ the candidate set

$$
F_j=\left\{k:\min_{x\in K}\ell_k(x)\leq\max_{x\in K}\ell_j(x)\right\}
$$

is finite. If two parameters in $K$ have equal lengths for classes $j,k$, then $k\in F_j$. These candidate sets depend on the fixed compact set $K$ and the source label $j$, not on the number of labels currently being matched.

For every $N$, define $E_N$ in the full ambient space of pairs of matrix tuples $(x,y)$ as follows. Require an injective choice $\sigma:\{1,\ldots,N\}\to\mathbb N$ with $\sigma(j)\in F_j$ and

$$
q_j(x)=q_{\sigma(j)}(y)\quad(1\leq j\leq N),
$$

and independently require an injective choice $\tau:\{1,\ldots,N\}\to\mathbb N$ with $\tau(j)\in F_j$ and

$$
q_j(y)=q_{\tau(j)}(x)\quad(1\leq j\leq N).
$$

There are finitely many possible pairs of choices $(\sigma,\tau)$ because every $F_j$ is finite. For each choice these are finitely many polynomial equations. Therefore $E_N$ is a finite union of [algebraic sets](../../../../../algebraic-set.md), hence an [algebraic set](../../../../../algebraic-set.md). Restricting an injective matching to its first $N$ entries proves

$$
E_1\supseteq E_2\supseteq E_3\supseteq\cdots.
$$

The [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md) now supplies $N_0$ such that $E_N=E_{N_0}$ for all $N\geq N_0$. This step takes place in a fixed affine space and uses polynomial equations, so it gives stabilization of the actual sets, not just stabilization of germs at individual parameters.

For $(x,y)\in E_{N_0}\cap(K\times K)$, stabilization gives injective partial length matchings in both directions for every $N$. Fix any length $a>0$. Only finitely many labels have length $a$ at $x$ or at $y$, by local finiteness. Take $N$ large enough to contain every such label at $x$. Its injective matching into the labels at $y$ preserves $q_j$, and hence preserves length, so the multiplicity of $a$ at $x$ is at most its multiplicity at $y$. The reverse matching gives the opposite inequality. Thus the two multiplicities are equal for every $a$, proving equality of the entire unmarked [length spectra](../../../../../length-spectrum.md). No assumed global matching or unjustified exchange of infinitely many neighborhoods is needed.

Finally choose a number

$$
L>\max_{1\leq j\leq N_0}\max_{x\in K}\ell_j(x).
$$

Suppose the two length multisets agree through $L$. For each of the first $N_0$ labels at $x$, select a distinct equal-length label at $y$, which is possible precisely because the truncated multisets agree with multiplicity. Each selected label belongs to the corresponding $F_j$. Do the same in the reverse direction. Then $(x,y)\in E_{N_0}$, and the previous paragraph proves equality of the full [length spectra](../../../../../length-spectrum.md). Since $K$ was selected using only the fixed thick genus-$g$ parameter space, the resulting finite $L$ depends only on $g,\varepsilon$. This proves

$$
\boxed{\mathcal L(X)\cap(0,L]=\mathcal L(Y)\cap(0,L]\ \Longrightarrow\ \mathcal L(X)=\mathcal L(Y),}
$$

with each intersection interpreted as a multiset. By the [Huber spectral equivalence theorem](../../../../../huber-spectral-equivalence-theorem.md), the corresponding entire [Laplacian](../../../../../laplacian.md) [spectra](../../../../../spectrum-functional-analysis.md) also agree. This is the finite matching reduction needed before the analytic and geometric rigidity steps in the [Wolpert generic spectral rigidity theorem](../../../../../wolpert-generic-spectral-rigidity-theorem.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
