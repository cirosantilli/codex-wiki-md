<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Cover the [projective line](../../../../../projective-line.md) by $U_0=\operatorname{Spec}k[t]$ and $U_1=\operatorname{Spec}k[t^{-1}]$. On their overlap the coordinate is invertible. Choose frames $e_0,e_1$ of the [twisting sheaf on projective space](../../../../../twisting-sheaf-on-projective-space.md) $\mathcal O(n)$ with $e_1=t^ne_0$. The [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md) applies to both charts and their intersection, so the [Čech cochain complex](../../../../../cech-cochain-complex.md)

$$
0\longrightarrow k[t]\oplus k[t^{-1}]\xrightarrow{\delta}k[t,t^{-1}]\longrightarrow0,\qquad\delta(a,b)=t^nb-a,
$$

computes the [sheaf cohomology](../../../../../sheaf-cohomology.md). Its kernel identifies with $k[t]\cap t^nk[t^{-1}]$, and its cokernel is

$$
\frac{k[t,t^{-1}]}{k[t]+t^nk[t^{-1}]}.
$$

For $n\geq0$, the intersection has basis $1,t,\ldots,t^n$; for $n<0$ it is zero. In the quotient, powers $t^j$ with $j\geq0$ or $j\leq n$ disappear. The surviving basis for $n\leq-2$ is $t^{n+1},\ldots,t^{-1}$; for $n\geq-1$ none survives. Hence

$$
\boxed{h^0(\mathcal O(n))=\max(n+1,0),\qquad h^1(\mathcal O(n))=\max(-n-1,0),\qquad H^i(\mathcal O(n))=0\ (i\geq2).}
$$

This is the [Čech cohomology of twists on the projective line](../../../../../cech-cohomology-of-twists-on-the-projective-line.md).

By the preceding question, $\omega=\Omega^1_{\mathbb P^1/k}=\mathcal O(-2)$. In the $dt$ frame its degree-one [Čech cohomology](../../../../../cech-cohomology.md) is one-dimensional, represented by $t^{-1}dt$. Define

$$
\operatorname{tr}:H^1(\omega)\longrightarrow k,\qquad [h(t)dt]\longmapsto[t^{-1}]h(t).
$$

This is well defined: differentials regular on $U_0$ have nonnegative powers, and those regular on $U_1$ have powers at most $-2$ when expressed using $dt$. Evaluation and the [cup product](../../../../../cup-product.md) give natural pairings

$$
H^i(E)\times H^{1-i}(E^\vee\otimes\omega)\longrightarrow H^1(\omega)\xrightarrow{\operatorname{tr}}k,\qquad i=0,1.
$$

For $E=\mathcal O(n)$ with $n\geq0$, the basis element $t^a$ in $H^0(E)$ pairs with $t^{-a-1}dt$ in $H^1(E^\vee\otimes\omega)$ and with no other element of this dual Laurent basis. The pairing matrix is a permutation matrix, hence invertible. For $n\leq-2$ the same computation exchanges degrees zero and one. For $n=-1$ both sides vanish. Thus the pairings are perfect for every [line bundle](../../../../../line-bundle.md) on $\mathbb P^1$.

Here we used the classification of [line bundles](../../../../../line-bundle.md) on the [projective line](../../../../../projective-line.md): they are $\mathcal O(a)$ for integers $a$. One direct justification is that every [line bundle](../../../../../line-bundle.md) has a nonzero rational section and hence is associated with a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md). The finite closed point defined by an irreducible polynomial $p(t)$ is linearly equivalent to $(\deg p)\infty$, using the [principal divisor](../../../../../principal-divisor-on-an-algebraic-curve.md) of $p(t)$. Thus every divisor is equivalent to its degree times $\infty$, proving the classification over arbitrary $k$.

To extend the pairing to every [locally free coherent sheaf](../../../../../locally-free-sheaf.md) $E$, induct on rank, without assuming the splitting theorem of the next question. A one-dimensional subspace of the generic fibre, saturated in $E$, gives an exact sequence

$$
0\longrightarrow L\longrightarrow E\longrightarrow Q\longrightarrow0
$$

with $L$ a [line bundle](../../../../../line-bundle.md) and $Q$ a lower-rank [vector bundle](../../../../../vector-bundle.md). This [saturated line subbundle on a smooth curve](../../../../../saturated-line-subbundle-on-a-smooth-curve.md) exists because its stalk and its torsion-free quotient are free over the [discrete valuation rings](../../../../../discrete-valuation-ring.md) of the curve. The dual sequence, tensored with $\omega$, is exact as well, since the original sequence splits locally.

The two [long exact sequences in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md), after dualizing one, are compatible with the evaluation pairings. In [Čech cohomology](../../../../../cech-cohomology.md), this compatibility follows by lifting a section locally: the differences of its lifts represent its connecting class, and contracting those differences with a dual cocycle gives the transpose connecting map, with the usual sign. Thus the connecting maps are adjoint; changing one vertical map's sign gives a commuting diagram. Its rows are

$$
\begin{aligned}
0&\to H^0(L)\to H^0(E)\to H^0(Q)\to H^1(L)\to H^1(E)\to H^1(Q)\to0,\\
0&\to H^1(L^\vee\omega)^*\to H^1(E^\vee\omega)^*\to H^1(Q^\vee\omega)^*\to H^0(L^\vee\omega)^*\to H^0(E^\vee\omega)^*\to H^0(Q^\vee\omega)^*\to0.
\end{aligned}
$$

The maps for $L$ and $Q$ are isomorphisms by the line-bundle calculation and induction. Exactness then makes the maps for $E$ isomorphisms, by the [Five lemma](../../../../../five-lemma.md) (or by comparing the relevant kernels and cokernels). All groups are finite-dimensional because the curve is projective and the sheaves coherent. Therefore [residue duality on the projective line](../../../../../residue-duality-on-the-projective-line.md) proves

$$
\boxed{H^i(\mathbb P^1,E)\cong H^{1-i}(\mathbb P^1,E^\vee(-2))^*,\qquad i=0,1.}
$$

These isomorphisms are natural in $E$. Higher [sheaf cohomology](../../../../../sheaf-cohomology.md) vanishes by the same two-chart complex.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
