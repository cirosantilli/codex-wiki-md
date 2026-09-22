<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose mutually inverse maps $i:D^D\to D$ and $j:D\to D^D$. This is an [extensional reflexive object](../../../../../../extensional-reflexive-object.md) in the [Cartesian closed category](../../../../../../cartesian-closed-category.md). Define its application morphism

$$
\operatorname{app}=\operatorname{ev}\circ(j\times\operatorname{id}_D):D\times D\to D.
$$

For [endomorphisms](../../../../../../endomorphism.md) $f,g:D\to D$, application in the underlying set $\operatorname{End}(D)$ is $f\cdot g=\operatorname{app}\circ\langle f,g\rangle$.

It is useful to define term interpretation uniformly over any context object $A$. An environment assigns each free variable $x$ a morphism $\rho(x):A\to D$. Variables are interpreted by their assigned maps, and application is interpreted by $\operatorname{app}$ and pairing. For [lambda abstraction](../../../../../../lambda-abstraction.md), lift the old environment along $\pi_A:A\times D\to A$, interpret the new variable by $\pi_D$, and let $h:A\times D\to D$ interpret the body. Then set

$$
\operatorname{interp}_\rho(\lambda x.M)=i\circ\Lambda h:A\to D.
$$

Taking $A=D$ gives interpretations in the requested set of [endomorphisms](../../../../../../endomorphism.md). Other context objects are needed in the recursive definition to handle bound variables correctly.

The [beta reduction](../../../../../../beta-reduction.md) rule follows from $ji=\operatorname{id}_{D^D}$ and the evaluation identity for [currying](../../../../../../currying.md). Applying the interpreted abstraction to a map $g:A\to D$ gives

$$
\operatorname{ev}\circ\langle\Lambda h,g\rangle=h\circ\langle\operatorname{id}_A,g\rangle.
$$

Induction on terms identifies this with interpretation of the [capture-avoiding substitution](../../../../../../capture-avoiding-substitution.md) of the argument for $x$.

For [eta conversion](../../../../../../eta-conversion.md), suppose $x$ is not free in $M$ and write $f:A\to D$ for the interpretation of $M$. The body $Mx$ on $A\times D$ is the uncurried form of $jf$. Hence

$$
\operatorname{interp}(\lambda x.Mx)=i\Lambda(\operatorname{uncurry}(jf))=ijf=f.
$$

Thus **beta-eta-equivalent terms have equal interpretations in $\operatorname{End}(D)$**. The full isomorphism, rather than just a retract of the function object, provides the inverse law used in the eta step.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
