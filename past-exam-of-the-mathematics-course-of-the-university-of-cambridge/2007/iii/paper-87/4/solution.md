<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [embedding-projection pair](../../../../../embedding-projection-pair.md) consists of continuous maps $e:D\to E$, $p:E\to D$ with $pe=\operatorname{id}_D$ and $ep\leq\operatorname{id}_E$ pointwise. Thus $e$ is an order embedding and $ep$ approximates an element of the larger domain from below. Such maps are automatically strict: applying the inequality at $\bot_E$ gives $e(\bot_D)\leq ep(\bot_E)\leq\bot_E$, and applying $p$ then gives $p(\bot_E)=\bot_D$.

Suppose $(\phi_{n-1},\psi_{n-1})$ is such a pair. Composition with fixed continuous maps is continuous on the pointwise [function space of complete partial orders](../../../../../function-space-of-complete-partial-orders.md), so both proposed lifted maps are continuous. Their composite on the smaller function space is

$$
\psi_n\phi_n(f)=\psi_{n-1}\phi_{n-1}f\psi_{n-1}\phi_{n-1}=f.
$$

Writing $q=\phi_{n-1}\psi_{n-1}\leq\operatorname{id}$, the other composite is $\phi_n\psi_n(g)=qgq\leq g$: for every $x$, $q(g(qx))\leq g(qx)\leq g(x)$ by monotonicity. Thus **the recursion produces [embedding-projection pairs](../../../../../embedding-projection-pair.md) at every stage**.

Here is an explicit [inverse-limit solution of the reflexive domain equation](../../../../../inverse-limit-solution-of-the-reflexive-domain-equation.md). Form

$$
D_\infty=\{(x_0,x_1,\ldots):x_n\in D_n,\ \psi_n(x_{n+1})=x_n\text{ for all }n\},
$$

ordered coordinatewise. The bottom sequence is coherent by strictness. A directed family has coordinatewise suprema, and continuity of each $\psi_n$ preserves the coherence condition. Thus $D_\infty$ is a [pointed complete partial order](../../../../../pointed-complete-partial-order.md).

Write $\phi_{m,n}:D_m\to D_n$ for the composite embeddings when $m\leq n$, and $\psi_{m,n}:D_n\to D_m$ for the corresponding composite projections, taking both as identities if $m=n$. Define $P_n:D_\infty\to D_n$ by $P_n(x)=x_n$, and define $E_n:D_n\to D_\infty$ by

$$
(E_na)_m=\begin{cases}\psi_{m,n}(a),&m\leq n,\\\phi_{n,m}(a),&m\geq n.\end{cases}
$$

The pair identities make this sequence coherent, and its coordinates are continuous. They also give $P_nE_n=\operatorname{id}_{D_n}$ and $E_nP_n\leq\operatorname{id}_{D_\infty}$. Put $Q_n=E_nP_n$. Since $E_n=E_{n+1}\phi_n$ and $P_n=\psi_nP_{n+1}$,

$$
Q_n=E_{n+1}(\phi_n\psi_n)P_{n+1}\leq Q_{n+1}.
$$

At coordinate $m$, $Q_nx$ equals $x_m$ once $n\geq m$, so

$$
\boxed{Q_n\uparrow\operatorname{id}_{D_\infty}.}
$$

This exhibits the required [embedding-projection pair](../../../../../embedding-projection-pair.md) for every finite stage.

To prove the function-space isomorphism, observe that $x_{n+1}\in D_{n+1}$ is itself a continuous function $f_n:D_n\to D_n$. Coherence says

$$
f_n=\psi_n f_{n+1}\phi_n.
$$

Conversely such a coherent function family determines an element of $D_\infty$, with initial coordinate $x_0=\psi_0(f_0)$. Define its action on the limit by

$$
\mathcal A(x)=\sup_n E_n f_n P_n\ \in[D_\infty\to D_\infty].
$$

The maps inside this supremum increase: substituting coherence expresses the $n$th one as $E_{n+1}q_nf_{n+1}q_nP_{n+1}$ with $q_n=\phi_n\psi_n\leq\operatorname{id}$, which is below the next map. The supremum is continuous by the function-space result in Question 3.

In the other direction, for a continuous $F:D_\infty\to D_\infty$, define $f_n=P_nFE_n$. These satisfy the same coherence equation. Hence define $\mathcal B(F)\in D_\infty$ by

$$
\mathcal B(F)_{n+1}=P_nFE_n,\qquad\mathcal B(F)_0=\psi_0(P_0FE_0).
$$

For a coherent family, restricting $\sup_nE_nf_nP_n$ back to stage $m$ gives $f_m$: every term with $n\geq m$ restricts exactly to $\psi_{m,n}f_n\phi_{m,n}=f_m$, and the earlier terms are below it. Thus $\mathcal B\mathcal A$ is the identity.

Conversely,

$$
\mathcal A\mathcal B(F)=\sup_nQ_nFQ_n=F.
$$

For the last equality, $Q_n\uparrow\operatorname{id}$ and continuity give, at every $x$, $\sup_nQ_nF(Q_nx)=\sup_{n,m}Q_nF(Q_mx)=F(x)$; the diagonal is cofinal because the double family increases in both indices. Both $\mathcal A$ and $\mathcal B$ are continuous, by coordinatewise evaluation, continuous composition and directed suprema. Therefore

$$
\boxed{D_\infty\cong[D_\infty\to D_\infty]}
$$

as complete partial orders with continuous maps, not merely as sets. This supplies the [extensional reflexive object](../../../../../extensional-reflexive-object.md) needed for a beta-eta model, together with all the stated finite-stage pairs.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 87](../../paper-87-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
