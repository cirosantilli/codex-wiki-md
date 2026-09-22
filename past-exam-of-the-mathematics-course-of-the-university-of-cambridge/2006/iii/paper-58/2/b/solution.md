<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The desired output is $|\psi_d\rangle=((\alpha+\beta)|0\rangle+(\alpha-\beta)|1\rangle)/\sqrt2$. To evaluate its [squared quantum fidelity](../../../../../../squared-quantum-fidelity.md), write the input [Bloch vector](../../../../../../bloch-vector.md) as $(x,y,z)$, with $x=c$, $y=2\operatorname{Im}(\alpha^*\beta)$ and $z=d$. The desired vector after the Hadamard is $(z,-y,x)$. From part (a), the actual vector is

$$
r_{\mathrm{out}}=\left(r_k z+\frac{s_k-1}{2}x,
-\frac{s_k+1}{2}y,r_kx\right).
$$

For $k\ge2$ this simplifies to $(1-1/k)(z,-y,x)-(x/k,0,0)$. The [pure state](../../../../../../pure-state.md) overlap is one half of one plus the dot product with the desired unit vector, so

$$
\boxed{\langle\psi_d|\rho|\psi_d\rangle
=1-\frac{1+xz}{2k},\qquad k\ge2.}
$$

Since $x^2+y^2+z^2=1$, $|xz|\le1/2$. Therefore the infidelity is uniformly bounded by $3/(4k)$, and **the [entanglement](../../../../../../entangled-state.md) effect on the implemented gate is negligible for large $k$**, uniformly over all initial pure states. The shifted field packets then have overlaps tending to one, so they retain negligible information about the [qubit](../../../../../../qubit.md) transitions. A large fixed [photon](../../../../../../photon.md) number without this broad number coherence would not suffice.

The printed overlap silently requires $k\ge2$. If the allowed packet has $k=1$, the exact result instead is

$$
\boxed{\langle\psi_d|\rho|\psi_d\rangle
=\frac12+\frac{y^2-xz}{4}.}
$$

For instance, $\alpha=\cos(\pi/8)$ and $\beta=\sin(\pi/8)$ give actual overlap $3/8$, whereas substituting $k=1$ into the printed expression gives $1/4$. This boundary correction follows directly from the two-shift overlap above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
