<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The payoff $e(x,z)$ is the expected fitness of an individual using strategy $x$ against a population using strategy $z$. The resident $x^*$ is initially common; the mutant $y$ is introduced at small frequency $\epsilon$. Convexity of the strategy set makes their population mixture admissible. If residents have higher expected fitness in every sufficiently small invasion by a fixed mutant, selection works against that mutant: this is an [evolutionarily stable strategy](../../../../../evolutionarily-stable-strategy.md). The allowed upper bound on $\epsilon$ may depend on $y$.

For expected payoffs of mixed strategies, $e(x,z)$ is affine in the population strategy $z$; in a finite matrix game it is $x^TAz$. This property is the basis of the [two-condition criterion for evolutionary stability](../../../../../two-condition-criterion-for-evolutionary-stability.md). For fixed $y\ne x^*$, put

$$
A_y=e(x^*,x^*)-e(y,x^*),\qquad B_y=e(x^*,y)-e(y,y).
$$

Affineness gives the exact invasion difference

$$
e(x^*,(1-\epsilon)x^*+\epsilon y)-e(y,(1-\epsilon)x^*+\epsilon y)=(1-\epsilon)A_y+\epsilon B_y.
$$

If this is positive for all sufficiently small $\epsilon>0$, taking $\epsilon\downarrow0$ gives $A_y\geq0$. If $A_y=0$, the difference is $\epsilon B_y$, so necessarily $B_y>0$. Conversely, if $A_y>0$, it remains positive for sufficiently small $\epsilon$: for example take $\epsilon<A_y/(A_y+|B_y|)$. If $A_y=0$ and $B_y>0$, it is positive for every $\epsilon>0$. Applying this argument separately to every $y$ proves

$$
\boxed{x^*\text{ is ESS}\iff\forall y\ne x^*,\quad A_y\geq0\ \text{and}\ (A_y=0\Rightarrow B_y>0).}
$$

Thus an [evolutionarily stable strategy](../../../../../evolutionarily-stable-strategy.md) is a symmetric [Nash equilibrium](../../../../../nash-equilibrium.md) with an additional condition against tied mutants. For a general nonlinear interaction function on a convex set, affineness would be an additional necessary hypothesis for this particular equivalence; here it follows from the mixed-strategy expected-payoff interpretation. For example, on $X=[0,1]$ take $e(x,z)=xz(x/2-z)$ and resident $x^*=0$. For every $y>0$, $A_y=0$ and $B_y=y^3/2>0$, but at population $\epsilon y$ the mutant earns $\epsilon y^3(1/2-\epsilon)>0$ while the resident earns zero. Thus the two conditions alone would not suffice for an arbitrary nonlinear $e$; the expected-payoff assumption is used explicitly.

For the [Hawk-Dove game](../../../../../hawk-dove-game.md), let $p$ be an individual's Hawk probability and $q$ the population's Hawk probability. The given matrix yields

$$
e(p,q)=\frac{V(1-q)}2+\frac{p(V-Dq)}2,\qquad e(p,q)-e(r,q)=\frac{(p-r)(V-Dq)}2.
$$

We use this formula in each case. In the usual interpretation, resource value $V$ and damage cost $D$ are positive. The parts below also specify the boundary or negative-value alternatives because positivity is not written explicitly in the PDF.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
