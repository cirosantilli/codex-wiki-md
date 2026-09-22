<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

The [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) for a maximization problem says the following. Suppose the constraints are $g_i(q)\ge0$ and $h_j(q)=0$, and define

$$
L(q,\lambda,\mu)
=f(q)+\sum_i\lambda_i g_i(q)+\sum_j\mu_jh_j(q),
\qquad \lambda_i\ge0.
$$

If a feasible $q^*$ satisfies [complementary slackness](../../../../../complementary-slackness.md) $\lambda_i g_i(q^*)=0$ and globally maximizes $L(\,\cdot\,,\lambda,\mu)$, then $q^*$ globally maximizes $f$. Indeed, for every feasible $q$,

$$
f(q)\le L(q,\lambda,\mu)
\le L(q^*,\lambda,\mu)
=f(q^*).
$$

This proves the theorem. In a [concave maximization problem](../../../../../concave-function.md), stationarity and the boundary optimality conditions ensure the required global maximum of the Lagrangian.

For the problem at hand, retain $x,z\ge0$ as the domain and attach a multiplier $\lambda$ to the equality:

$$
L=x+y+2a\sqrt{1+z}
+\lambda\left(b-x-\frac12y^2-z\right).
$$

For $\lambda\ge1$, this is concave in $(x,y,z)$ on the domain. Its separate maximizers satisfy

$$
y=\frac1\lambda,
\qquad
z=\max\left(\frac{a^2}{\lambda^2}-1,0\right),
$$

while the $x$ term is $(1-\lambda)x$. Thus $x$ may be positive only when $\lambda=1$; when $\lambda>1$, its maximizing value is $x=0$.

If

$$
b\ge a^2-\frac12,
$$

take $\lambda=1$. Then $y=1$, $z=a^2-1$, and feasibility fixes

$$
x=b-a^2+\frac12\ge0.
$$

The Lagrangian sufficiency theorem gives the maximum

$$
\boxed{(x,y,z)=
\left(b-a^2+\frac12,\,1,\,a^2-1\right)},
$$



$$
\boxed{f_{\max}=b+a^2+\frac32}.
$$

If

$$
\frac12\le b<a^2-\frac12,
$$

then $\lambda>1$ and $x=0$. The equality constraint becomes

$$
\frac1{2\lambda^2}
+\frac{a^2}{\lambda^2}-1=b,
$$

so

$$
\lambda^2=\frac{a^2+1/2}{b+1}.
$$

Consequently

$$
\boxed{x=0,\qquad
y=\sqrt{\frac{2(b+1)}{2a^2+1}},
\qquad
z=\frac{2a^2b-1}{2a^2+1}}.
$$

The assumptions $a\ge1$ and $b\ge1/2$ ensure $z\ge0$. At the stationary point $\sqrt{1+z}=ay$, so the maximum value is

$$
\boxed{f_{\max}
=(1+2a^2)y
=\sqrt{2(b+1)(2a^2+1)}}.
$$

The two formulas agree at $b=a^2-1/2$.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
