<h1 id="3/f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\mathcal F$ be any [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) on $X$, and choose $m$ from (i). Filter it by the powers of the [nilradical sheaf](../../../../../nilradical-sheaf.md):

$$
\mathcal F\supseteq\mathcal N\mathcal F\supseteq\cdots\supseteq\mathcal N^m\mathcal F=0.
$$

Each subquotient

$$
\mathcal Q_j=\mathcal N^j\mathcal F/\mathcal N^{j+1}\mathcal F,\qquad 0\leq j<m,
$$

is a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) annihilated by $\mathcal N$. Apply (ii) to the [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) $\mathcal N^j\mathcal F$. Since $X_{\mathrm{red}}$ is an [affine scheme](../../../../../affine-scheme.md), [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md) gives

$$
H^1(X,\mathcal Q_j)\cong H^1(X_{\mathrm{red}},\mathcal Q_j)=0.
$$

The [short exact sequences](../../../../../short-exact-sequence.md)

$$
0\longrightarrow\mathcal N^{j+1}\mathcal F\longrightarrow\mathcal N^j\mathcal F\longrightarrow\mathcal Q_j\longrightarrow0
$$

yield the segments of the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md)

$$
H^1(X,\mathcal N^{j+1}\mathcal F)\longrightarrow H^1(X,\mathcal N^j\mathcal F)\longrightarrow H^1(X,\mathcal Q_j)=0.
$$

Starting from $\mathcal N^m\mathcal F=0$, descending [mathematical induction](../../../../../mathematical-induction.md) makes every middle group zero, finally giving $H^1(X,\mathcal F)=0$.

This holds for every [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) $\mathcal F$. Since a [Noetherian scheme](../../../../../noetherian-scheme.md) is a [quasi-compact scheme](../../../../../quasi-compact-scheme.md), the [Serre criterion for affineness](../../../../../cohomological-criterion-for-affineness.md) in (a) applies and proves

$$
\boxed{X_{\mathrm{red}}\text{ affine}\Longrightarrow X\text{ affine}.}
$$

This is an instance of the general fact that [affineness is invariant under nilpotent thickening](../../../../../affineness-is-invariant-under-nilpotent-thickening.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [F](../../f.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the introduction to schemes course of the University of Oxford](../../../../split.md)
6. [Introduction to schemes course of the University of Oxford](../../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
