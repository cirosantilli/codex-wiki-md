<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [monomorphism](../../../../../../monomorphism.md) $m:A\to B$ satisfies $mu=mv\Rightarrow u=v$, and an [epimorphism](../../../../../../epimorphism.md) $e:A\to B$ satisfies $ue=ve\Rightarrow u=v$. A [strong monomorphism](../../../../../../strong-monomorphism.md) is a [monomorphism](../../../../../../monomorphism.md) with the right lifting property against all [epimorphisms](../../../../../../epimorphism.md): every square $mu=ve$ has a diagonal $d$ satisfying $de=u$ and $md=v$. The diagonal is unique by monicity. A [regular monomorphism](../../../../../../regular-monomorphism.md) is an [equalizer](../../../../../../equaliser.md) of some pair $h,k:B\rightrightarrows Z$. It is monic because two [equalizer](../../../../../../equaliser.md) factorizations of the same arrow must agree.

The converted TeX omits the remainder of this subpart. For the printed [strict monomorphism](../../../../../../strict-monomorphism.md) condition, an arrow $g:C\to B$ is admissible when, for every pair $h,k$ out of $B$, the implication $hm=km\Rightarrow hg=kg$ holds; strictness says each such $g$ factors uniquely through $m$. If $m$ equalizes $h_0,k_0$, every admissible $g$ satisfies $h_0g=k_0g$, and the [equalizer](../../../../../../equaliser.md) property supplies its unique factorization. Hence every regular [monomorphism](../../../../../../monomorphism.md) is strict.

Strictness itself implies monicity: whenever $mu=mv$, the common composite is admissible, so uniqueness of its factor through $m$ gives $u=v$. Now take a square $mu=ve$ with $e$ epic. Whenever $hm=km$, we have $hve=hmu=kmu=kve$, hence $hv=kv$. Thus $v$ is admissible and has a unique factor $d$ through $m$. Monicity gives $de=u$. We have proved the chain

$$
\boxed{\text{regular monomorphism}\ \Longrightarrow\ \text{strict monomorphism}\ \Longrightarrow\ \text{strong monomorphism}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
