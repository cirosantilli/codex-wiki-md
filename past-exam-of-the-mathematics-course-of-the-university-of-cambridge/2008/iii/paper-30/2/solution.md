<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a probability [measure-preserving system](../../../../../measure-preserving-system.md), [ergodicity](../../../../../ergodicity.md) means that every measurable set $A$ satisfying $T^{-1}A=A$ modulo null sets has measure zero or one. Equivalently, the only invariant functions are almost everywhere constant. The [pointwise ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) states that, for $f\in L^1(\mu)$,

$$
\frac1N\sum_{j=0}^{N-1}f(T^jx)\longrightarrow\mathbb E(f\mid\mathcal I)(x)\quad\hbox{almost everywhere},
$$

where $\mathcal I$ is the invariant sigma-algebra; on a probability space the convergence also holds in $L^1$. For an [ergodic transformation](../../../../../ergodicity.md), the limit is the constant $\int f\,d\mu$.

For the [Gauss continued-fraction map](../../../../../gauss-continued-fraction-map.md), the [Gauss measure](../../../../../gauss-measure.md) is the probability measure

$$
\boxed{d\nu(x)=\frac{dx}{(\log2)(1+x)},\qquad 0\leq x\leq1.}
$$

Its density integrates to one and is bounded above and below by positive constants, so it has the same null sets as [Lebesgue measure](../../../../../lebesgue-measure.md). Apart from countably many endpoints, the inverse branches are $h_a(y)=1/(a+y)$, $a=1,2,\ldots$. For a bounded measurable test function $F$, substitution on each branch gives

$$
\begin{aligned}
\int F(Tx)\,d\nu(x)
&=\frac1{\log2}\sum_{a=1}^\infty\int_0^1\frac{F(y)}{(a+y)(a+y+1)}\,dy\\
&=\frac1{\log2}\int_0^1F(y)\sum_{a=1}^\infty\left(\frac1{a+y}-\frac1{a+y+1}\right)\,dy\\
&=\frac1{\log2}\int_0^1\frac{F(y)}{1+y}\,dy=\int F\,d\nu.
\end{aligned}
$$

Thus $T$ is a [measure-preserving transformation](../../../../../measure-preserving-transformation.md). Its definition at zero and the rational branch endpoints does not affect these identities.

For [ergodicity](../../../../../ergodicity.md), we give the full shrinking-cylinder argument. A digit cylinder with first $n$ partial quotients $a_1,\ldots,a_n$ is an interval $I=h((0,1))$, where $h=h_{a_1}\circ\cdots\circ h_{a_n}$ and $T^n\circ h$ is the identity. The [continued fraction convergents](../../../../../continued-fraction-convergent.md) give

$$
h(y)=\frac{p_n+p_{n-1}y}{q_n+q_{n-1}y},\qquad
|h'(y)|=\frac1{(q_n+q_{n-1}y)^2},\qquad
|I|=\frac1{q_n(q_n+q_{n-1})}.
$$

Here $q_n\geq q_{n-1}>0$ after the initial step, and the recurrence $q_n=a_nq_{n-1}+q_{n-2}$ makes $q_n$ tend to infinity at least at the Fibonacci rate. Hence the nested cylinders of every irrational point shrink to that point. The [bounded distortion of continued-fraction cylinders](../../../../../bounded-distortion-of-continued-fraction-cylinders.md) is uniform: the ratio of the largest to the smallest value of $|h'|$ is at most four. Since $1/(1+h(y))$ ranges between $1/2$ and $1$, the density

$$
w(y)=\frac{|h'(y)|}{(\log2)(1+h(y))}
$$

has maximum-to-minimum ratio at most eight. Consequently every measurable $E\subseteq(0,1)$ satisfies

$$
\frac{\nu(h(E))}{\nu(I)}\geq\frac18\operatorname{Leb}(E)\geq\frac{\log2}{8}\nu(E).
$$

The last inequality uses $d\nu/dx\leq1/\log2$.

Now suppose $T^{-1}A=A$ modulo null sets and $\nu(A)>0$. Choose an irrational [density point](../../../../../density-point.md) $x\in A$, and let $I_n$ be its successive digit cylinders. The [Lebesgue density theorem](../../../../../lebesgue-s-density-theorem.md) applies to these intervals even though they need not be centered: an interval of length $\ell$ containing $x$ lies in the centered interval of radius $\ell$, so its relative complement tends to zero. Comparability of the two densities then gives

$$
\frac{\nu(I_n\setminus A)}{\nu(I_n)}\longrightarrow0.
$$

But invariance gives $\mathbf1_A(h(y))=\mathbf1_A(y)$ almost everywhere for each inverse branch of $T^n$. Pulling the exceptional null sets through $h$ is legitimate since $h$ has a positive smooth Jacobian on this fixed branch. Thus the distortion estimate with $E=A^c$ gives

$$
\frac{\nu(I_n\setminus A)}{\nu(I_n)}=\frac{\nu(h(A^c))}{\nu(I_n)}\geq\frac{\log2}{8}\nu(A^c).
$$

Letting $n\to\infty$ forces $\nu(A^c)=0$. Therefore **the Gauss continued-fraction map is ergodic for the [Gauss measure](../../../../../gauss-measure.md)**.

For an irrational $x$, the successive [continued fraction](../../../../../continued-fraction.md) digits satisfy $a_j(x)=\lfloor1/T^{j-1}x\rfloor$. The event that a digit equals two is the interval $(1/3,1/2]$, up to null endpoints. Apply the [pointwise ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) to its indicator:

$$
\begin{aligned}
\frac1N|\{1\leq j\leq N:a_j(x)=2\}|
&\longrightarrow\nu((1/3,1/2])\\
&=\frac{\log(3/2)-\log(4/3)}{\log2}
=\frac{\log(9/8)}{\log2}
=\boxed{\log_2 9-3}.
\end{aligned}
$$

This holds for almost every $x$ with respect to both the [Gauss measure](../../../../../gauss-measure.md) and [Lebesgue measure](../../../../../lebesgue-measure.md), since they have the same null sets.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
