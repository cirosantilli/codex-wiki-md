<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A covering-surface formulation of the [Ahlfors second fundamental theorem](../../../../../ahlfors-second-fundamental-theorem.md) is as follows. For a regular finite bordered [Riemann surface](../../../../../riemann-surfaces.md) $X$ mapped holomorphically to a fixed metric bordered [Riemann surface](../../../../../riemann-surfaces.md) $Y$, let $S=A_f(X)/A(Y)$ be the [average sheet number](../../../../../average-sheet-number.md) and $L$ the pulled-back length of the relative boundary, namely the boundary mapped into the interior of $Y$. With the modern sign convention for the [Euler characteristic](../../../../../euler-characteristic.md),

$$
\max\{-\chi(X),0\}\ge-S\chi(Y)-hL,
$$

where $h$ depends on $Y$ and its metric, not on $X$ or the map. The associated area comparison is $|S_D-S|\le h_DL$ for each fixed regular target region $D$. These formulations and the sign convention are explained in [https://www.math.purdue.edu/~eremenko/dvi/ahl.pdf](https://www.math.purdue.edu/~eremenko/dvi/ahl.pdf) .

The island version of the [Ahlfors second fundamental theorem](../../../../../ahlfors-second-fundamental-theorem.md) for a disk source, which is the useful form here, says that for $q\ge3$ fixed [Jordan domains](../../../../../jordan-domain.md) $D_j$ with disjoint closures on the [Riemann sphere](../../../../../riemann-sphere.md),

$$
\boxed{\sum_{j=1}^q n_j(R)\ge(q-2)S(R)-hL(R).}
$$

Here $n_j$ counts simply connected [islands of a meromorphic function](../../../../../island-of-a-meromorphic-function.md) over $D_j$, once each without weighting by mapping degree, and

$$
S(R)=\frac1{4\pi}\int_{|z|<R}(f^{\#}_{\mathrm{round}})^2dA,\qquad L(R)=\int_{|z|=R}f^{\#}_{\mathrm{round}}|dz|.
$$

An [island of a meromorphic function](../../../../../island-of-a-meromorphic-function.md) is a relatively compact inverse-image component mapped properly onto its target domain; components reaching the source boundary are not counted. The simply connected island estimate is recorded, for spherical disks, in Lemma 2 of [https://pdfs.semanticscholar.org/d247/562607e237af7c8fc6e683b77be6b94829fa.pdf](https://pdfs.semanticscholar.org/d247/562607e237af7c8fc6e683b77be6b94829fa.pdf) . Regular target regions give the same estimate with a region-dependent constant. General [Jordan domains](../../../../../jordan-domain.md) can be enclosed in slightly larger regular [Jordan domains](../../../../../jordan-domain.md) still having disjoint closures. A [simple island](../../../../../simple-island.md) over an enlarged domain restricts to one over the original domain, so it suffices to prove the conclusion for regular domains.

Suppose a nonconstant [meromorphic function](../../../../../meromorphic-function.md) on the plane has no [simple islands](../../../../../simple-island.md) over five such domains. On every counted simply connected island its [proper map](../../../../../proper-map.md) has integer degree at least two. The [area formula](../../../../../area-formula-geometric-measure-theory.md) therefore gives

$$
2n_j(R)\le S_{D_j}(R),\qquad S_{D_j}(R)=\frac1{A(D_j)}\int_{\{|z|<R\}\cap f^{-1}D_j}(f^{\#}_{\mathrm{round}})^2dA.
$$

Together with area comparison and the [Ahlfors second fundamental theorem](../../../../../ahlfors-second-fundamental-theorem.md), this yields

$$
3S(R)\le\sum_jn_j(R)+hL(R)\le\frac52S(R)+CL(R),\qquad \frac12S(R)\le CL(R).
$$

The area comparison can also be seen directly. The two-form $[\mathbf1_D/A(D)-1/(4\pi)]dA$ on the target sphere has zero integral and a bounded one-form primitive. One construction solves its [Poisson equation](../../../../../poisson-equation.md): the gradient of the spherical [Green function](../../../../../green-s-function.md) has an integrable $1/\mathrm{distance}$ singularity, so convolution against the bounded density gives a bounded primitive. Pulling back and applying [Stokes theorem](../../../../../stokes-theorem.md), or smooth approximation at the domain boundary, bounds the integral by a constant times $L(R)$.

We now derive the needed [length-area exhaustion of the complex plane](../../../../../length-area-exhaustion-of-the-complex-plane.md). The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) on a circle gives

$$
L(R)^2\le2\pi R\int_{|z|=R}(f^{\#}_{\mathrm{round}})^2|dz|=8\pi^2R S'(R).
$$

If $L(R)/S(R)\ge\varepsilon>0$ for all sufficiently large $R$, then $S(R)>0$ and

$$
\left(\frac1{S(R)}\right)'=-\frac{S'(R)}{S(R)^2}\le-\frac{\varepsilon^2}{8\pi^2R}.
$$

Integration makes $1/S(R)$ negative, which is impossible. Hence there are radii $R_k\to\infty$ with $L(R_k)/S(R_k)\to0$. This contradicts $S/2\le CL$ and proves the [Ahlfors five islands theorem](../../../../../ahlfors-five-islands-theorem.md): **one of the five target domains has a bounded simply connected inverse-image component mapped biholomorphically onto it**.

Four domains do not suffice. Take the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) $\wp$ for the square lattice $\mathbb Z+i\mathbb Z$. The equation

$$
(\wp')^2=4(\wp-e_1)(\wp-e_2)(\wp-e_3)
$$

shows the three distinct finite branch values $e_1,e_2,e_3$; the fourth is infinity, because all [poles](../../../../../pole.md) are double. Equivalently, the degree-two map from the elliptic torus to the [Riemann sphere](../../../../../riemann-sphere.md) has these four branch values, with all their preimages of local degree two. Choose four small disjoint [Jordan domains](../../../../../jordan-domain.md), each containing one of these [four totally ramified Weierstrass values](../../../../../four-totally-ramified-weierstrass-values.md). A degree-one [island of a meromorphic function](../../../../../island-of-a-meromorphic-function.md) over any one would contain a preimage of its central value of local degree one, contradicting total ramification. Thus **$\wp$ provides four domains with no simple island**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
