<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Gelfond–Schneider theorem](../../../../../gelfond-schneider-theorem.md) says that if $a\ne0,1$ is algebraic and $b$ is algebraic irrational, every number $e^{b\lambda}$ with $e^\lambda=a$ is transcendental. Thus the statement includes every determination of the power, not merely a chosen principal branch.

Here is an auxiliary-function outline with the arithmetic and analytic steps specified. Assume $v=e^{b\lambda}$ were algebraic, and put $K=\mathbb Q(a,b,v)$, $d=[K:\mathbb Q]$. For a large [integer](../../../../../integer.md) $T$, choose degrees $L_1\asymp T\log T$ and $L_2\asymp T/\log T$, with constants large enough that $(L_1+1)(L_2+1)>2d(T+1)^2$. Apply [Siegel lemma](../../../../../siegel-s-lemma.md) to impose

$$
P(s+tb,a^sv^t)=0\qquad(0\leq s,t\leq T)
$$

on a nonzero [polynomial](../../../../../polynomial-split.md) $P(X,Y)\in\mathbb Z[X,Y]$ of these two degrees. Each field equation gives at most $d$ rational equations. Clearing denominators and bounding conjugates gives equation-coefficient logarithmic size $O(L_1\log T+L_2T)$; the surplus of variables therefore permits coefficient height $H$ with

$$
\log H=O(L_1\log T+L_2T)=o(T^2).
$$

The [entire function](../../../../../entire-function.md) $F(z)=P(z,e^{\lambda z})$ is nonzero: its [polynomial](../../../../../polynomial-split.md)-exponential terms have distinct exponents $j\lambda$, and their independence follows by the differential-operator argument in question 2. Here $\lambda\ne0$. Its maximum modulus satisfies $\log M_F(R)=O(\log H+L_1\log R+L_2R)$. The grid points $s+tb$ are distinct because $b$ is irrational, and lie in a disk of radius $(1+|b|)T$.

Suppose the vanishing grid has been extended to $0\leq s,t\leq B$, for some $B\geq T$. Divide $F$ by the product of its $(B+1)^2$ known linear zero factors and use the maximum principle on a disk of radius $C B$, with $C$ large and fixed. At a point of the doubled grid, the quotient estimate gives

$$
\log|F(s+tb)|\leq-c_1B^2+O(\log H+L_1\log B+L_2B),\qquad0\leq s,t\leq2B,
$$

if the value is nonzero. But this value equals the [algebraic number](../../../../../algebraic-number.md) $P(s+tb,a^sv^t)$. Clearing its denominators and taking its norm gives the opposite bound

$$
\log|F(s+tb)|\geq-C_1(\log H+L_1\log B+L_2B).
$$

For sufficiently large initial $T$, the terms on the right are $o(B^2)$ uniformly for every $B\geq T$: $L_2/B=O(1/\log T)$ and $L_1\log B/B^2=O((\log T)^2/T)$. Thus every doubled-grid value must be zero. Iterating doubles the grid indefinitely. This supplies quadratically many distinct zeros in disks of linearly growing radius, whereas [Jensen's formula](../../../../../jensen-s-formula.md) and the exponential-[polynomial](../../../../../polynomial-split.md) growth bound allow only $O(R)$ zeros for a nonzero $F$. The contradiction proves the theorem. This is the [Schneider lattice proof of the Gelfond–Schneider theorem](../../../../../schneider-lattice-proof-of-the-gelfond-schneider-theorem.md).

Now fix any [logarithms](../../../../../logarithm.md) of algebraic $\alpha,\beta\ne0,1$. Their values are nonzero. If $q=\log\alpha/\log\beta$ were algebraic irrational, then $e^{q\log\beta}=\alpha$ would be algebraic, contradicting the theorem with base $\beta$. Hence

$$
\boxed{\frac{\log\alpha}{\log\beta}\text{ is either rational or transcendental}.}
$$

For arbitrarily many [logarithms](../../../../../logarithm.md) the qualitative [Baker theorem on algebraic linear combinations of logarithms](../../../../../baker-s-theorem.md) states that [logarithms](../../../../../logarithm.md) of [algebraic numbers](../../../../../algebraic-number.md) which are linearly independent over $\mathbb Q$ remain independent over $\overline{\mathbb Q}$, even after adjoining one to the list. Equivalently a nonzero homogeneous algebraic-coefficient linear combination of such [logarithms](../../../../../logarithm.md) is transcendental. Rational relations are therefore the only source of homogeneous algebraic relations among the chosen [logarithms](../../../../../logarithm.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
