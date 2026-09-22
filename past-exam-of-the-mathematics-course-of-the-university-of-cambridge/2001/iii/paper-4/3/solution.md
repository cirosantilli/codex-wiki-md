<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The identification with $\mathbf P^1$ means that $C$ is a [smooth plane conic](../../../../../smooth-plane-conic.md). An arbitrary singular or nonreduced conic over an [algebraically closed field](../../../../../algebraically-closed-field.md) cannot be identified with the projective line, so this is a necessary qualification implicit in the requested description.

Choose an equation $\ell=0$ for $L\subset\mathbf P^3$ and a degree-two equation $q=0$ whose restriction to $L$ defines $C$. Its [homogeneous ideal](../../../../../homogeneous-ideal.md) in $\mathbf P^3$ is $(\ell,q)$. These equations form a [regular sequence](../../../../../regular-sequence.md): $\ell$ is a non-zero-divisor in the polynomial ring, and modulo $\ell$ the ring is a polynomial ring in three variables, in which the nonzero quadratic $q$ is again a non-zero-divisor. The generator classes therefore form a basis of the [conormal sheaf](../../../../../conormal-sheaf.md), with their grading shifts:

$$
\mathcal I_C/\mathcal I_C^2\cong\mathcal O_C(-1)\oplus\mathcal O_C(-2).
$$

One can verify the absence of relations from the two-generator [Koszul complex](../../../../../koszul-complex.md): a relation between $\ell,q$ is a multiple of $(q,-\ell)$, whose coefficients become zero modulo $\mathcal I_C$. This is the [normal sheaf of a projective complete intersection](../../../../../normal-sheaf-of-a-projective-complete-intersection.md) calculation. Dualizing the conormal sheaf gives

$$
N_{C/\mathbf P^3}\cong\mathcal O_C(1)\oplus\mathcal O_C(2).
$$

These twists are restrictions from $\mathbf P^3$, not intrinsic degree-one twists on $\mathbf P^1$. A line in the plane cuts the degree-two curve in two points counted with multiplicity, so the [degree of a line bundle](../../../../../degree-of-a-line-bundle.md) $\mathcal O_C(1)$ is two. The [Picard group of the projective line](../../../../../picard-group-of-the-projective-line.md) then gives

$$
\mathcal O_C(1)\cong\mathcal O_{\mathbf P^1}(2),\qquad\mathcal O_C(2)\cong\mathcal O_{\mathbf P^1}(4).
$$

Equivalently, the degree-two [Veronese embedding](../../../../../veronese-embedding.md) $[s:t]\mapsto[s^2:st:t^2]$ pulls each linear coordinate back to a quadratic. Thus the [normal bundle of a smooth plane conic](../../../../../normal-bundle-of-a-smooth-plane-conic.md) is

$$
\boxed{N_{C/\mathbf P^3}\cong\mathcal O_{\mathbf P^1}(4)\oplus\mathcal O_{\mathbf P^1}(2),\qquad\{a,b\}=\{4,2\}.}
$$

The same splitting follows from the normal sequence for the two embeddings:

$$
0\longrightarrow N_{C/L}\longrightarrow N_{C/\mathbf P^3}\longrightarrow N_{L/\mathbf P^3}|_C\longrightarrow0.
$$

Its outer terms are $\mathcal O_{\mathbf P^1}(4)$ and $\mathcal O_{\mathbf P^1}(2)$. The [extension group](../../../../../extension-group.md) class lies in $\operatorname{Ext}^1(\mathcal O(2),\mathcal O(4))=H^1(\mathbf P^1,\mathcal O(2))=0$, by the preceding [Čech cohomology](../../../../../cech-cohomology.md) calculation, so the sequence splits. Both methods distinguish the ambient twist from the intrinsic degree on the curve.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
