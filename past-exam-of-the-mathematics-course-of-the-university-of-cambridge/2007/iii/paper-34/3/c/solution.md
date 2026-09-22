<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [quantum state ensemble](../../../../../../quantum-state-ensemble.md) $\mathcal E=\{p_i,\rho_i\}$ with average $\overline\rho=\sum_ip_i\rho_i$, the [Holevo quantity](../../../../../../holevo-quantity.md) is

$$
\boxed{\chi(\mathcal E)=S(\overline\rho)-\sum_ip_iS(\rho_i)=\sum_ip_iD(\rho_i\Vert\overline\rho).}
$$

The second equality follows by expanding the trace definition: $\sum_ip_i\operatorname{Tr}\rho_i\log\overline\rho=\operatorname{Tr}\overline\rho\log\overline\rho$. All positive-weight states are supported within $\overline\rho$, so the expression is finite.

For a [CPTP map](../../../../../../quantum-channel.md) $\Lambda$, the output average is $\Lambda(\overline\rho)$, with unchanged probabilities $p_i$. The [data-processing inequality for quantum relative entropy](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) gives

$$
\begin{aligned}
\chi(\Lambda\mathcal E)
&=\sum_ip_iD(\Lambda(\rho_i)\Vert\Lambda(\overline\rho))\\
&\leq\sum_ip_iD(\rho_i\Vert\overline\rho)
=\chi(\mathcal E).
\end{aligned}
$$

Thus **the Holevo quantity cannot increase under a quantum channel**.

The underlying monotonicity can also be seen directly from [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md). Attach the classical label $X$, and realize $\Lambda$ by a [Stinespring representation of a completely positive map](../../../../../../stinespring-representation-of-a-completely-positive-map.md) with output $B$ and discarded environment $E$. The isometry preserves $I(X:BE)$, whose input value is $\chi(\mathcal E)$. The difference from the output value is

$$
I(X:BE)-I(X:B)=S(XB)+S(BE)-S(B)-S(XBE)\geq0,
$$

which is precisely strong subadditivity. This explains why discarding an environment loses accessible ensemble information.

Here “operation” means the unconditional channel, including the classical outcome when a measurement is retained. Conditioning on a selected outcome can increase the Holevo quantity. For instance, take equally likely vectors $\sqrt a|0\rangle\pm\sqrt{1-a}|1\rangle$, with $1/2<a<1$. Their input Holevo quantity is $h_2(a)<1$. The filter $K=\operatorname{diag}(\sqrt{(1-a)/a},1)$ succeeds on either state with probability $2(1-a)$ and produces the orthogonal states $|+\rangle,|-\rangle$ after normalization. The success-conditioned quantity is $1$. This does not violate the unconditional statement.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
