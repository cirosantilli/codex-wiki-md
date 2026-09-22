<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the unit $\eta$ just constructed and replace it by the inclusion $A=S^{r-1}\hookrightarrow Y=\operatorname{Cyl}(\eta)$ into its [mapping cylinder](../../../../../../mapping-cylinder.md); $Y\simeq\Omega S^r$. Put $m=2r-3$. The [homology](../../../../../../homology-split.md) isomorphisms from question 4(ii) and the relative [exact sequence](../../../../../../exact-sequence.md) give $H_j(Y,A;\mathbb Z)=0$ for $j\leq m$.

Both $A$ and $Y$ are simply connected for $r\geq3$. For the degree-two start, the absolute [Hurewicz theorem](../../../../../../hurewicz-theorem.md) identifies their $\pi_2$ with $H_2$; naturality and the [homology](../../../../../../homology-split.md) isomorphism show $\eta_*$ is an isomorphism on $\pi_2$, so $\pi_2(Y,A)=0$. The relative [fundamental group](../../../../../../fundamental-group.md) also vanishes. If there were a first nonzero [relative homotopy group](../../../../../../relative-homotopy-group.md) in some degree $3\leq k\leq m$, the [Relative Hurewicz theorem](../../../../../../relative-hurewicz-theorem.md) for a $(k-1)$-connected simply connected pair would identify it with $H_k(Y,A)$, which is zero. Induction therefore gives $\pi_j(Y,A)=0$ for all $j\leq m$.

The relative [homotopy](../../../../../../homotopy.md) sequence now makes $\eta_*:\pi_i(S^{r-1})\to\pi_i(\Omega S^r)$ an isomorphism when $i+1\leq m$, and a surjection at $i=m$. Under loop-suspension adjunction, the adjoint of $\eta\circ a$ is $\Sigma a$, so this particular isomorphism is the [suspension](../../../../../../suspension-topology.md) homomorphism. Consequently the requested [Freudenthal suspension theorem](../../../../../../freudenthal-suspension-theorem.md) is

$$
\boxed{\pi_i(S^{r-1})\xrightarrow{\ \Sigma\ }\pi_{i+1}(S^r)\text{ is an isomorphism for }r\geq3,\ i\leq2r-4.}
$$

For $i=0$ this is read as the identification of connected-component sets; all degree-one groups here also vanish. The proof is the [homology comparison proof of Freudenthal suspension](../../../../../../homology-comparison-proof-of-freudenthal-suspension.md).

To compute the specified unstable groups, $S^1$ has contractible [universal cover](../../../../../../universal-cover.md), so $\pi_2(S^1)=0$. The [Hopf fibration](../../../../../../hopf-fibration.md) $S^1\to S^3\to S^2$ has exact segment $0=\pi_3S^1\to\pi_3S^3\to\pi_3S^2\to\pi_2S^1=0$, giving $\pi_3S^2=\mathbb Z$. The supplied starting value is $\pi_4S^3=\mathbb Z/2$. To pass from the group over $S^{n-1}$ to that over $S^n$, use $r=n,i=n$; the condition $n\leq2n-4$ holds exactly when $n\geq4$. Thus every later step is an isomorphism, and

$$
\boxed{\pi_{n+1}(S^n)=\begin{cases}0,&n=1,\\\mathbb Z,&n=2,\\\mathbb Z/2,&n\geq3.\end{cases}}
$$

This is the [first homotopy group above the dimension of a sphere](../../../../../../first-homotopy-group-above-the-dimension-of-a-sphere.md). The stable range deliberately excludes the step from $n=2$ to $n=3$, so the different groups there do not conflict with the theorem.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
