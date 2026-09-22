<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $u=u_n\in H^n(K(\mathbb Z/2,n);\mathbb F_2)$ for the fundamental class. We use the path-loop [Serre spectral sequence](../../../../../serre-spectral-sequence.md), its multiplicative structure, and the [Kudo transgression theorem](../../../../../kudo-transgression-theorem.md): transgression of the fundamental classes and their compatible [Steenrod squares](../../../../../steenrod-square.md) is natural, equivalently [cohomology suspension](../../../../../cohomology-suspension.md) commutes with these stable operations. The initial ring is $H^*(K(\mathbb Z/2,1);\mathbb F_2)=\mathbb F_2[t_1]$.

Here is the low-degree calculation. In the first path fibration, $t$, $t^2$ and $t^4$ transgress respectively to $u_2$, $\operatorname{Sq}^1u_2$ and $\operatorname{Sq}^2\operatorname{Sq}^1u_2$, in degrees $2,3,5$. These supply all indecomposable base classes through degree five; the other classes there are products. Repeating the path-loop calculation raises the degree of the transgressive classes by one. For $n=3$, the class $\operatorname{Sq}^2u_3$ transgresses from $u_2^2$, and $\operatorname{Sq}^2\operatorname{Sq}^1u_3$ from the degree-five generator. For $n=4$, $\operatorname{Sq}^3u_4$ transgresses from $u_3^2$. For larger $n$ all four displayed low-degree operations are transgressive indecomposables. Acyclicity of the path-space total [cohomology](../../../../../cohomology-split.md) forces these transgressions and excludes additional classes in this range.

More systematically, this is the range up to $n+3$ of the [Serre polynomial generators for mod-two Eilenberg–MacLane cohomology](../../../../../serre-polynomial-generators-for-mod-two-eilenberg-maclane-cohomology.md):

$$
H^*(K(\mathbb Z/2,n);\mathbb F_2)
=\mathbb F_2[\operatorname{Sq}^Iu_n:
I\text{ admissible},\ e(I)<n].
$$

For an [admissible sequence of Steenrod squares](../../../../../admissible-sequence-of-steenrod-squares.md), $I=(i_1,\ldots,i_r)$ has $i_j\geq2i_{j+1}$; its degree increment is $\sum i_j$, and its [Steenrod excess](../../../../../excess-of-an-admissible-steenrod-sequence.md) is $e(I)=i_1-i_2-\cdots-i_r$. Include the empty sequence. Up to increment three the nonempty possibilities are $(1),(2),(3),(2,1)$; the strict excess bound and possible products explain precisely the small-$n$ exceptions.

**The [low-degree mod-two cohomology of an Eilenberg–MacLane space](../../../../../low-degree-mod-two-cohomology-of-an-eilenberg-maclane-space.md) is**

$$
\boxed{
H^i=
\begin{cases}
\mathbb F_2\{1\},&i=0,\\
0,&0<i<n,\\
\mathbb F_2\{u\},&i=n,\\
\mathbb F_2\{\operatorname{Sq}^1u\},&i=n+1,\\
\mathbb F_2\{\operatorname{Sq}^2u\},&i=n+2,\\
\mathbb F_2\{u\operatorname{Sq}^1u,\,
\operatorname{Sq}^2\operatorname{Sq}^1u\},&i=n+3,\ n=2,\\
\mathbb F_2\{\operatorname{Sq}^3u,\,
\operatorname{Sq}^2\operatorname{Sq}^1u\},&i=n+3,\ n\geq3.
\end{cases}}
$$

Negative-degree [cohomology](../../../../../cohomology-split.md) is zero. For $n=2$, $\operatorname{Sq}^2u=u^2$ and $\operatorname{Sq}^3u=0$ by instability, so the product in degree five must not be omitted. For $n=3$, $\operatorname{Sq}^3u=u^2$ is a product, still independent from $\operatorname{Sq}^2\operatorname{Sq}^1u$. For $n\geq4$ the listed classes are indecomposable. The [Adem relations](../../../../../adem-relations.md) include $\operatorname{Sq}^1\operatorname{Sq}^1=0$ and $\operatorname{Sq}^1\operatorname{Sq}^2=\operatorname{Sq}^3$, so no further increment-three class comes from reversing the two squares.

Now use the space actually printed in the PDF,

$$
Y=\mathbb{RP}^{10}/\mathbb{RP}^{6};
$$

the converted TeX dropped the projective-space $P$'s. This [stunted real projective space](../../../../../stunted-real-projective-space.md) has one cell in dimensions $7,8,9,10$, besides its basepoint, and is $6$-connected. The integral cellular boundary is $2$ in even dimensions and zero in odd dimensions. Hence

$$
\widetilde H_i(Y;\mathbb Z)=
\begin{cases}\mathbb Z/2,&i=7,9,\\0,&\text{otherwise}.\end{cases}
$$

The [Hurewicz theorem](../../../../../hurewicz-theorem.md) gives $\pi_7(Y)=\mathbb Z/2$.

