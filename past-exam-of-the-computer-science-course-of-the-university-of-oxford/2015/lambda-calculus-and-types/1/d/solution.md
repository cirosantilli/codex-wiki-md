<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [structural induction](../../../../../structural-induction.md) on the construction of $p\in\mathcal R$, with the stronger induction claim that $p$ is an [invertible lambda term](../../../../../invertible-lambda-term.md): there is a [lambda term](../../../../../lambda-term.md) $q$ satisfying both

$$
p\bullet q=_{\beta\eta}I,
\qquad q\bullet p=_{\beta\eta}I.
$$

The base constructor has exactly the two-sided inverse proved in part (c). Strengthening the claim is useful because the inductive construction needs inverses of its constituent [lambda terms](../../../../../lambda-term.md) in both orders.

For the inductive constructor, let $t_i$ be the two-sided inverse supplied for $s_i$. Thus, for a fresh variable $u$, [beta-eta equivalence](../../../../../beta-eta-equivalence.md) gives

$$
s_i(t_i u)=_{\beta\eta}u,
\qquad t_i(s_i u)=_{\beta\eta}u
\qquad(1\leq i\leq n).
$$

For $n\geq1$, define

$$
\boxed{q\equiv\lambda z y_1\cdots y_n.\,
z(t_1y_n)(t_2y_1)\cdots(t_ny_{n-1}).}
$$

This [lambda term](../../../../../lambda-term.md) reverses the [cyclic permutation](../../../../../cyclic-permutation.md) and applies the appropriate inverse to each argument. First use [beta reduction](../../../../../beta-reduction.md) to expand one order of [composition of lambda terms](../../../../../composition-of-lambda-terms.md):

$$
\begin{aligned}
(p\bullet q)z
&\longrightarrow_\beta^*\lambda x_1\cdots x_n.\,
(qz)(s_2x_2)\cdots(s_nx_n)(s_1x_1)\\
&\longrightarrow_\beta^*\lambda x_1\cdots x_n.\,
z(t_1(s_1x_1))(t_2(s_2x_2))\cdots(t_n(s_nx_n))\\
&=_{\beta\eta}\lambda x_1\cdots x_n.\,zx_1\cdots x_n
=_\eta z.
\end{aligned}
$$

For the other order, [beta reduction](../../../../../beta-reduction.md) gives

$$
\begin{aligned}
(q\bullet p)z
&\longrightarrow_\beta^*\lambda y_1\cdots y_n.\,
(pz)(t_1y_n)(t_2y_1)\cdots(t_ny_{n-1})\\
&\longrightarrow_\beta^*\lambda y_1\cdots y_n.\,
z(s_2(t_2y_1))\cdots(s_n(t_ny_{n-1}))(s_1(t_1y_n))\\
&=_{\beta\eta}\lambda y_1\cdots y_n.\,zy_1\cdots y_n
=_\eta z.
\end{aligned}
$$

These computations close the stronger induction. For $n=1$, each formula has the single argument involving $s_1$ and $t_1$; for $n=0$, the constructor is $I$ and its inverse is $I$. Every construction is finite, so the inverse is a finite [lambda term](../../../../../lambda-term.md). There is no requirement that this inverse itself belong to $\mathcal R$.

$$
\boxed{\forall p\in\mathcal R\;\exists q:\quad
p\bullet q=_{\beta\eta}I=q\bullet p.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Lambda calculus and types](../../../lambda-calculus-and-types-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
