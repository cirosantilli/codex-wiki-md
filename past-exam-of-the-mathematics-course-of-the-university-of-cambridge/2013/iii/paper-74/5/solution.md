<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For each object $X$, characteristic maps identify $\mathcal E(X,\Omega)$ with $\operatorname{Sub}(X)$. These [subobject](../../../../../subobject.md) posets carry a natural [Heyting algebra](../../../../../heyting-algebra.md) structure. Truth and falsity classify $X$ and the empty [subobject](../../../../../subobject.md). Intersections define $\wedge$, unions define $\vee$, and implication is characterized by

$$
R\leq(P\Rightarrow Q)\quad\Longleftrightarrow\quad R\cap P\leq Q.
$$

These operations commute with [pullback](../../../../../pullback-category-theory.md), giving arrows on $\Omega$ and the [internal Heyting algebra of truth values](../../../../../internal-heyting-algebra-of-truth-values.md). Concretely, the order relation on $\Omega$ is the [subobject](../../../../../subobject.md) where $p\wedge q=p$; its characteristic map is implication. Negation is $p\Rightarrow\bot$.

If $U\hookrightarrow1$ has truth value $u:1\to\Omega$, its [quasi-closed local operator](../../../../../quasi-closed-local-operator.md) is

$$
\boxed{q(U)(p)=((p\Rightarrow u)\Rightarrow u).}
$$

This is double negation relative to the bottom value $u$. In the [Heyting algebra](../../../../../heyting-algebra.md) interval $[u,1]$, relative implication is inherited and relative negation is $N_u(p)=p\Rightarrow u$. Also $N_u(p)=N_u(p\vee u)$. Therefore the displayed map is the composite of adjoining $u$ and relative double negation. It is inflationary, idempotent, fixes truth and preserves binary meets, so it is a [Lawvere-Tierney topology](../../../../../lawvere-tierney-topology.md). Its value at bottom is $u$.

The truth values of its sheaf [topos](../../../../../elementary-topos.md) are the fixed elements $p=q(U)(p)$. They have bottom $u$, inherited meet and join $q(U)(p\vee r)$. Their relative negation is $N_u(p)$, which is again fixed because $N_u^3=N_u$. The relative double-negation law holds on every fixed element, and

$$
p\wedge N_u(p)=u,\qquad q(U)(p\vee N_u(p))=1.
$$

Thus every [subobject](../../../../../subobject.md) in the sheaf [topos](../../../../../elementary-topos.md) has a complement: **every quasi-closed subtopos is Boolean**. This identifies its internal logic, not merely the global truth-value lattice.

Now work in $\mathcal E/\Omega$. The arrow $\top:1\hookrightarrow\Omega$ is a subterminal object there; internally it supplies a freely varying generic truth value $u$. Let $a_q$ be [sheafification for a local operator](../../../../../sheaf-reflector-for-a-local-operator.md) for its quasi-closed topology, and let $\pi:\mathcal E/\Omega\to\mathcal E$ be the slice geometric morphism. The composite $h$ has inverse image $h^*=a_q\pi^*$.

To prove surjectivity, take any mono $S\hookrightarrow X$ in $\mathcal E$, classified by $p:X\to\Omega$. Its [pullback](../../../../../pullback-category-theory.md) along $\pi$ has predicate $p(x)$, independent of the generic $u$. If $h^*$ sends the mono to an isomorphism, it is $q$-dense in the slice, so

$$
((p(x)\Rightarrow u)\Rightarrow u)=1
$$

for all $(x,u)$. Pull back this identity along the graph $x\mapsto(x,p(x))$. Substituting $u=p(x)$ gives $q_{p(x)}(p(x))=p(x)$, and therefore $p(x)=1$. Thus the original mono was already invertible.

For parallel arrows $r,s:X\rightrightarrows Y$, equality of their inverse images makes the inverse image of their [equalizer](../../../../../equaliser.md) invertible. The preceding mono argument makes the [equalizer](../../../../../equaliser.md) invertible and hence $r=s$. Therefore **$h^*$ is faithful**, and the composite is a [surjective geometric morphism](../../../../../surjective-geometric-morphism.md). A fixed double-negation subtopos can erase information; allowing the generic relative bottom is what detects every original predicate.

For the completeness consequence, let $\mathbb T$ be coherent and use its [classifying topos](../../../../../classifying-topos.md) with the generic model. Its conservative syntactic interpretation makes an underivable [coherent sequent](../../../../../coherent-sequent.md) fail as a [subobject](../../../../../subobject.md) inclusion. Pulling this model into the Boolean cover constructed above preserves coherent formulas and still refutes that inclusion, because the inverse image is faithful and reflects containment. In the [Boolean topos](../../../../../boolean-topos.md), the difference between antecedent and consequent is a nonzero complemented [subobject](../../../../../subobject.md). Slicing over that difference gives a nondegenerate [Boolean topos](../../../../../boolean-topos.md) with a global tuple satisfying the antecedent and the negation of the consequent.

Classical first-order deduction is sound in a [Boolean topos](../../../../../boolean-topos.md). Hence $\mathbb T$ together with constants for that tuple, the antecedent and the negated consequent is classically consistent: a proof of contradiction would hold in the nondegenerate sliced model. The ordinary [Henkin construction](../../../../../henkin-construction.md) supplies a set model of this consistent theory. Briefly, extend it by witness constants, complete it to a maximal consistent theory, form the term structure modulo provable equality, and prove the truth lemma by induction on formulas. For possibly empty sorts use the standard encoding by sort predicates and functional graph relations, without asserting sort inhabitance; the constants for the chosen tuple assert only the needed witnesses. The resulting set model is a countermodel to the original sequent.

Consequently **a [coherent sequent](../../../../../coherent-sequent.md) valid in every set-valued model of a coherent theory is derivable in coherent logic**. The Boolean cover supplies the crucial passage from the generic intuitionistic countermodel to consistency with classical negation; the final set-model step uses ordinary first-order completeness via its Henkin proof, rather than an assumption that every [Boolean topos](../../../../../boolean-topos.md) has points.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
