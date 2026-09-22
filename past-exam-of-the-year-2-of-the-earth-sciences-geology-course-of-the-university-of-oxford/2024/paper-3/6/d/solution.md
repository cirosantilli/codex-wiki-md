<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [null space](../../../../../kernel-of-a-linear-map-split.md) consists of [concentration](../../../../../concentration.md) patterns on which transport produces no change. Here it is the family

$$
\boxed{\mathbf c=\alpha\mathbf1.}
$$

Every box has the same [concentration](../../../../../concentration.md). [Ocean circulation](../../../../../ocean-circulation.md) may continue, but inflow and outflow of the [chemical tracer](../../../../../chemical-tracer.md) balance in each box. With $\mathbf b=0$ these are exactly the [steady states](../../../../../steady-state.md); physically admissible members have $\alpha\ge0$. With nonzero $\mathbf b$, adding $\alpha\mathbf1$ to any particular [steady state](../../../../../steady-state.md) leaves its transport balance unchanged, but a [null space](../../../../../kernel-of-a-linear-map-split.md) [vector](../../../../../vector.md) alone need not balance the sources and sinks.

To identify the tracer inventory, apply [conserved inventory from a left null vector](../../../../../conserved-inventory-from-a-left-null-vector.md). Directly summing each column gives

$$
\mathbf1^TA=(-2+2,\ 1-2+1,\ -2+2,\ 1+1-2)=(0,0,0,0).
$$

Consequently, for the supplied [ordinary differential equations](../../../../../ordinary-differential-equation.md),

$$
M(t)=\mathbf1^T\mathbf c(t),\qquad
\frac{dM}{dt}=-\mathbf1^T\mathbf b.
$$

For $\mathbf b=0$, $M$ is a [conserved quantity](../../../../../conserved-quantity.md). The connected [box model](../../../../../box-model.md) equalizes [concentrations](../../../../../concentration.md), approaching the unique member of the [null space](../../../../../kernel-of-a-linear-map-split.md) with the initial inventory:

$$
\boxed{\mathbf c(t)\longrightarrow\frac{\mathbf1^T\mathbf c(0)}4\mathbf1.}
$$

The [arithmetic mean](../../../../../arithmetic-mean.md) is appropriate here because the supplied [matrix](../../../../../matrix.md) has zero column sums. In a general [box model](../../../../../box-model.md) the conserved quantity is $w^T\mathbf c$, where $w$ is a positive [left null space](../../../../../left-null-space.md) [vector](../../../../../vector.md); for physical [concentrations](../../../../../concentration.md) expressed per unit [volume](../../../../../volume.md), these weights represent the box [volumes](../../../../../volume.md) up to a common factor. One must establish the weights from the equations, rather than infer equal [volumes](../../../../../volume.md) from a schematic drawing.

Nonnegative initial [concentrations](../../../../../concentration.md) remain nonnegative under transport alone. Indeed $A+2I$ is a [nonnegative matrix](../../../../../nonnegative-matrix.md), so

$$
e^{tA}=e^{-2t}\sum_{k=0}^{\infty}\frac{t^k(A+2I)^k}{k!}
$$

has nonnegative entries for $t\ge0$: it is a [positive matrix semigroup](../../../../../positive-matrix-semigroup.md). Its column sums are one by $\mathbf1^TA=0$. To see why equalization occurs, set $d=\mathbf c-(M/4)\mathbf1$ for $\mathbf b=0$; then $\mathbf1^Td=0$ and

$$
\frac{d}{dt}\frac{\|d\|_2^2}{2}
=d^TAd=-\frac12\bigl[3(d_1-d_2)^2+(d_1-d_4)^2+(d_2-d_3)^2+3(d_3-d_4)^2\bigr].
$$

The right side vanishes only for constant $d$, which in the zero-sum [vector subspace](../../../../../vector-subspace.md) means $d=0$. Its strict negative bound on the [unit sphere](../../../../../unit-sphere.md) in that [vector subspace](../../../../../vector-subspace.md) gives decay to zero. Thus the [matrix exponential](../../../../../matrix-exponential.md) redistributes inventory without creating negative [concentrations](../../../../../concentration.md); arbitrary prescribed sinks can still exhaust the tracer if they are allowed to act indefinitely.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
