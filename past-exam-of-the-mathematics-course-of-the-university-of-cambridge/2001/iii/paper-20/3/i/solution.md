<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Gelfond–Schneider theorem](../../../../../../gelfond-schneider-theorem.md) says that if $a\ne0,1$ is algebraic and $\beta$ is algebraic irrational, then every value $\exp(\beta\lambda)$ with $e^\lambda=a$ is transcendental. Fix such a nonzero logarithm $\lambda$, and suppose $\gamma=e^{\beta\lambda}$ is algebraic. The [field](../../../../../../field.md) $K=\mathbb Q(a,\beta,\gamma)$ then contains all values needed in [Schneider lattice proof of the Gelfond–Schneider theorem](../../../../../../schneider-lattice-proof-of-the-gelfond-schneider-theorem.md).

Here is an outline including the parameter balance. For a large $L$, choose [polynomial](../../../../../../polynomial-split.md) degrees $M\asymp L\log L$, $N\asymp L/\log L$, with constants large enough that $(M+1)(N+1)>[K:\mathbb Q]L^2$. Impose

$$
P(s+t\beta,a^s\gamma^t)=0\qquad(0\le s,t<L).
$$

Expand these $K$-linear equations in a rational basis and clear denominators. [Siegel lemma](../../../../../../siegel-s-lemma.md) gives a nonzero [integer](../../../../../../integer.md) [polynomial](../../../../../../polynomial-split.md) $P$ with $\log H(P)=O(L^2/\log L)$. This follows because each coefficient in the grid equations has [arithmetic height](../../../../../../height-function.md) $O(M\log L+NL)$ and the ratio of unknowns to constraints stays bounded away from one. The [exponential polynomial](../../../../../../exponential-polynomial.md) $F(z)=P(z,e^{\lambda z})$ is not identically zero: distinct exponentials are independent over the [polynomial](../../../../../../polynomial-split.md) ring, as one sees by successively applying powers of $D-j\lambda$ to kill all but one term.

The irrationality of $\beta$ makes the $L^2$ grid points distinct. Their zeros make subsequent grid values extremely small. More precisely, if a whole $S\times S$ grid has been obtained, take an outer radius $R\asymp S\log S$. Growth gives $\log\max_{|z|=R}|F(z)|\le\log H(P)+O(M\log R+NR)$. The product form of Schwarz's lemma contributes $(C/\log S)^{S^2}$ at the next grid points. Therefore

$$
\log|F(s+t\beta)|\le-cS^2\log\log S\qquad(s,t\le S)
$$

for large initial $L$, unless the value is zero. But every such value is algebraic in the same $K$, since $e^{\lambda(s+t\beta)}=a^s\gamma^t$. Its [arithmetic height](../../../../../../height-function.md) is $O(\log H(P)+M\log S+NS)$, so the Liouville lower bound is incompatible with the displayed upper bound for a nonzero value. Induction extends the zero grid indefinitely.

A fixed nonzero [exponential polynomial](../../../../../../exponential-polynomial.md) has only $O(R)$ zeros in a disc of radius $R$, by its exponential-type growth and [Jensen's formula](../../../../../../jensen-s-formula.md) centered at a nonzero value. The grids give $S^2$ distinct zeros in a disc of radius $O(S)$, a contradiction. Thus **$a^\beta$ is transcendental for every choice of logarithm**, completing the [Schneider lattice proof of the Gelfond–Schneider theorem](../../../../../../schneider-lattice-proof-of-the-gelfond-schneider-theorem.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
