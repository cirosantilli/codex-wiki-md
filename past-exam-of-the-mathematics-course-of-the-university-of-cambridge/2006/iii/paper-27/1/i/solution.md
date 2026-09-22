<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Every nonzero [P-adic number](../../../../../../p-adic-number.md) has a unique decomposition $z=p^mu$ with $m\in\mathbb Z$ and $u\in\mathbb Z_p^\times$. The [group homomorphism kernel](../../../../../../kernel-of-a-group-homomorphism.md) of reduction from the [unit group](../../../../../../unit-group.md) onto $\mathbb F_p^\times$ is $1+p\mathbb Z_p$, the group of [principal units](../../../../../../principal-unit.md). Each nonzero residue class has a unique lift $\omega$ satisfying $\omega^{p-1}=1$, by the simple-root [Hensel lemma](../../../../../../hensel-s-lemma.md) proved in question 3. Uniqueness makes these lifts multiplicative. They form the [cyclic group](../../../../../../cyclic-group.md) $\mu_{p-1}$, and every unit has a unique factorization

$$
u=\omega\,v,\qquad\omega\in\mu_{p-1},\quad v\in1+p\mathbb Z_p.
$$

Thus $\mathbb Q_p^\times=p^{\mathbb Z}\times\mu_{p-1}\times(1+p\mathbb Z_p)$.

For odd $p$, the [p-adic logarithm](../../../../../../p-adic-logarithm.md) and [p-adic exponential function](../../../../../../p-adic-exponential-function.md) give inverse group isomorphisms $1+p\mathbb Z_p\leftrightarrow p\mathbb Z_p$. To verify the convergence domain, for $t\in p\mathbb Z_p$ the [p-adic logarithm](../../../../../../p-adic-logarithm.md) terms have valuations $nv_p(t)-v_p(n)\to\infty$, and the exponential terms have valuations $nv_p(t)-v_p(n!)\to\infty$, since $v_p(n!)\le(n-1)/(p-1)$ and $p>2$. In both series every term after the linear one has strictly larger [valuation](../../../../../../valuation.md) than the linear term. Consequently $\log(1+t)\in p\mathbb Z_p$ and $\exp(t)\in1+p\mathbb Z_p$. The formal identities $\log(vw)=\log v+\log w$ and $\exp(\log v)=v$, $\log(\exp t)=t$ hold on these convergent domains, as follows by multiplying the convergent series or passing to their formal identities termwise.

Choose a generator $\zeta$ of $\mu_{p-1}$. An explicit isomorphism is

$$
\boxed{\mathbb Z/(p-1)\mathbb Z\times\mathbb Z_p\times\mathbb Z\longrightarrow\mathbb Q_p^\times,\qquad(a,b,m)\longmapsto\zeta^a\exp(pb)p^m.}
$$

The inverse reads off the [valuation](../../../../../../valuation.md), the root-of-unity unit factor, and $p^{-1}\log(v)$. Both directions are continuous with the standard product topology, so this is also a [topological group](../../../../../../topological-group-split.md) isomorphism. The odd-prime condition is essential for using all of $1+p\mathbb Z_p$ as the [p-adic logarithm](../../../../../../p-adic-logarithm.md)-isomorphism domain.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
