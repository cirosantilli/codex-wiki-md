<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $P=P_0+dP_1+O(d^2)$ and $r=r_0+dr_1+O(d^2)$, with each coefficient satisfying the zero [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md). The steady complex equation, including the fluctuating coupling, is $0=\mathcal L_rP-dB\sin(2\pi x/\ell)$. Since $B_0=(P_0-P_0^*)/(2i)$, its order-$d$ terms give

$$
\mathcal L_{r_0}P_1=-ir_1P_0'+\frac{P_0-P_0^*}{2i}\sin(2\pi x/\ell).
$$

This is a [regular perturbation](../../../../../../regular-perturbation.md) equation for the threshold shift. The right projection uses the complex [inner product](../../../../../../inner-product.md), not a bilinear product without conjugation.

The [linear operator](../../../../../../linear-operator.md) $\mathcal L_{r_0}$ is self-adjoint on the domain $H^2(0,\ell)\cap H_0^1(0,\ell)$ in complex [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). For functions $v,w$ in that domain, two [integration by parts](../../../../../../integration-by-parts.md) steps give

$$
\int_0^\ell v^*\mathcal L_{r_0}w\,dx
=\int_0^\ell(\mathcal L_{r_0}v)^*w\,dx
+\left[v^*w'-(v^*)'w+ir_0v^*w\right]_0^\ell.
$$

The boundary term vanishes. In particular $ir_0\partial_x$ is formally self-adjoint: both complex conjugation of $i$ and integration by parts contribute a minus sign. Taking $v=P_0$, $w=P_1$ and using $\mathcal L_{r_0}P_0=0$ proves

$$
\int_0^\ell P_0^*\mathcal L_{r_0}P_1\,dx=0.
$$

This is the [Fredholm solvability condition for a self-adjoint operator](../../../../../../fredholm-solvability-condition-for-a-self-adjoint-operator.md). Define $s(x)=\sin(2\pi x/\ell)$ and $N=\int_0^\ell|P_0|^2\,dx$. The gauged sine mode has

$$
I=\int_0^\ell P_0^*P_0'\,dx=-\frac{ir_0}{2}N,
$$

since the real envelope contributes an integral of its own derivative, whose endpoint term is zero. In particular the denominator in the solvability condition is nonzero. Therefore

$$
\boxed{r_1=-\frac{\displaystyle\int_0^\ell P_0^*(P_0-P_0^*)s(x)\,dx}{\displaystyle2\int_0^\ell P_0^*P_0'\,dx}
=\frac{2}{r_0N}\int_0^\ell P_0^*B_0s(x)\,dx.}
$$

For either parity choice this expression is real. Indeed $|P_0|^2$, $A_0^2$ and $B_0^2$ are even about the midpoint, while $s$ is odd. Hence $\int|P_0|^2s=\int B_0^2s=0$, and the last numerator reduces to $\int A_0B_0s$.

No integral evaluation is needed to compare the two shifts. The phase change $P_Q=iP_D$ gives $A_Q=-B_D$, $B_Q=A_D$, and leaves $N$ and $I$ unchanged. Thus $A_QB_Q=-A_DB_D$, and

$$
\boxed{r_{1,Q}=-r_{1,D}.}
$$

Equivalently, the term involving $|P_0|^2$ vanishes by parity, while $(P_Q^*)^2=-(P_D^*)^2$ reverses the remaining perturbation numerator. This is [parity splitting of a mean-field dynamo threshold](../../../../../../parity-splitting-of-a-mean-field-dynamo-threshold.md): the perturbation breaks the phase degeneracy and lowers one onset threshold by the amount it raises the other.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
