<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**True.** An [irreducible ideal](../../../../../../irreducible-ideal.md) $I$ is a proper [ideal](../../../../../../ideal.md) such that $I=J\cap K$ forces $I=J$ or $I=K$. Passing to the [quotient ring](../../../../../../quotient-ring.md) $A=R/I$ turns this into the assertion that zero cannot be the intersection of two nonzero [ideals](../../../../../../ideal.md). Also $A$ is [Noetherian](../../../../../../noetherian-ring.md): ascending chains of [ideals](../../../../../../ideal.md) lift to ascending chains of [ideals](../../../../../../ideal.md) containing $I$ in $R$.

Suppose $ab=0$ in $A$, and suppose $b$ is not a [nilpotent element](../../../../../../nilpotent.md). The [ascending chain condition](../../../../../../ascending-chain-condition.md) makes the chain of [annihilators](../../../../../../annihilator-ring-theory.md)

$$
\operatorname{Ann}(b)\subseteq\operatorname{Ann}(b^2)\subseteq\cdots
$$

stabilize. Choose $n\geq1$ with $\operatorname{Ann}(b^n)=\operatorname{Ann}(b^{n+1})$. We claim

$$
(a)\cap(b^n)=0.
$$

If $z=ua=vb^n$ lies in this intersection, then $bz=uab=0$, so $vb^{n+1}=0$. The equality of [annihilators](../../../../../../annihilator-ring-theory.md) implies $vb^n=0$, hence $z=0$. Since $b$ is not nilpotent, $(b^n)\ne0$. Irreducibility of zero therefore forces $(a)=0$, or $a=0$.

We have proved that $ab=0$ and $a\ne0$ force $b$ to be a [nilpotent element](../../../../../../nilpotent.md). This says precisely that zero is a [primary ideal](../../../../../../primary-ideal.md) in $A$, and therefore that $I$ is a [primary ideal](../../../../../../primary-ideal.md) in $R$.

If its [radical of an ideal](../../../../../../radical-of-an-ideal.md) is to be denoted by a [prime ideal](../../../../../../prime-ideal.md), this requires no extra hypothesis: for any [primary ideal](../../../../../../primary-ideal.md) $I$, $uv\in\sqrt I$ and $u\notin\sqrt I$ imply $u^nv^n\in I$ with $u^n\notin I$, so some power of $v$ lies in $I$. Thus $v\in\sqrt I$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
