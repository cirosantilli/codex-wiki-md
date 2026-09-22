<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For finite $A\subset\mathbb Z$, define the occupation-product function

$$
D(\eta,A)=\prod_{x\in A}\eta(x)=1_{\{\eta\equiv1\text{ on }A\}},
$$

with empty product one. Use the [stirring representation of symmetric exclusion](../../../../../../stirring-representation-of-symmetric-exclusion.md) on the time interval $[0,t]$. Trace the labels at the sites of $A$ backwards to time zero, and call their set of ancestors $B_t$. Labels remain distinct under swaps, so $|B_t|=|A|$. Pathwise,

$$
D(\eta_t,A)=D(\eta,B_t).
$$

Reverse time in the Poisson clocks. Their joint law is unchanged, and each interchange is its own inverse. Thus the backward set $B_t$ has the same law as the finite-particle symmetric exclusion set $A_t$ started from $A$. Taking [expectations](../../../../../../expected-value.md) gives the [product self-duality of symmetric exclusion](../../../../../../product-self-duality-of-symmetric-exclusion.md)

$$
\boxed{\mathbb P^\eta(\eta_t\equiv1\text{ on }A)=\mathbb P^A(\eta\equiv1\text{ on }A_t).}
$$

The argument holds for every deterministic initial configuration $\eta$ and every [finite set](../../../../../../finite-set.md) $A$, including the empty set, and makes no stationarity assumption.

The generator identity confirms the same mechanism. For any [edge](../../../../../../edge-of-a-graph.md) $xy$, let $A^{xy}$ interchange membership of $x,y$. Then

$$
D(\eta^{xy},A)=D(\eta,A^{xy}).
$$

Summing over [edges](../../../../../../edge-of-a-graph.md) gives $L_\eta D=L_A D$. In the finite-particle generator only [edges](../../../../../../edge-of-a-graph.md) joining an occupied to a vacant site contribute; in the occupation generator the same transpositions act on the other argument. Symmetry supplies the same rate in both operations.

To see why this qualification matters, suppose right jumps have rate $a$ and left jumps rate $b\ne a$. Take $A=\{0\}$ and an initial configuration whose only particle is at $1$. The derivative at zero of the left-hand [probability](../../../../../../probability.md) is $b$, since that particle must jump left into zero. The derivative of the right-hand [probability](../../../../../../probability.md) for the same asymmetric finite-particle process is $a$, since its particle must jump right from zero to the initially occupied site $1$. Thus the printed same-process identity would be false in that asymmetric interpretation. Under the symmetric convention established in the preceding part, the proof is complete.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
