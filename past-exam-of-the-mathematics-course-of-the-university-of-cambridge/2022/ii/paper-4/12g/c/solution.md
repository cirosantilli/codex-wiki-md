<h1 id="12g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The set $E=\Delta_2\times\Delta_2$ is a compact convex square. Define

$$
u_i(p,q)=\max\{0,A(e_i,q)-A(p,q)\},
\qquad
p'=\frac{p+u(p,q)}{1+u_1(p,q)+u_2(p,q)}.
$$

Similarly, set

$$
v_j(p,q)=\max\{0,B(p,e_j)-B(p,q)\},
\qquad
q'=\frac{q+v(p,q)}{1+v_1(p,q)+v_2(p,q)}.
$$

These formulae define a continuous self-map $(p,q)\mapsto(p',q')$ of $E$. The square is homeomorphic to a closed disc, so the [Brouwer fixed-point theorem](../../../../../../brouwer-fixed-point-theorem.md) gives a fixed point $(p^*,q^*)$.

Let $U=u_1+u_2$ at that fixed point. From $p'=p$,

$$
u_i=p_iU.
$$

If $U>0$, every $i$ with $p_i>0$ has $A(e_i,q)-A(p,q)>0$. This contradicts bilinearity, because

$$
\sum_i p_i\bigl(A(e_i,q)-A(p,q)\bigr)=0.
$$

Hence $U=0$, all $u_i=0$, and

$$
A(p^*,q^*)\geq A(e_i,q^*)
$$

for both pure strategies. By linearity this holds for every mixed strategy $p$. The same argument with $v_j$ gives

$$
B(p^*,q^*)\geq B(p^*,q)
$$

for every $q$. Therefore

$$
\boxed{
\forall(p,q)\in E,\quad
A(p^*,q^*)\geq A(p,q^*),
\qquad
B(p^*,q^*)\geq B(p^*,q)
}.
$$

In game terms, $p$ and $q$ are the players' [mixed strategies](../../../../../../mixed-strategy.md), and $A,B$ are their expected payoffs in a two-by-two [bimatrix game](../../../../../../bimatrix-game.md). The inequalities say that neither player can improve unilaterally, so $(p^*,q^*)$ is a [Nash equilibrium](../../../../../../nash-equilibrium.md). This is the [Brouwer proof of Nash equilibrium for a two-by-two game](../../../../../../brouwer-proof-of-nash-equilibrium-for-a-two-by-two-game.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12G](../../12g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
