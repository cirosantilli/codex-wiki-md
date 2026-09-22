<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $s=\sqrt{-5}$ and $P=(2,1+s)$. The [polynomial](../../../../../polynomial-split.md) $x^2+5$ reduces to $(x+1)^2$ modulo $2$, so the [Kummer-Dedekind theorem](../../../../../kummer-dedekind-theorem.md) gives

$$
\boxed{(2)=P^2,\qquad N(P)=2.}
$$

If $P=(a+bs)$, its [norm](../../../../../norm.md) would imply $a^2+5b^2=2$, impossible for integers $a,b$. Thus $P$ represents the nontrivial [ideal class](../../../../../ideal-class.md). Since the [class number](../../../../../class-number.md) is $2$, every nonprincipal [integral ideal](../../../../../integral-ideal.md) $I$ has $[I]=[P]$, and $[IP]=1$. Write $IP=(\gamma)$ with $\gamma\in\mathcal O_M$; integrality follows from $IP\subseteq\mathcal O_M$. Multiplying by $P$ gives

$$
(2)I=(\gamma)P.
$$

Norms give $4N(I)=2N(\gamma)$, hence $N(\gamma)=2N(I)$. If $N(I)=p_3\equiv1\pmod{20}$, writing $\gamma=a+bs$ yields

$$
a^2+5b^2=2p_3\equiv2\pmod5,
$$

contradicting the list $0,1,4$ of squares modulo $5$. Therefore **no nonprincipal [ideal](../../../../../ideal.md) has [norm](../../../../../norm.md) $p_3$**.

As $p_3\equiv1\pmod4$ and $p_3\equiv1\pmod5$, [quadratic reciprocity](../../../../../quadratic-reciprocity.md) gives $(-5/p_3)=1$. Thus $x^2+5$ has two distinct roots modulo $p_3$ and

$$
(p_3)=RR',\qquad N(R)=N(R')=p_3.
$$

The [norm](../../../../../norm.md) obstruction shows that $R$ must be principal, say $R=(x+ys)$. Taking its [norm](../../../../../norm.md) proves

$$
\boxed{p_3=x^2+5y^2.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the number theory course of the University of Oxford](../../../../split.md)
6. [Number theory course of the University of Oxford](../../../../../number-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
