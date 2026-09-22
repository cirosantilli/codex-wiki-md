<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

On the [polydisc](../../../../../polydisc.md), put $b_i(z)=f_i(z)-f_i(a)$ and define

$$
F(z)=\sum_{k=1}^n\int_{a_k}^{z_k}b_k(z_1,\ldots,z_{k-1},t,a_{k+1},\ldots,a_n)\,dt.
$$

Each integral is along the straight coordinate segment, which remains in the [polydisc](../../../../../polydisc.md). Holomorphic dependence on parameters and differentiation under the integral show that $F$ is a [holomorphic function](../../../../../holomorphic-function.md). For a fixed $j$, terms with $k<j$ do not depend on $z_j$, and the $k=j$ term contributes $b_j(z_1,\ldots,z_j,a_{j+1},\ldots,a_n)$. If $k>j$, use the assumed symmetry $\partial_jb_k=\partial_kb_j$ to obtain

$$
\partial_j\int_{a_k}^{z_k}b_k(\ldots,t,\ldots)dt=b_j(z_1,\ldots,z_k,a_{k+1},\ldots,a_n)-b_j(z_1,\ldots,z_{k-1},a_k,\ldots,a_n).
$$

These differences telescope. Therefore

$$
\boxed{\frac{\partial F}{\partial z_j}=f_j(z)-f_j(a),\qquad F(a)=0.}
$$

This is the [coordinate-integral primitive on a polydisc](../../../../../coordinate-integral-primitive-on-a-polydisc.md).

For a closed [holomorphic one-form](../../../../../holomorphic-one-form.md) $\beta=\sum_i c_i dz_i$, closedness is exactly $\partial_ic_j=\partial_jc_i$. The preceding construction plus $\sum_i c_i(a)(z_i-a_i)$ gives a local [holomorphic function](../../../../../holomorphic-function.md) $G$ with $\partial G=\beta$. The kernel of $\partial$ on the [structure sheaf of a complex manifold](../../../../../structure-sheaf-of-a-complex-manifold.md) consists of locally constant functions: holomorphicity already gives $\bar\partial G=0$, and $\partial G=0$ then implies $dG=0$. Thus the [holomorphic Poincaré lemma](../../../../../holomorphic-poincare-lemma.md) gives the short exact sequence of [sheaves](../../../../../sheaf-mathematics.md)

$$
\boxed{0\longrightarrow\underline{\mathbb C}\longrightarrow\mathcal O_M\xrightarrow{\partial}\widetilde\Omega_M^1\longrightarrow0.}
$$

The first object is the complex [constant sheaf](../../../../../constant-sheaf.md), and surjectivity is local, on stalks. It does not say that every global closed [holomorphic one-form](../../../../../holomorphic-one-form.md) has a global primitive.

Now assume compactness. The constancy assertion is for a connected [complex manifold](../../../../../complex-manifold.md); otherwise it holds on each connected component. A smooth complex-valued $u$ with $\partial\bar\partial u=0$ is a [pluriharmonic function](../../../../../pluriharmonic-function.md). Restricting to each complex coordinate line makes it a [harmonic function](../../../../../harmonic-function.md) of one complex variable. Choose $x_0$ where $|u|$ has its global maximum and a coordinate [polydisc](../../../../../polydisc.md) about $x_0$. The allowed harmonic maximum principle makes the first coordinate-line restriction constant. Every point on that line still has the same maximal modulus and the same value, so the second coordinate may then vary without changing $u$. Continue through all coordinates to conclude that $u$ equals $u(x_0)$ on the whole [polydisc](../../../../../polydisc.md). The set where it has this value is closed and, by the same argument at each of its points, open. Connectedness therefore gives **$u$ constant**. In particular global [holomorphic functions](../../../../../holomorphic-function.md) on a compact connected [complex manifold](../../../../../complex-manifold.md) are constant.

For the top-degree pairing, write locally $\theta=g\,dz_1\wedge\cdots\wedge dz_n$. With the complex orientation,

$$
i^{n^2}\theta\wedge\overline\theta=2^n|g|^2\,dx_1\wedge dy_1\wedge\cdots\wedge dx_n\wedge dy_n.
$$

