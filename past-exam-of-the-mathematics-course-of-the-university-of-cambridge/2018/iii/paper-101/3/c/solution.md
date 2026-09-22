<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**True, without a Noetherian hypothesis.** By definition, the [symbolic power](../../../../../../symbolic-power.md) is the [contraction of an ideal](../../../../../../contraction-of-an-ideal.md)

$$
P^{(n)}=P^nR_P\cap R,
$$

where the intersection notation means inverse image under $R\to R_P$, even if this map is not [injective](../../../../../../injective-function.md). In the [local ring](../../../../../../local-ring.md) $A=R_P$, put $\mathfrak m=PR_P$. Then $P^nR_P=\mathfrak m^n$, and $\sqrt{\mathfrak m^n}=\mathfrak m$: every element of $\mathfrak m$ has its $n$th power in $\mathfrak m^n$, whereas a [unit](../../../../../../unit-in-a-ring.md) cannot have a power in this proper [ideal](../../../../../../ideal.md).

The [ideal](../../../../../../ideal.md) $\mathfrak m^n$ is $\mathfrak m$-primary. Indeed, if $uv\in\mathfrak m^n$ and $v\notin\mathfrak m$, then $v$ is a [unit](../../../../../../unit-in-a-ring.md), so $u\in\mathfrak m^n$. Its [contraction of an ideal](../../../../../../contraction-of-an-ideal.md) is therefore $P$-primary: its [radical of an ideal](../../../../../../radical-of-an-ideal.md) contracts to $P$, and the same implication applies to the images of any two elements of $R$. Thus $P^{(n)}$ is always $P$-primary, proving the reverse implication immediately when $P^n=P^{(n)}$.

For the other implication, suppose $P^n$ is $P$-primary. Membership in the contraction can be expressed by clearing denominators:

$$
r\in P^{(n)}\quad\Longleftrightarrow\quad
sr\in P^n\text{ for some }s\notin P.
$$

For completeness, if $r/1=a/t$ with $a\in P^n$ and $t\notin P$, equality of fractions gives $u(tr-a)=0$ for some $u\notin P$, so $(ut)r=ua\in P^n$; the converse follows by inverting $s$. Since $s\notin\sqrt{P^n}=P$, the [primary ideal](../../../../../../primary-ideal.md) property forces $r\in P^n$. The inclusion $P^n\subseteq P^{(n)}$ always holds, giving

$$
\boxed{P^n\text{ is }P\text{-primary}\iff P^n=P^{(n)}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
