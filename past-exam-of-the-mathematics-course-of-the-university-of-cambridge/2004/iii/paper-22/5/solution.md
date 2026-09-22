<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [cochain complex](../../../../../cochain-complex.md) $E$, define the [shift of a cochain complex](../../../../../shift-of-a-cochain-complex.md) by

$$
\boxed{(\Sigma E)^i=E^{i+1},\qquad d_{\Sigma E}^i=-d_E^{i+1}.}
$$

For a [cochain map](../../../../../cochain-map.md) $a:E\to F$, put $(\Sigma a)^i=a^{i+1}$. This is again a [cochain map](../../../../../cochain-map.md), so the construction is a functor. The sign ensures the standard cone identities; the shifted differential squares to zero. Iteration gives $E[r]^i=E^{i+r}$ and differential $(-1)^rd_E$, and $H^i(E[r])=H^{i+r}(E)$.

For $\phi:E\to F$, its algebraic [mapping cone](../../../../../mapping-cone-homological-algebra.md) is

$$
\boxed{C(\phi)^i=F^i\oplus E^{i+1},\qquad d_C(f,e)=(d_Ff+\phi e,-d_Ee).}
$$

Applying this differential twice gives first component $d_F^2f+d_F\phi e-\phi d_Ee=0$, since $\phi$ is a [cochain map](../../../../../cochain-map.md), and second component $d_E^2e=0$. The maps

$$
u:F\to C(\phi),\quad u(f)=(f,0),\qquad v:C(\phi)\to\Sigma E,\quad v(f,e)=e
$$

are [cochain maps](../../../../../cochain-map.md): $d_Cu(f)=(d_Ff,0)=u(d_Ff)$ and $v(d_C(f,e))=-d_Ee=d_{\Sigma E}v(f,e)$. They are maps of complexes of [sheaves](../../../../../sheaf-mathematics.md), because every displayed operation is a [sheaf](../../../../../sheaf-mathematics.md) morphism in each degree.

The [bounded below derived category of sheaves](../../../../../bounded-below-derived-category-of-sheaves.md) $D(X)=D^+(X)$ can be constructed by first quotienting the category of bounded below [cochain complexes](../../../../../cochain-complex.md) by [cochain homotopy](../../../../../cochain-homotopy.md) and then formally inverting all [quasi-isomorphisms](../../../../../quasi-isomorphism.md). A morphism may be represented by a roof $E\xleftarrow{\sim}E'\to F$. Alternatively, take [injective resolutions of sheaves](../../../../../injective-resolution-of-sheaves.md) and use homotopy classes of maps between the resulting injective complexes. The [cohomology sheaf](../../../../../cohomology-sheaf.md) functors descend to the localization, because they already identify homotopic maps and turn [quasi-isomorphisms](../../../../../quasi-isomorphism.md) into isomorphisms. If $E\cong0$ in $D(X)$, applying these functors gives $\mathcal H^i(E)=0$ for every $i$. Conversely, if all these [sheaves](../../../../../sheaf-mathematics.md) vanish, the unique map $E\to0$ is a [quasi-isomorphism](../../../../../quasi-isomorphism.md), which becomes invertible in $D(X)$. Hence

$$
\boxed{E\cong0\text{ in }D(X)\quad\Longleftrightarrow\quad\mathcal H^i(E)=0\text{ for every }i.}
$$

An [exact triangle in a derived category](../../../../../exact-triangle-in-a-derived-category.md) is a triangle isomorphic to a cone triangle

$$
E\xrightarrow{\phi}F\xrightarrow{u}C(\phi)\xrightarrow{v}\Sigma E.
$$

In particular the last arrow is part of the structure; a mere sequence of three objects with successive composite zero does not suffice.

Suppose $0\to E\xrightarrow{\phi}F\xrightarrow{\psi}G\to0$ is degreewise exact. Define

$$
r:C(\phi)\to G,\qquad r(f,e)=\psi(f).
$$

Then $r(d_C(f,e))=\psi(d_Ff)+\psi\phi(e)=d_G\psi(f)=d_Gr(f,e)$, so $r$ is a [cochain map](../../../../../cochain-map.md). It is natural under maps of short exact sequences. It is degreewise surjective as a [sheaf](../../../../../sheaf-mathematics.md) map, and its kernel can be identified with $E^i\oplus E^{i+1}$ using $(a,e)\mapsto(\phi(a),e)$. In these coordinates the kernel differential is

