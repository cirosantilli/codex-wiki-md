<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $w_{xy}=w_{yx}>0$ for an [edge](../../../../../edge-of-a-graph.md) conductance and $w_x=\sum_{y\sim x}w_{xy}$. Take $s\ne t$, as implicit in a unit source-to-sink [electrical network](../../../../../electrical-network.md). An oriented [current flow](../../../../../current-flow.md) is antisymmetric, $i_{yx}=-i_{xy}$. [Kirchhoff's first law](../../../../../kirchhoff-node-law.md) is conservation of current: $\sum_yi_{xy}=0$ at every vertex other than the source and sink, with the divergences there equal to the prescribed total flow and its negative. [Kirchhoff's second law](../../../../../kirchhoff-cycle-law.md) says that the sum of oriented [voltage](../../../../../voltage.md) drops around any closed cycle is zero. [Ohm's law](../../../../../ohm-s-law.md) is

$$
i_{xy}=w_{xy}(v_x-v_y),\qquad v_x-v_y=\frac{i_{xy}}{w_{xy}}.
$$

Thus the resistance of an [edge](../../../../../edge-of-a-graph.md) is $1/w_{xy}$, and the cycle law reads $\sum_{j=0}^{m-1}i_{x_jx_{j+1}}/w_{x_jx_{j+1}}=0$ for $x_m=x_0$.

Let $\tau=\inf\{n\geq0:X_n=t\}$. Its expectation is finite. Indeed, from each state there is a path to $t$ of length at most $|V|-1$ with positive [probability](../../../../../probability.md); finiteness gives a common lower bound $a>0$ on reaching $t$ within that many steps. The [Markov property](../../../../../markov-property.md) then gives $\mathbb P(\tau>k(|V|-1))\leq(1-a)^k$, proving the assertion. Define the [expected occupation count before absorption](../../../../../expected-occupation-count-before-absorption.md)

$$
G(s,x)=\mathbb E_s\sum_{n=0}^{\tau-1}\mathbf1_{X_n=x},\qquad G(s,t)=0.
$$

[Conditional expectation](../../../../../conditional-expectation.md) at every pre-stopping visit to $x$ gives $\mathbb E_s N_{xy}=G(s,x)p_{xy}$ for the number $N_{xy}$ of directed traversals. Hence the expected signed count is

$$
u_{xy}=G(s,x)p_{xy}-G(s,y)p_{yx}
=w_{xy}\left(\frac{G(s,x)}{w_x}-\frac{G(s,y)}{w_y}\right).
$$

This proves [Ohm's law](../../../../../ohm-s-law.md) with [voltage](../../../../../voltage.md) $v_x=G(s,x)/w_x$, grounded at $v_t=0$. Summing its [voltage](../../../../../voltage.md) drops along a cycle telescopes, proving [Kirchhoff's second law](../../../../../kirchhoff-cycle-law.md).

For [Kirchhoff's first law](../../../../../kirchhoff-node-law.md), count entrances and exits on each stopped path. Their net difference at $x$ is the initial indicator minus the final indicator. Taking expectations,

$$
\sum_yu_{xy}=\mathbb E_s\sum_{n<\tau}\left(\mathbf1_{X_n=x}-\mathbf1_{X_{n+1}=x}\right)
=\mathbf1_{x=s}-\mathbf1_{x=t}.
$$

Thus the source emits exactly one unit, the sink receives one unit, and all other vertices conserve current.

We also establish the uniqueness required for the conclusion. The cycle law implies that [edge](../../../../../edge-of-a-graph.md) [voltage](../../../../../voltage.md) drops are differences of vertex potentials: define a potential by summing drops along a path to $t$, and cycle sums make this independent of the path. If two unit flows obey both laws, their difference has the form $j_{xy}=w_{xy}(h_x-h_y)$ with zero divergence at every vertex. Therefore

$$
0=\sum_x h_x\sum_yj_{xy}
=\sum_{\{x,y\}\in E}w_{xy}(h_x-h_y)^2.
$$

Strict positivity of the conductances and connectedness force $h$ to be constant, so $j=0$. We conclude the [electrical current from stopped random-walk traversals](../../../../../electrical-current-from-stopped-random-walk-traversals.md) identity

$$
\boxed{u_{xy}=i_{xy}\text{ for the unit source-to-sink current}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
