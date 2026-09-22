<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The displayed identity is false with the printed non-strict inequality. For example, take $A=B=\{y\}$ and let $r=P_y(\widetilde H_y<\infty)\in(0,1)$. The event $L_y\leq\widetilde H_y$ says that the walk returns to $y$ at most once, so its left side is $\mu_y(1-r^2)$, whereas its right side is $e_{\{y\}}(y)=\mu_y(1-r)$.

The standard and evidently intended [last-exit decomposition for a transient random walk](../../../../../../../last-exit-decomposition-for-a-transient-random-walk.md) has $L_B<\widetilde H_A$. Decompose that corrected event according to $n=L_B$ and $z=X_n\in B$. The [Strong Markov property](../../../../../../../strong-markov-property.md) at time $n$ gives

$$
\mu_yP_y(L_B<\widetilde H_A,L_B\geq0)
=\sum_{n\geq0}\sum_{z\in B}
\mu_yP_y(X_n=z,\widetilde H_A>n)P_z(\widetilde H_B=\infty).
$$

Reversibility of the [random walk on a graph](../../../../../../../random-walk-on-a-graph.md) gives the path-reversal identity

$$
\mu_yP_y(X_n=z,\widetilde H_A>n)
=\mu_zP_z(X_n=y,H_A=n).
$$

Since $e_B(z)=\mu_zP_z(\widetilde H_B=\infty)$ is the [equilibrium measure of a finite set](../../../../../../../equilibrium-measure-of-a-finite-set.md), summing first over $n$ and then over $z$ yields

$$
\boxed{\mu_yP_y(L_B<\widetilde H_A,L_B\geq0)
=\sum_{z\in B}e_B(z)P_z(X_{H_A}=y,H_A<\infty)
=P_{e_B}(X_{H_A}=y,H_A<\infty).}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 226](../../../../paper-226-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