It is everywhere nonnegative and is positive on an open set if $\theta$ is not identically zero. Hence

$$
\boxed{i^{n^2}\int_M\theta\wedge\overline\theta>0,\quad\text{so}\quad\int_M\theta\wedge\overline\theta\ne0.}
$$

The phase factor is necessary: the unnormalized integral need not be a positive real number. This is the [integral pairing of complex top forms](../../../../../integral-pairing-of-complex-top-forms.md).

If $\psi$ is a [holomorphic differential form](../../../../../holomorphic-differential-form.md) of degree $n-1$, then $d\psi=\partial\psi$ has type $(n,0)$ and $d\overline{d\psi}=0$. The graded [Leibniz rule](../../../../../leibniz-rule.md) and [Stokes theorem](../../../../../stokes-theorem.md) give

$$
\int_Md\psi\wedge\overline{d\psi}=\int_Md(\psi\wedge\overline{d\psi})=0.
$$

The positive pairing just proved forces $d\psi=0$. Thus **every holomorphic $(n-1)$-form on a compact complex $n$-manifold is closed**, without a [Kähler metric](../../../../../kahler-metric.md) assumption.

On a compact [complex surface](../../../../../complex-surface.md), this proves closedness of all [holomorphic one-forms](../../../../../holomorphic-one-form.md). Sending such a form to its [de Rham cohomology](../../../../../de-rham-cohomology.md) class defines the required inclusion. Indeed, if $\alpha=df$, its type $(1,0)$ gives $\bar\partial f=0$, so $f$ is a global [holomorphic function](../../../../../holomorphic-function.md) and is constant. Therefore $\alpha=0$.

To prove the zero intersection, let $\alpha,\beta$ be [holomorphic one-forms](../../../../../holomorphic-one-form.md) and suppose $[\alpha]=[\overline\beta]$. There is a smooth complex-valued $f$ with $\alpha-\overline\beta=df$. Its type components are $\partial f=\alpha$ and $\bar\partial f=-\overline\beta$. Closedness of $\beta$ gives $\partial\overline\beta=0$, hence $\partial\bar\partial f=0$. Compact pluriharmonic rigidity now makes $f$ constant and $\alpha=\beta=0$. The two spaces are therefore linearly independent in [de Rham cohomology](../../../../../de-rham-cohomology.md), and conjugation preserves their dimensions:

$$
\boxed{H^0(M,\Omega_M^1)\cap\overline{H^0(M,\Omega_M^1)}=0,\qquad2h^{1,0}\leq b_1.}
$$

For the other bound, take the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) of the short exact sequence above. The map $H^0(M,\underline{\mathbb C})\to H^0(M,\mathcal O_M)$ is an isomorphism, componentwise. Since every global [holomorphic one-form](../../../../../holomorphic-one-form.md) is closed, the relevant portion is

$$
0\longrightarrow H^0(M,\Omega_M^1)\longrightarrow H^1(M,\underline{\mathbb C})\longrightarrow H^1(M,\mathcal O_M).
$$

Identify the middle term with first [de Rham cohomology](../../../../../de-rham-cohomology.md), and the last with $H^{0,1}_{\bar\partial}(M)$ by the [Dolbeault theorem](../../../../../dolbeault-theorem.md). Taking dimensions gives

$$
\boxed{2h^{1,0}\leq b_1\leq h^{1,0}+h^{0,1},\qquad h^{1,0}\leq h^{0,1}.}
$$

These are the [Betti and Hodge bounds for compact complex surfaces](../../../../../betti-and-hodge-bounds-for-compact-complex-surfaces.md).

A strict example is the scalar [Hopf surface](../../../../../hopf-surface.md) $X=(\mathbb C^2\setminus\{0\})/\langle z\mapsto2z\rangle$. Polar coordinates identify it smoothly with $S^3\times S^1$: the dilation fixes the angular coordinate and shifts $\log|z|$ by $\log2$. Its first [Betti number](../../../../../betti-number.md) is one, since its fundamental group is $\mathbb Z$. The proved lower bound then forces $h^{1,0}=0$, and the upper bound forces $h^{0,1}\geq1$. Thus **$h^{1,0}<h^{0,1}$ on this compact complex surface**; no unsupported cohomology computation is needed.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
