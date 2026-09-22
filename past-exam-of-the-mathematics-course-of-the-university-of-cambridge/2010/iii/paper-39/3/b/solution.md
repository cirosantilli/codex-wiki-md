<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\nu$ be the common increment law. The [random walk](../../../../../../random-walk.md) has the [Markov property](../../../../../../markov-property.md), since $\xi_{t+1}$ is independent of $\mathcal F_t$ and $X_{t+1}=X_t+\xi_{t+1}$. Its [transition operator](../../../../../../transition-operator.md) is $Ph(x)=\int h(x+z)\nu(dz)$ wherever that integral exists.

Set $V(T,x)=f(x)$. For $1\leq t<T$, suppose the Borel function $V(t+1,\cdot)$ has been constructed and represents $U_{t+1}$. On the Borel set

$$
A_t=\left\{x:\int|V(t+1,x+z)|\nu(dz)<\infty\right\},
$$

define the [optimal stopping value function](../../../../../../optimal-stopping-value-function.md) recursively by

$$
V(t,x)=\max\left\{f(x),\int V(t+1,x+z)\nu(dz)\right\}.
$$

Outside $A_t$, assign the finite Borel value $f(x)$. Measurability of integrals against a fixed probability law proves measurability of both the set and the function. Integrability of $U_{t+1}=V(t+1,X_t+\xi_{t+1})$ and independence imply $X_t\in A_t$ almost surely and

$$
\mathbb E[U_{t+1}\mid\mathcal F_t]
=\int V(t+1,X_t+z)\nu(dz).
$$

The Snell recursion thus proves $U_t=V(t,X_t)$ by induction.

At time zero the generated [sigma-algebra](../../../../../../sigma-algebra.md) is trivial, so $U_0$ is deterministic. Since $X_0=0$, define $V(0,x)=U_0$ for all $x$, with

$$
U_0=\max\{f(0),\mathbb E[V(1,\xi_1)]\}
$$

when $T\geq1$. This supplies a globally finite deterministic representation without assuming integrability of rewards from every unvisited starting state. Hence

$$
\boxed{U_t=V(t,X_t)\quad(0\leq t\leq T).}
$$

With the additional statewise integrability normally used to define a value function for arbitrary starting states, one can instead use the Bellman maximum at time zero too. For $T=0$, the representation is simply $U_0=f(0)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
