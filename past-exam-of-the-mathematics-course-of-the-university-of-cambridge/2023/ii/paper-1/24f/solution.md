<h1 id="24f/solution">Solution</h1>

↑ **Parent:** [24F](../24f.md)

A [germ of a holomorphic function](../../../../../germ-of-a-holomorphic-function.md) at $z\in D$ is an equivalence class $[f]_z$ of pairs consisting of a neighbourhood $U$ of $z$ and a holomorphic function $f:U\to\mathbb C$. Two pairs represent the same germ if their functions agree on some neighbourhood of $z$.

The [space of germs of holomorphic functions](../../../../../space-of-germs-of-holomorphic-functions.md) is

$$
\mathcal G=\{[f]_z:z\in D\}.
$$

For every holomorphic $f$ on an open $U\subseteq D$, the set

$$
\widetilde U_f=\{[f]_z:z\in U\}
$$

is declared open; these sets form a basis. The forgetful map

$$
\pi:\mathcal G\to D,
\qquad \pi([f]_z)=z,
$$

maps each $\widetilde U_f$ homeomorphically onto $U$. The inverses of these restrictions give the charts defining the complex structure, so $\pi$ is a local biholomorphism.

The evaluation map is

$$
\mathcal E:\mathcal G\to\mathbb C,
\qquad \mathcal E([f]_z)=f(z).
$$

It is well-defined by the germ equivalence relation. On the chart $\widetilde U_f$, its coordinate expression is

$$
\mathcal E\circ(\pi|_{\widetilde U_f})^{-1}(z)=f(z),
$$

which is holomorphic. Hence $\mathcal E$ is analytic, as stated in [evaluation map on a space of germs](../../../../../evaluation-map-on-a-space-of-germs.md).

Now put

$$
D=\mathbb C\setminus\{\zeta:\zeta^8=1\},
\qquad
R=\{(z,w)\in D\times\mathbb C:w^2=z^8-1\}.
$$

This gives the [germ surface of the square root of z to the eighth minus one](../../../../../germ-surface-of-the-square-root-of-z-to-the-eighth-minus-one.md). An explicit gluing description is obtained by pairing the eight roots into four adjacent pairs and cutting the plane along four disjoint arcs joining the members of each pair. On the complement of the cuts choose one branch $q(z)$ of $\sqrt{z^8-1}$. Take two copies, labelled by $q$ and $-q$, and glue the upper bank of each cut in one copy to the lower bank in the other, and conversely. The cut interiors are restored by the gluing, while the eight endpoints remain absent because they are not in $D$.

On this surface define

$$
\pi(z,w)=z,
\qquad
\mathcal E(z,w)=w.
$$

For each $(z,w)\in R$, the [holomorphic function](../../../../../holomorphic-function.md) $z^8-1$ is nonzero near $z$, so it has a unique local square root $q$ with $q(z)=w$. Define

$$
\Phi:R\longrightarrow\mathcal G,
\qquad
\Phi(z,w)=[q]_z.
$$

This is well-defined, injective, and analytic in the displayed local sheets; its inverse on its image is $[q]_z\mapsto(z,q(z))$. Thus $\Phi$ is the required analytic embedding, and it intertwines both the forgetful and evaluation maps.

To compactify, first add one point above each of the eight roots of unity. These are simple branch points of the double cover. Since the polynomial has even degree eight, the [even-degree hyperelliptic model](../../../../../even-degree-hyperelliptic-model.md) has two distinct, unbranched points above infinity. Consequently

$$
|\overline R\setminus R|=8+2=10.
$$

Finally apply the [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) to the degree-two meromorphic map $\bar\pi:\overline R\to\mathbb C_\infty$. Its only ramification consists of the eight simple finite branch points, so

$$
2g(\overline R)-2
=2(2g(\mathbb C_\infty)-2)+8
=2(-2)+8=4.
$$

Therefore

$$
\boxed{g(\overline R)=3.}
$$

This is the [compactification of y squared equals x to the eighth minus one](../../../../../compactification-of-y-squared-equals-x-to-the-eighth-minus-one.md).

## ↑ Ancestors (10)

1. [24F](../24f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
