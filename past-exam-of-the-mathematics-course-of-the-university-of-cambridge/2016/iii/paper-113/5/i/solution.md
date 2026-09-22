<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [direct image of a coherent sheaf under a closed immersion](../../../../../../direct-image-of-a-coherent-sheaf-under-a-closed-immersion.md) puts $\mathcal G=f_*\mathcal F$ in the category of coherent sheaves on $\mathbb P_k^n$. By [sheaf cohomology under a closed inclusion](../../../../../../sheaf-cohomology-under-a-closed-inclusion.md) and the supplied compatibility of twisting with direct image,

$$
H^p(X,\mathcal F(d))\cong H^p(\mathbb P_k^n,\mathcal G(d)).
$$

Here is a proof of the required [Serre vanishing](../../../../../../serre-vanishing.md) on projective space. A [coherent sheaf](../../../../../../coherent-sheaf.md) on $\mathbb P_k^n$ is the [sheaf associated with a graded module](../../../../../../sheaf-associated-with-a-graded-module.md) for a finite graded $k[t_0,\ldots,t_n]$-module. Equivalently, it has a presentation by finite sums of twisting sheaves. Use a [finite twisting resolution of a coherent sheaf on projective space](../../../../../../finite-twisting-resolution-of-a-coherent-sheaf-on-projective-space.md): resolve the graded module by a finite graded [free resolution](../../../../../../free-resolution.md), using the [Hilbert syzygy theorem](../../../../../../hilbert-s-syzygy-theorem.md), and sheafify; [exactness of localization](../../../../../../exactness-of-localization.md) preserves the resolution. Its terms are finite sums of $\mathcal O(a)$.

Choose $d$ sufficiently large that all twists $a+d$ occurring in these finitely many terms are nonnegative. The [cohomology of twisting sheaves on projective space](../../../../../../cohomology-of-twisting-sheaves-on-projective-space.md) then vanishes in every positive degree for every resolution term. In a short exact sequence $0\to\mathcal K_{j+1}\to\mathcal E_j\to\mathcal K_j\to0$, with $\mathcal K_0=\mathcal G$, the [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) identifies $H^p(\mathcal K_j(d))$ with $H^{p+1}(\mathcal K_{j+1}(d))$ for $p>0$. Iterating to the final acyclic term proves

$$
\boxed{H^p(X,\mathcal F(d))=0\quad(p>0,\ d\gg0).}
$$

The standard graded-module description used here is given in [Stacks Project, Section 30.15](https://stacks.math.columbia.edu/tag/0BXE); the vanishing follows from the displayed finite-resolution argument.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
