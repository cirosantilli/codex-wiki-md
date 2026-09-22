<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the embedding characterization of a [supercompact cardinal](../../../../../supercompact-cardinal.md): for every cardinal $\mu\geq\kappa$ there is an [elementary embedding](../../../../../elementary-embedding.md) $j:V\to M$ into a [transitive class](../../../../../transitive-class.md) with critical point $\kappa$, $j(\kappa)>\mu$ and $M^\mu\subseteq M$. In the [Lévy hierarchy](../../../../../levy-hierarchy.md), a $\Sigma_2$ sentence can be put into the form $\exists x\,\forall y\,\theta(x,y)$ with bounded matrix $\theta$. The same argument allows parameters $p\in V_\kappa$, which the embedding fixes.

Suppose $V\models\exists x\,\forall y\,\theta(x,y,p)$ and choose a witness $a$. Pick an [ordinal](../../../../../ordinal.md) $\lambda$ with $a,p\in V_\lambda$, and a cardinal $\mu\geq\kappa$ large enough that $\mu\geq|V_\lambda|$ and $\mu>\lambda$. Take the corresponding supercompact embedding. Its closure implies $V_\lambda\subseteq M$: induct on rank, enumerate each set in this rank segment by at most $\mu$ elements already in $M$, and use $M^\mu\subseteq M$ followed by taking the range. Thus $a\in M$ and $\operatorname{rank}(a)<j(\kappa)$.

Bounded formulas are absolute between [transitive classes](../../../../../transitive-class.md). Since $\forall y\,\theta(a,y,p)$ holds in $V$, it holds in $M$ and then in the transitive rank segment $V_{j(\kappa)}^M$. This segment contains $a,p$, so

$$
M\models V_{j(\kappa)}\models\exists x\,\forall y\,\theta(x,y,p).
$$

Apply elementarity to the first-order assertion that this sentence holds in the indicated [cumulative hierarchy](../../../../../cumulative-hierarchy.md) level, and use $j(p)=p$. We obtain the [supercompact Sigma-two downward reflection](../../../../../supercompact-sigma-two-downward-reflection.md) conclusion

$$
\boxed{V\models\sigma(p)\Longrightarrow V_\kappa\models\sigma(p)\qquad(\sigma\in\Sigma_2,\ p\in V_\kappa).}
$$

The closure requirement is used to put the original witness into the target; elementarity alone would not do that.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
