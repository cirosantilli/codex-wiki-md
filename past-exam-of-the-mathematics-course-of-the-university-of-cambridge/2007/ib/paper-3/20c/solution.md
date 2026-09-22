<h1 id="20c/solution">Solution</h1>

↑ **Parent:** [20C](../20c.md)

For the [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md), write a maximization problem as $\max_{x\in D}f(x)$ subject to $g_i(x)\leq c_i$. Here $D$ may already incorporate simple constraints such as nonnegativity. Define the [Lagrangian in optimization](../../../../../optimization-lagrangian.md)

$$
L(x,\lambda)=f(x)-\sum_i\lambda_i(g_i(x)-c_i),\qquad\lambda_i\geq0.
$$

The theorem states that a feasible point $x_*$ is a global maximizer if there are such multipliers for which $x_*$ globally maximizes $L(\cdot,\lambda)$ on $D$ and [complementary slackness](../../../../../complementary-slackness.md) holds: $\lambda_i(g_i(x_*)-c_i)=0$ for every $i$. To prove it, for any feasible $x$ observe that

$$
f(x)\leq L(x,\lambda)\leq L(x_*,\lambda)=f(x_*).
$$

The first inequality uses feasibility and nonnegative multipliers, the second uses global maximization of the [Lagrangian in optimization](../../../../../optimization-lagrangian.md), and the last uses [complementary slackness](../../../../../complementary-slackness.md). Thus **$x_*$ is globally optimal**. No convexity hypothesis is needed for this implication; [concavity](../../../../../concave-function.md) is useful when establishing the required global maximization of $L$ from its [gradient](../../../../../gradient.md).

For the particular problem, put $d=e^{c_2}-1\geq0$ and $R=c_1-2d\geq0$. The logarithmic constraint is equivalent to $x_1\geq d$. The objective increases strictly with either variable, so at a maximum the resource constraint is tight: otherwise $x_1$ could be increased. Hence

$$
x_1=\frac{c_1-3x_2}{2},\qquad0\leq x_2\leq\frac R3.
$$

On this interval the objective becomes $F(x_2)=(c_1-3x_2)/2+3\log(1+x_2)$, with

$$
F'(x_2)=-\frac32+\frac3{1+x_2},\qquad F''(x_2)=-\frac3{(1+x_2)^2}<0.
$$

It increases up to $x_2=1$ and decreases thereafter, so the unique feasible maximizer is

$$
\boxed{x_2^*=\min\left\{1,\frac{c_1-2(e^{c_2}-1)}3\right\},\qquad x_1^*=\frac{c_1-3x_2^*}{2}.}
$$

The maximum value is

$$
\boxed{\begin{cases}
\displaystyle d+3\log(1+R/3),&0\leq R\leq3,\\[3pt]
\displaystyle\frac{c_1-3}{2}+3\log2,&R\geq3.
\end{cases}}
$$

The two expressions agree at $R=3$. This includes the degenerate feasible set $R=0$, where $x_1^*=d$ and $x_2^*=0$.

To certify the result using the [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md), take $D=[0,\infty)^2$ and

$$
L=x_1+3\log(1+x_2)-\lambda(2x_1+3x_2-c_1)+\mu(\log(1+x_1)-c_2),
$$

where $\lambda,\mu\geq0$. Set

$$
\lambda=\frac1{1+x_2^*},\qquad\mu=(2\lambda-1)(1+x_1^*).
$$

Since $x_2^*\leq1$, $\lambda\geq1/2$ and $\mu\geq0$. These choices make both components of $\nabla_xL$ vanish at $x_*$: $1-2\lambda+\mu/(1+x_1^*)=0$ and $3/(1+x_2^*)-3\lambda=0$. The [Lagrangian in optimization](../../../../../optimization-lagrangian.md) is [concave](../../../../../concave-function.md) on $D$, so the zero [gradient](../../../../../gradient.md) proves global maximization there. The resource constraint is tight. When $R<3$ the logarithmic constraint is tight; when $R\geq3$, $\mu=0$. Thus [complementary slackness](../../../../../complementary-slackness.md) holds in every case, including both endpoints, and the theorem establishes the claimed optimum.

## ↑ Ancestors (10)

1. [20C](../20c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
