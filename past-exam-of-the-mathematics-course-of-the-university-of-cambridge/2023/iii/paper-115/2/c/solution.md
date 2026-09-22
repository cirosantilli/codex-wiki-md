<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We induct on $n$. The claim is immediate for $\mathbb{CP}^0$. In the stated cover, $U=U_0\cong\mathbb C^n$ is contractible. The homotopy

$$
[z_0:z_1:\cdots:z_n]\longmapsto[t z_0:z_1:\cdots:z_n]
$$

deformation retracts $V$ onto the hyperplane $z_0=0$, which is $\mathbb{CP}^{n-1}$. Moreover,

$$
U\cap V\cong\mathbb C^n\setminus\{0\}
$$

deformation retracts onto $S^{2n-1}$.

The [Mayer--Vietoris sequence](../../../../../../mayer-vietoris-sequence.md) for the de Rham complex contains

$$
H^{i-1}_{\mathrm{dR}}(U\cap V)
\longrightarrow H^i_{\mathrm{dR}}(\mathbb{CP}^n)
\longrightarrow H^i_{\mathrm{dR}}(U)\oplus H^i_{\mathrm{dR}}(V).
$$

For odd $i>1$, the group on the right vanishes by contractibility and the induction hypothesis, while the group on the left vanishes because $i-1$ is positive and even and is neither $0$ nor $2n-1$. Thus the middle group vanishes. For $i=1$, the preceding map

$$
H^0(U)\oplus H^0(V)\longrightarrow H^0(U\cap V)
$$

is surjective because all three spaces are connected, so the connecting map into $H^1(\mathbb{CP}^n)$ is zero. Therefore all odd de Rham cohomology groups of $\mathbb{CP}^n$ vanish.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
