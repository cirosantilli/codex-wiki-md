<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We specify the convention for [quadratic uniformity of a set](../../../../../../quadratic-uniformity-of-a-set.md). Write $\delta=|A|/N$ and $f=1_A-\delta$ on $[1,N]$, extended by zero elsewhere. Let $\mathcal C_N$ be the integer cubes $(x,h_1,h_2,h_3)$ with all eight vertices in $[1,N]$, and let $T_N=|\mathcal C_N|$. In the eighth-power convention, $A$ is $\alpha$-quadratically uniform when

$$
\frac1{T_N}\sum_{\mathcal C_N}
\prod_{\epsilon\in\{0,1\}^3}\mathcal C^{|\epsilon|}
 f(x+\epsilon_1h_1+\epsilon_2h_2+\epsilon_3h_3)\le\alpha,
$$

where $\mathcal C$ means complex conjugation. This quantity is nonnegative and is the eighth power of the normalized [Gowers U3 norm on an interval](../../../../../../gowers-u3-norm-on-an-interval.md). If uniformity instead means that the norm itself is at most $\alpha$, replace the present parameter by $\alpha^8$. Removing the balance would not define density-relative uniformity.

Embed the interval in $G=\mathbb Z/M\mathbb Z$ with $M=12N+1$, and keep the zero extension of $f$. This group has invertible $2$ and $3$. Every cube with all vertices in the interval is an integer cube: its face relations have magnitude at most $2N<M$, so their modular equalities are ordinary equalities. Conversely every such integer cube gives one modular cube. Thus

$$
\|f\|_{U^3(G)}^8=\frac{T_N}{M^4}\|f\|_{U^3(N)}^8\le\alpha,
$$

since $T_N\le M^4$. The cube quantity is nonnegative, for it can be written as an average of squares of two-fold multiplicative-derivative correlations, by expanding the third increment.

We prove the counting estimate needed below. For functions $|u_j|\le1$, put

$$
\Lambda_4(u_0,u_1,u_2,u_3)=\mathbb E_{x,d}\prod_{j=0}^3u_j(x+jd).
$$

Three applications of [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) give

$$
\boxed{|\Lambda_4(u_0,u_1,u_2,u_3)|\le\min_j\|u_j\|_{U^3(G)}.}
$$

Here are the elimination steps, to make the [generalized von Neumann inequality for four-term progressions](../../../../../../generalized-von-neumann-inequality-for-four-term-progressions.md) explicit. Set $\Delta_hu(x)=u(x)\overline{u(x+h)}$. Reparametrize by the position $x+3d$, and apply Cauchy-Schwarz in that position to eliminate $u_3$. Pairing the two remaining difference variables produces increments $3h,2h,h$ in $u_0,u_1,u_2$. Reparametrize by the position of $u_2$, apply Cauchy-Schwarz to eliminate it, and average over $h$ using Cauchy-Schwarz again. The remaining increments in $u_0$ are $3h,2k$. Finally reparametrize by the position of $u_1$ and eliminate it in the same way. The resulting bound is

$$
|\Lambda_4|^8\le
\mathbb E_{x,h,k,l}\Delta_l\Delta_{2k}\Delta_{3h}u_0(x)
=\|u_0\|_{U^3(G)}^8.
$$

In the last equality $2k$ and $3h$ range freely since their multipliers are units. Each elimination drops only a factor bounded by one; expansion of the squared average gives exactly the stated multiplicative derivative. To target $u_j$ instead, subtract its slope from all four slopes and eliminate the other three factors. The increments are the three nonzero slope differences times independent variables, all among $\pm1,\pm2,\pm3$ and hence invertible. This proves the minimum bound.

Now let $a=1_A$ and $g=\delta1_{[1,N]}$ on $G$. Telescoping the four factors, the difference $\Lambda_4(a,a,a,a)-\Lambda_4(g,g,g,g)$ is a sum of four terms with one balanced factor $f$ and three factors bounded by one. Therefore

$$
|\Lambda_4(a,a,a,a)-\delta^4\Lambda_4(I,I,I,I)|\le4\alpha^{1/8}.
$$

For $N\ge16$, restricting to $1\le x\le\lfloor N/4\rfloor$ and $1\le d\le\lfloor N/8\rfloor$ gives at least $N^2/128$ progressions inside the interval. Since $M\le13N$, $\Lambda_4(I,I,I,I)\ge1/100000$. Choose, for example,

$$
\boxed{\alpha\le\left(\frac{\delta^4}{800000}\right)^8.}
$$

Then $\Lambda_4(a,a,a,a)\ge\delta^4/200000$. Constant progressions contribute only $|A|/M^2\le1/N$. For $N>400000\delta^{-4}$, this is strictly below the displayed lower bound. A nonconstant progression consequently exists. Its four points are actual integer progression points: the two adjacent three-term relations have magnitude less than $M$, so they do not wrap. Hence

$$
\boxed{A\text{ contains a nonconstant four-term arithmetic progression}.}
$$

This proves the [four-term progressions in a quadratically uniform interval set](../../../../../../four-term-progressions-in-a-quadratically-uniform-interval-set.md) criterion, with the parameter normalization and the interval boundary both accounted for.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
