<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $h_{ab}=\delta g_{ab}$ and $C^a{}_{bc}=\delta\Gamma^a{}_{bc}$. The difference between two [affine connections](../../../../../../../affine-connection.md) is a tensor, so its infinitesimal change $C$ is a type $(1,2)$ [tensor field](../../../../../../../tensor-field.md). Both [affine connections](../../../../../../../affine-connection.md) are [torsion-free](../../../../../../../torsion-free-connection.md), giving $C^a{}_{bc}=C^a{}_{cb}$. Varying [metric compatibility](../../../../../../../metric-compatibility.md) gives

$$
\nabla_c h_{ab}=g_{db}C^d{}_{ca}+g_{ad}C^d{}_{cb}.
$$

Lower the first index of $C$. Add the versions with derivatives $b,c$ and subtract the one with derivative $d$; the lower-slot symmetry cancels the unwanted terms, leaving

$$
\nabla_bh_{dc}+\nabla_ch_{db}-\nabla_dh_{bc}=2g_{da}C^a{}_{bc}.
$$

Therefore

$$
\boxed{\delta\Gamma^a{}_{bc}=\frac12g^{ad}
(\nabla_ch_{db}+\nabla_bh_{dc}-\nabla_dh_{bc}).}
$$

All [covariant derivatives](../../../../../../../covariant-derivative.md) use the original [Levi-Civita connection](../../../../../../../levi-civita-connection.md). The PDF has $\nabla_bh_{dc}$ as its second term; the converted TeX's $\nabla_dh_{dc}$ is a transcription error.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 49](../../../../paper-49-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
