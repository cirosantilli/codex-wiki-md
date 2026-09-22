<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

Write a point of the band $X$ as $(u,t)$ with $u\in S^2$, $|t|\leq1/2$, after rescaling the radius of the first three coordinates. The antipodal identification is

$$
(u,t)\sim(-u,-t).
$$

The homotopy $(u,t)\mapsto(u,(1-s)t)$ is equivariant under this identification, so it descends to a deformation retraction of $Y$ onto the central slice

$$
S^2/(u\sim-u)=\mathbb{RP}^2.
$$

Thus

$$
\boxed{Y\simeq\mathbb{RP}^2.}
$$

The two boundary spheres of $X$ are exchanged by the antipodal map, so $\partial Y\cong S^2$. This is the [mapping-cylinder model of punctured real projective three-space](../../../../../mapping-cylinder-model-of-punctured-real-projective-three-space.md).

The standard cellular chain complex for $\mathbb{RP}^3$, with one cell in each dimension zero through three, has boundary maps alternating between multiplication by two and zero:

$$
0\longrightarrow\mathbb Z
\xrightarrow{0}\mathbb Z
\xrightarrow{2}\mathbb Z
\xrightarrow{0}\mathbb Z
\longrightarrow0.
$$

Therefore the [integral homology of real projective three-space](../../../../../integral-homology-of-real-projective-three-space.md) is

$$
\boxed{
H_i(\mathbb{RP}^3;\mathbb Z)=
\begin{cases}
\mathbb Z,&i=0,3,\\
\mathbb Z/2,&i=1,\\
0,&\text{otherwise}.
\end{cases}}
$$

In particular,

$$
H_0(Y)=\mathbb Z,\qquad
H_1(Y)=\mathbb Z/2,\qquad
H_i(Y)=0\quad(i\geq2).
$$

Apply the [Mayer–Vietoris theorem](../../../../../mayer-vietoris-sequence.md) to

$$
Z=Y_1\cup_{\partial Y}Y_2,
\qquad
Y_1\cap Y_2\simeq S^2.
$$

The relevant pieces of the long exact sequence are

$$
0\to H_3(Z)\to H_2(S^2)=\mathbb Z\to0
$$

and

$$
0\to(\mathbb Z/2)^2\to H_1(Z)
\to H_0(S^2)\to H_0(Y_1)\oplus H_0(Y_2).
$$

The last map is injective, so

$$
\boxed{
H_i(Z;\mathbb Z)=
\begin{cases}
\mathbb Z,&i=0,3,\\
(\mathbb Z/2)^2,&i=1,\\
0,&\text{otherwise}.
\end{cases}}
$$

Since $\partial Y\cong S^2$ is simply connected and $\pi_1(Y)\cong\pi_1(\mathbb{RP}^2)\cong\mathbb Z/2$, the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) gives

$$
\boxed{
\pi_1(Z,z_0)\cong
(\mathbb Z/2)*(\mathbb Z/2)
\cong D_\infty,}
$$

the [infinite dihedral group](../../../../../infinite-dihedral-group.md). Topologically, $Z$ is the [double of punctured real projective three-space](../../../../../double-of-punctured-real-projective-three-space.md), namely $\mathbb{RP}^3\#\mathbb{RP}^3$.

The universal cover of each copy of $Y$ is $S^3$ with two disjoint open balls removed, homeomorphic to $S^2\times[0,1]$. The universal cover of the double strings infinitely many such cylinders together according to the Cayley line of $D_\infty$. Hence the familiar covering space is

$$
\boxed{\widetilde Z\cong S^2\times\mathbb R.}
$$

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
