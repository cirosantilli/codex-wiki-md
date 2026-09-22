<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $Q=(A\to B)\to A$ and $P=Q\to A$. The displayed formula is $(P\to B)\to B$. A proof of [logical implication](../../../../../../logical-implication.md) may use its temporary assumption more than once; this is ordinary [natural deduction](../../../../../../natural-deduction.md), not a linear proof system.

Assume $h:P\to B$, then $f:Q$, then $a:A$, then $g:Q$. The [identity weakening rule](../../../../../../identity-weakening-rule.md) derives $a:A$ from the hypotheses $a:A$ and $g:Q$. Discharging $g$ by the [implication introduction rule](../../../../../../implication-introduction-rule.md) gives $\lambda g^Q.a:P$. Applying $h$ by the [implication elimination rule](../../../../../../implication-elimination-rule.md) gives $h(\lambda g^Q.a):B$. Discharge $a$ to obtain $\lambda a^A.h(\lambda g^Q.a):A\to B$. Applying $f$ gives an $A$; discharge $f$ to obtain a $P$; apply $h$ once more to obtain $B$, and finally discharge $h$.

Here is the complete decorated [natural deduction](../../../../../../natural-deduction.md) derivation, split at its intermediate $A\to B$ conclusion to keep the tree readable. Superscript labels mark which assumption occurrences are discharged; both occurrences labelled $1$ are discharged together.

$$
\frac{
 \frac{
  [h:P\to B]^1\qquad
  \frac{\frac{[a:A]^3\quad[g:Q]^4}{a:A}\;\mathrm{Id}}
  {\lambda g^Q.a:P}\;\to I_4
 }{h(\lambda g^Q.a):B}\;\to E
}{\lambda a^A.h(\lambda g^Q.a):A\to B}\;\to I_3
$$

To avoid an excessively wide final tree, continue the same derivation as follows, using the right-hand derived premise above:

$$
\frac{
 \frac{
  [f:Q]^2\qquad \lambda a^A.h(\lambda g^Q.a):A\to B
 }{f(\lambda a^A.h(\lambda g^Q.a)):A}\;\to E
}{\lambda f^Q.f(\lambda a^A.h(\lambda g^Q.a)):P}\;\to I_2
$$

followed by

$$
\frac{
 \frac{[h:P\to B]^1\quad\lambda f^Q.f(\lambda a^A.h(\lambda g^Q.a)):P}
 {h(\lambda f^Q.f(\lambda a^A.h(\lambda g^Q.a))):B}\;\to E
}{\lambda h^{P\to B}.h(\lambda f^Q.f(\lambda a^A.h(\lambda g^Q.a))):(P\to B)\to B}\;\to I_1.
$$

Thus the concise [lambda term](../../../../../../lambda-term.md), with bound-variable types determined by the displayed tree, is

$$
\boxed{\lambda h.\;h\bigl(\lambda f.\;f(\lambda a.\;h(\lambda g.\;a))\bigr).}
$$

Under the [Curry-Howard correspondence](../../../../../../curry-howard-correspondence.md), [implication introduction rules](../../../../../../implication-introduction-rule.md) correspond to [lambda abstractions](../../../../../../lambda-abstraction.md), [implication elimination rules](../../../../../../implication-elimination-rule.md) to applications, and the [identity weakening rule](../../../../../../identity-weakening-rule.md) retains the first term while allowing an unused second hypothesis. No other inference rule or classical axiom is required.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
