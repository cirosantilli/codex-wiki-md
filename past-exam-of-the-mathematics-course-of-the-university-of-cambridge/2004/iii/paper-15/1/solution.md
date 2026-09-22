<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose an oriented basis $\omega_1,\omega_2$ of the [period lattice](../../../../../period-lattice.md), so $\operatorname{Im}(\omega_2/\omega_1)>0$. The [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) is constructed by the normally convergent series

$$
\wp(z)=\frac1{z^2}+\sum_{\omega\in\Lambda\setminus\{0\}}\left(\frac1{(z-\omega)^2}-\frac1{\omega^2}\right).
$$

On compact sets away from the lattice the summands are $O(|\omega|^{-3})$, which is summable over a plane lattice. It is even, has double poles at the lattice with zero residues, and is periodic. To check periodicity without splitting divergent series, differentiate termwise: $\wp'(z)=-2\sum_{\omega\in\Lambda}(z-\omega)^{-3}$ is invariant under lattice shifts. Hence $\wp(z+\omega_j)-\wp(z)$ is constant; evenness evaluated at $z=-\omega_j/2$ makes this constant zero.

The [Weierstrass sigma function](../../../../../weierstrass-sigma-function.md) is the canonical product

$$
\boxed{\sigma(z)=z\prod_{\omega\in\Lambda\setminus\{0\}}\left(1-\frac z\omega\right)\exp\left(\frac z\omega+\frac{z^2}{2\omega^2}\right).}
$$

Its logarithmic tails are likewise $O(|\omega|^{-3})$, so it defines an entire function with simple zeros exactly at the lattice and $\sigma'(0)=1$. Pairing opposite lattice factors makes it odd. Its logarithmic derivative is the [Weierstrass zeta function](../../../../../weierstrass-zeta-function.md)

$$
\zeta(z)=\frac{\sigma'(z)}{\sigma(z)}=\frac1z+\sum_{\omega\ne0}\left(\frac1{z-\omega}+\frac1\omega+\frac z{\omega^2}\right),\qquad \zeta'=-\wp.
$$

Thus $\eta_j=\zeta(z+\omega_j)-\zeta(z)$ is constant. Integrating this identity and evaluating the sigma ratio at $z=-\omega_j/2$ gives

$$
\sigma(z+\omega_j)=-e^{\eta_j(z+\omega_j/2)}\sigma(z).
$$

Integration of zeta around a fundamental cell, containing one pole of residue one, gives the [Legendre relation for Weierstrass quasi-periods](../../../../../legendre-relation-for-weierstrass-quasi-periods.md) $\eta_1\omega_2-\eta_2\omega_1=2\pi i$. These formulas explain why sigma itself is not an [elliptic function](../../../../../elliptic-function.md), but balanced products of translates can be.

For completeness, the basic algebraic property of wp is $(\wp')^2=4\wp^3-g_2\wp-g_3$, where $g_2=60\sum_{\omega\ne0}\omega^{-4}$ and $g_3=140\sum_{\omega\ne0}\omega^{-6}$. The identity follows by canceling the principal parts using the Laurent expansion: the difference is an entire elliptic function, hence constant, and its constant term is zero. The discriminant is nonzero; equivalently the three half-period values are distinct. These properties lead to the cubic embedding in 2(ii).

Now let $F$ be a nonzero meromorphic function on the torus and lift it to a periodic meromorphic function on the plane. Its logarithmic derivative $g=F'/F$ is periodic. Choose a fundamental parallelogram with no zero or pole on its boundary. The [residue theorem](../../../../../residue-theorem.md) applied to $g$ gives equality of the total zero and pole multiplicities. Applied to $zg$, it gives the difference of the sums of the zero and pole lifts. Pairing opposite edges explicitly yields

$$
\frac1{2\pi i}\oint zg(z)dz
=\frac{\omega_1}{2\pi i}\int_a^{a+\omega_2}g(z)dz
-\frac{\omega_2}{2\pi i}\int_a^{a+\omega_1}g(z)dz.
$$

Each integral of $F'/F$ on the right is $2\pi i$ times an integer, since its endpoint values of $F$ coincide and the image path avoids zero. Therefore **the zero sum and pole sum agree in $\mathbb C/\Lambda$**.

Conversely, suppose the point sums agree modulo the lattice. Change one chosen lift of a point by a lattice element so the two sums agree exactly in $\mathbb C$; this changes no point of the torus. Then

$$
\boxed{F(z)=\prod_{j=1}^n\frac{\sigma(z-P_j)}{\sigma(z-Q_j)}}
$$

has the prescribed divisor. Its multiplier under either basis period is $\exp(\eta_j(\sum Q_i-\sum P_i))=1$, so it descends to the torus. Repetitions contribute their appropriate multiplicities. This proves the [principality criterion on a complex elliptic curve](../../../../../principality-criterion-on-a-complex-elliptic-curve.md):

$$
\boxed{\operatorname{div}(F)=\sum[P_i]-\sum[Q_i]\iff\sum P_i=\sum Q_i\text{ in }\mathbb C/\Lambda.}
$$

There is an implicit qualification in the wording about separate zero and pole divisors: their supports must be disjoint. If a point occurs on both lists, cancel common multiplicities first when prescribing the divisor difference. A function cannot simultaneously have a zero and a pole at the same point; for example identical one-point lists satisfy the sum condition but do not specify separate zero and pole divisors. For $n=0$, any nonzero constant supplies the empty divisor.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
