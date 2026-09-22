<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [chain map](../../../../../../chain-map.md) identity $d_Df=fd_C$ gives, for $(x,y)\in M_i$,

$$
d_f^2(x,y)=\left(d_C^2x,
(-1)^{i-1}f(d_Cx)+(-1)^id_Df(x)+d_D^2y\right)=(0,0).
$$

Thus $M$ is a [chain complex](../../../../../../chain-complex.md); it is a sign convention for the algebraic [mapping cone](../../../../../../mapping-cone-homological-algebra.md).

Put $E_i=C_{i-1}$ with differential $d_E=d_C$. Inclusion into the second summand and projection onto the first give a [short exact sequence of chain complexes](../../../../../../short-exact-sequence-of-chain-complexes.md)

$$
0\longrightarrow D\xrightarrow{\iota}M\xrightarrow{\rho}E\longrightarrow0.
$$

Its [connecting homomorphism](../../../../../../connecting-homomorphism.md) is particularly explicit. If $x\in C_{i-1}$ is a [chain cycle](../../../../../../chain-cycle.md), lift it to $(x,0)\in M_i$ and take its boundary. The second component is $(-1)^if(x)$, so the [long exact sequence in homology](../../../../../../long-exact-sequence-in-homology.md) contains

$$
\cdots\longrightarrow H_i(C)\xrightarrow{(-1)^{i+1}f_*}H_i(D)
\longrightarrow H_i(M)\longrightarrow H_{i-1}(C)
\xrightarrow{(-1)^if_*}H_{i-1}(D)\longrightarrow\cdots.
$$

If every $H_i(M)$ vanishes, the [exact sequence](../../../../../../exact-sequence.md) makes every $f_*$ both injective and surjective. Conversely, if every $f_*$ is an [isomorphism](../../../../../../isomorphism.md), the map $H_i(D)\to H_i(M)$ has zero image, while $H_i(M)\to H_{i-1}(C)$ has zero image and zero kernel; hence $H_i(M)=0$.

One can also see the converse directly on [chain cycles](../../../../../../chain-cycle.md). If $(x,y)\in M_i$ is a [chain cycle](../../../../../../chain-cycle.md), then $d_Cx=0$ and $d_Dy=-(-1)^if(x)$. Injectivity of the [induced map on homology](../../../../../../induced-map-on-homology.md) $f_*$ gives $x=d_Cz$. Subtracting the [chain boundary](../../../../../../chain-boundary.md) $d_f(z,0)$ leaves $(0,t)$ with $d_Dt=0$. Surjectivity of the [induced map on homology](../../../../../../induced-map-on-homology.md) $f_*$ lets us choose a [chain cycle](../../../../../../chain-cycle.md) $w\in C_i$ and $v\in D_{i+1}$ such that

$$
t=(-1)^{i+1}f(w)+d_Dv.
$$

Then $(0,t)=d_f(w,v)$. Thus every [chain cycle](../../../../../../chain-cycle.md) in $M$ is a [chain boundary](../../../../../../chain-boundary.md), proving the [mapping cone acyclicity criterion](../../../../../../mapping-cone-acyclicity-criterion.md):

$$
\boxed{H_*(M)=0\quad\Longleftrightarrow\quad f\text{ is a quasi-isomorphism}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
