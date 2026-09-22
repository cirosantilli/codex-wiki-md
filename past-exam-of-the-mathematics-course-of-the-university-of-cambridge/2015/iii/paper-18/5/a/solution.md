<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [holomorphic vector bundle](../../../../../../holomorphic-vector-bundle.md) $E$, the [sheaf of vector-bundle-valued differential forms](../../../../../../sheaf-of-vector-bundle-valued-differential-forms.md) is

$$
\mathcal A^{p,q}(E)(U)=\Gamma\left(U,
\bigwedge^p(T^{1,0}X)^*\otimes\bigwedge^q(T^{0,1}X)^*\otimes E\right),
$$

where sections are smooth and restrictions are the usual ones. In a [holomorphic local frame](../../../../../../holomorphic-local-trivialization.md) of $E$, the [Dolbeault operator](../../../../../../dolbeault-operator.md) $\bar\partial_E$ acts coefficientwise and satisfies $\bar\partial_E^2=0$. Its [Dolbeault cohomology with values in a holomorphic vector bundle](../../../../../../dolbeault-cohomology-with-values-in-a-holomorphic-vector-bundle.md) is the cohomology of the global section complex $\mathcal A^{p,\bullet}(X,E)$.

The bundle-valued [Dolbeault theorem](../../../../../../dolbeault-theorem.md) identifies this with [sheaf cohomology](../../../../../../sheaf-cohomology.md):

$$
\boxed{H^q(X,\Omega_X^p\otimes\mathcal O(E))\cong H^{p,q}_{\bar\partial}(X,E).}
$$

Here $\Omega_X^p$ is the [sheaf of holomorphic differential forms](../../../../../../sheaf-of-holomorphic-differential-forms.md), and $\mathcal O(E)$ is the [sheaf of holomorphic sections of a vector bundle](../../../../../../sheaf-of-holomorphic-sections-of-a-vector-bundle.md). Equivalently, the complex

$$
0\longrightarrow\Omega_X^p\otimes\mathcal O(E)
\longrightarrow\mathcal A^{p,0}(E)\xrightarrow{\bar\partial_E}\mathcal A^{p,1}(E)
\xrightarrow{\bar\partial_E}\cdots
$$

is a [fine sheaf](../../../../../../fine-sheaf.md) resolution, by the local [Dolbeault-Poincaré lemma](../../../../../../dolbeault-poincare-lemma.md) and smooth [partitions of unity](../../../../../../partition-of-unity.md). In particular $p=0$ computes $H^q(X,\mathcal O(E))$; for $p>0$ the holomorphic differential-form factor must be retained.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
