<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The global drift hypothesis as printed is impossible on a finite state space.** Indeed, let $x_*$ minimize $f$. Every possible value of $f(X_{n+1})$ is at least $f(x_*)$, so

$$
\mathbb E[f(X_{n+1})\mid X_n=x_*]\geq f(x_*),
$$

contradicting a decrease by $\delta>0$. Equivalently, its formal iteration would give $\mathbb E_xf(X_n)=f(x)-n\delta$, whereas $f$ is bounded on the finite state space. This is the [constant nonzero drift is impossible on a finite Markov chain](../../../../../../constant-nonzero-drift-is-impossible-on-a-finite-markov-chain.md) obstruction. Thus there is no genuine chain satisfying all the literal premises.

The meaningful intended version imposes the drift only on $S\setminus D$, and stops at $D$. In the [natural filtration](../../../../../../natural-filtration.md) $\mathcal F_n=\sigma(X_0,\ldots,X_n)$, the [Markov property](../../../../../../markov-property.md) then gives, on $\{T>n\}$,

$$
\mathbb E[f(X_{n+1})-f(X_n)\mid\mathcal F_n]=-\delta.
$$

The correct [stopped martingale](../../../../../../stopped-martingale.md) is

$$
\boxed{\widetilde Y_n=f(X_{n\wedge T})+\delta(n\wedge T).}
$$

It is adapted and integrable, since $f$ is bounded and $n\wedge T\leq n$. Its increment equals

$$
\widetilde Y_{n+1}-\widetilde Y_n
=\mathbf1_{\{T>n\}}\bigl(f(X_{n+1})-f(X_n)+\delta\bigr),
$$

whose [conditional expectation](../../../../../../conditional-expectation.md) is zero. Taking [expectations](../../../../../../expected-value.md) yields

$$
\mathbb E_x f(X_{n\wedge T})+\delta\mathbb E_x(n\wedge T)=f(x).
$$

Since $T<\infty$ [almost surely](../../../../../../almost-sure-convergence.md) and $f(X_T)=0$, the [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md) gives $\mathbb E_x f(X_{n\wedge T})\to0$. The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) gives $\mathbb E_x(n\wedge T)\uparrow\mathbb E_xT$, without presupposing its finiteness. Consequently the [constant-drift hitting-time identity](../../../../../../constant-drift-hitting-time-identity.md) is

$$
\boxed{\mathbb E_xT=\frac{f(x)}\delta<\infty.}
$$

For $x\in D$, both sides are zero. Under the repaired hypothesis the unstopped $f(X_n)+n\delta$ need not be a [martingale](../../../../../../martingale-split.md) after hitting $D$; it is the displayed [stopped martingale](../../../../../../stopped-martingale.md) that proves the result.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
