<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The integral [Poincare duality](../../../../../poincare-duality.md) theorem says that a closed connected oriented $n$-manifold has a [fundamental class](../../../../../fundamental-class.md) $[M]\in H_n(M;\mathbb Z)$ for which cap product gives $H^q(M;\mathbb Z)\cong H_{n-q}(M;\mathbb Z)$. The general [Poincare duality with the orientation local system](../../../../../poincare-duality-with-the-orientation-local-system.md) uses $[M]\in H_n(M;\mathcal O_M)$ and gives

$$
H^q(M;\mathcal A)\xrightarrow{\ \frown[M]\ }H_{n-q}(M;\mathcal O_M\otimes\mathcal A)
$$

for a [local coefficient system](../../../../../local-coefficient-system.md) $\mathcal A$. Over $\mathbb F_2$ it holds without orientability. For constant integral coefficients on a nonorientable connected closed manifold, $H_n=H^0(M;\mathcal O_M)=0$, while $H^n=H_0(M;\mathcal O_M)=\mathbb Z/2$: the invariants of sign reversal in $\mathbb Z$ are zero and its coinvariants are $\mathbb Z/(a\sim-a)$.

If the three-manifold is orientable, duality and the [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) give

$$
H_2(M;\mathbb Z)\cong H^1(M;\mathbb Z)\cong\operatorname{Hom}(H_1(M;\mathbb Z),\mathbb Z)\cong\boxed{\mathbb Z^b}.
$$

For a nonorientable three-manifold, $H_3=0$ and $H^3=\mathbb Z/2$. The top-degree universal coefficient sequence therefore gives

$$
\operatorname{Ext}^1_{\mathbb Z}(H_2(M;\mathbb Z),\mathbb Z)\cong\mathbb Z/2.
$$

Since the homology groups are finitely generated, their cyclic decomposition shows that this Ext group is isomorphic to the torsion subgroup of $H_2$. Thus the torsion is exactly $\mathbb Z/2$, not the possibly larger torsion subgroup of $H_1$. Also [odd-dimensional closed manifolds have zero Euler characteristic](../../../../../odd-dimensional-closed-manifolds-have-zero-euler-characteristic.md), by pairing complementary mod-two Betti numbers. If $r$ is the free rank of $H_2$, it follows that $0=\chi(M)=1-b+r$, giving the [second homology of a closed nonorientable three-manifold](../../../../../second-homology-of-a-closed-nonorientable-three-manifold.md)

$$
\boxed{H_2(M;\mathbb Z)\cong\mathbb Z^{b-1}\oplus\mathbb Z/2,\qquad b\geq1.}
$$

The inequality is forced by the nonnegative free rank $b-1$.

For the final graded-group construction, one always has $K^0=K^3=K^6=\mathbb Z$, since each of these is copied from $H^0$ of a connected three-manifold. Suppose it were the cohomology of a closed six-manifold $N$. The group $K^0$ makes $N$ connected, and $K^6=\mathbb Z$ makes it orientable: the nonorientable alternative has top integral cohomology $\mathbb Z/2$, as above. Its third rational cohomology would then be one-dimensional. But the middle [Poincare duality pairing](../../../../../poincare-duality-pairing.md) on $H^3(N;\mathbb Q)$ is nondegenerate and skew-symmetric by graded commutativity, hence must have even dimension. Equivalently, a generator $u$ would satisfy $u\smile u=-u\smile u$, so its square in the torsion-free top group is zero and the entire rank-one pairing vanishes. This contradicts duality and the [even rank of middle cohomology in dimension four k plus two](../../../../../even-rank-of-middle-cohomology-in-dimension-four-k-plus-two.md). Therefore

$$
\boxed{K\text{ is never the integral cohomology of a closed six-manifold}.}
$$

Both existence questions have negative answers, independently of the other groups of the original three-manifold.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