For the next two groups, let $K=K(\mathbb Z/2,7)$ and choose $f:Y\to K$ representing the generator of $H^7(Y;\mathbb F_2)$. It induces an isomorphism on $\pi_7$, and the target's higher [homotopy groups](../../../../../homotopy-group.md) vanish.

We need the [low-degree integral homology of a mod-two Eilenberg–MacLane space](../../../../../low-degree-integral-homology-of-a-mod-two-eilenberg-maclane-space.md). Here it is

$$
H_7(K;\mathbb Z)=\mathbb Z/2,\quad H_8(K;\mathbb Z)=0,\quad
H_9(K;\mathbb Z)=\mathbb Z/2,\quad H_{10}(K;\mathbb Z)=\mathbb Z/2.
$$

To justify the torsion orders, the [Serre class](../../../../../serre-class.md) theorem first makes every positive-degree integral [homology](../../../../../homology-split.md) group of $K$ a finite 2-group. The [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) with $\mathbb F_2$ and the low-degree dimensions give one cyclic summand in degrees seven, nine and ten and none in degree eight. The mod-two [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) is $\operatorname{Sq}^1$. Its relevant nonzero actions are

$$
u\mapsto\operatorname{Sq}^1u,\qquad
\operatorname{Sq}^2u\mapsto\operatorname{Sq}^3u,\qquad
\operatorname{Sq}^2\operatorname{Sq}^1u
\mapsto\operatorname{Sq}^3\operatorname{Sq}^1u.
$$

The last target is nonzero: $(3,1)$ is admissible with excess two, below seven. It also follows by transgressing the nonzero square $(\operatorname{Sq}^1u_2)^2$ through successive path fibrations. Each nonzero Bockstein pairs the mod-two classes associated with a cyclic integral summand of order exactly two; for a summand of order $2^r$ with $r>1$, this first Bockstein would be zero. In degree ten, $\operatorname{Sq}^3u$ is already the Ext class from $H_9$, so the independent class $\operatorname{Sq}^2\operatorname{Sq}^1u$ detects $H_{10}$. This proves all four integral groups without confusing them with mod-two Betti numbers.

Let $x\in H^1(\mathbb{RP}^{10};\mathbb F_2)$ be its usual generator. The quotient classes in degrees $7$ through $10$ identify with $x^7,\ldots,x^{10}$ via the pair's [cohomology](../../../../../cohomology-split.md). The [Steenrod squares on real projective space](../../../../../steenrod-squares-on-real-projective-space.md) satisfy

$$
\operatorname{Sq}^j(x^r)=\binom rj x^{r+j}.
$$

Thus

$$
f^*u=x^7,\quad
f^*\operatorname{Sq}^1u=x^8,\quad
f^*\operatorname{Sq}^2u=x^9,\quad
f^*\operatorname{Sq}^3u=x^{10},\quad
f^*\operatorname{Sq}^2\operatorname{Sq}^1u=0,
$$

since $\binom72$ and $\binom73$ are odd, while $\binom82$ is even. In degree nine, the nonzero [cohomology](../../../../../cohomology-split.md) map detects the map on $H_9$, as $H_8=0$ on both sides. Consequently $f_*:H_9(Y;\mathbb Z)\to H_9(K;\mathbb Z)$ is an isomorphism.

Treat $f$ as a mapping-cylinder pair $(K,Y)$. It is $8$-connected: both spaces are $6$-connected, $\pi_7$ is an isomorphism, and $\pi_8(K)=0$. The relative [homology](../../../../../homology-split.md) sequence gives $H_9(K,Y)=0$, since $H_9(Y)\to H_9(K)$ is an isomorphism and $H_8(Y)=0$. The [Relative Hurewicz theorem](../../../../../relative-hurewicz-theorem.md) then gives $\pi_9(K,Y)=0$, and the relative [homotopy](../../../../../homotopy.md) sequence identifies this group with $\pi_8(Y)$. Thus $\pi_8(Y)=0$ and the pair is now $9$-connected.

Next,

$$
H_{10}(K,Y)\cong H_{10}(K)\cong\mathbb Z/2,
$$

because $H_{10}(Y)=0$ and the degree-nine map is an isomorphism. Apply the [Relative Hurewicz theorem](../../../../../relative-hurewicz-theorem.md) again and use $\pi_{10}(K)=\pi_9(K)=0$:

$$
\pi_9(Y)\cong\pi_{10}(K,Y)\cong H_{10}(K,Y)\cong\mathbb Z/2.
$$

Therefore **the [homotopy groups of the stunted projective space through degree nine](../../../../../homotopy-groups-of-the-stunted-projective-space-through-degree-nine.md) are**

$$
\boxed{\pi_i(\mathbb{RP}^{10}/\mathbb{RP}^{6})=
\begin{cases}
0,&1\leq i\leq6,\\
\mathbb Z/2,&i=7,\\
0,&i=8,\\
\mathbb Z/2,&i=9.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