$$
d(a,e)=(d_Ea+e,-d_Ee).
$$

There is a [contracting homotopy](../../../../../contracting-homotopy.md) $h^i(a,e)=(0,a)$ in degree $i-1$:

$$
dh(a,e)=(a,-d_Ea),\qquad hd(a,e)=(0,d_Ea+e),\qquad dh+hd=\operatorname{id}.
$$

Thus the kernel has zero [cohomology sheaves](../../../../../cohomology-sheaf.md). The [cohomology-sheaf exact sequence](../../../../../cohomology-sheaf-exact-sequence.md) is the sequence of the short exact sequence of complexes $0\to\ker r\to C(\phi)\to G\to0$, or equivalently its ordinary complex-cohomology sequence at every stalk. It follows that $r$ induces isomorphisms of all [cohomology sheaves](../../../../../cohomology-sheaf.md), proving

$$
\boxed{C(\phi)\xrightarrow{\sim}G\text{ is a natural quasi-isomorphism}.}
$$

Under this isomorphism the cone triangle becomes the [exact triangle](../../../../../exact-triangle-in-a-derived-category.md)

$$
E\xrightarrow{\phi}F\xrightarrow{\psi}G\xrightarrow{\delta}\Sigma E,
$$

where $\delta=v\circ r^{-1}$ in the derived category.

For the final construction write $U=S^2\setminus S^1$ and set $A=i_!\mathbb Q_U$, $B=\mathbb Q_{S^2}$, $C=j_*\mathbb Q_{S^1}$, each initially placed in degree zero. The stated sequence $0\to A\to B\to C\to0$ is exact on stalks: on $U$ its first map is an isomorphism and its last [sheaf](../../../../../sheaf-mathematics.md) is zero; on the equator its first [sheaf](../../../../../sheaf-mathematics.md) is zero and the second map is an isomorphism. Take its connecting morphism

$$
\boxed{\mu=\delta:C\longrightarrow A[1]\quad\text{in }D(S^2).}
$$

The source has only $\mathcal H^0(C)=C$, whereas the target has only $\mathcal H^{-1}(A[1])=A$. Therefore every induced map $\mathcal H^i(\mu)$ is zero: in any degree at least one of its source and target is zero. This is a [ghost morphism in a derived category](../../../../../ghost-morphism-in-a-derived-category.md).

To prove the derived morphism itself is nonzero, apply derived global sections, giving the [hypercohomology](../../../../../hypercohomology.md) sequence. The [extension by zero](../../../../../extension-by-zero.md) identifies $H^*(S^2;A)$ with the [compactly supported cohomology](../../../../../compactly-supported-cohomology.md) of $U$, and closed direct image identifies $H^*(S^2;C)$ with $H^*(S^1;\mathbb Q)$. The complement $U$ is two open disks, each homeomorphic to $\mathbb R^2$, so

$$
H_c^q(U;\mathbb Q)=\begin{cases}\mathbb Q^2,&q=2,\\0,&q\ne2.\end{cases}
$$

The degree-one part of the resulting exact sequence is

$$
0=H^1(S^2;\mathbb Q)\longrightarrow H^1(S^1;\mathbb Q)=\mathbb Q\xrightarrow{\mu_*}H_c^2(U;\mathbb Q)=\mathbb Q^2\longrightarrow H^2(S^2;\mathbb Q)=\mathbb Q\longrightarrow0.
$$

Thus $\mu_*$ is injective, in particular nonzero. With the hemispheres oriented from $S^2$, the last map is $(a,b)\mapsto a+b$, so an appropriately oriented equator generator maps to $(1,-1)$. A zero morphism in the [derived category of sheaves](../../../../../derived-category-of-sheaves.md) would induce a zero map after derived global sections and taking [cohomology](../../../../../cohomology-split.md). Consequently **$\mu\ne0$, although $\mathcal H^i(\mu)=0$ for every $i$**. This establishes explicitly that the collection of cohomology-sheaf functors detects zero objects but is not faithful on morphisms.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
