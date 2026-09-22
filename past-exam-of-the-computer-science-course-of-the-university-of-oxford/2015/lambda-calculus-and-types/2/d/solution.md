<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The exact restriction in the ordinary [simply typed lambda calculus](../../../../../simply-typed-lambda-calculus.md) is

$$
\boxed{\varnothing\mapsto\lambda xy.(\lambda z.x)(yx):A\Rightarrow(B\Rightarrow A)
\quad\Longleftrightarrow\quad
B=A\Rightarrow C\text{ for some simple type }C.}
$$

Thus the unrestricted choice of $A,B$ available in part (c) fails. A reading of the printed sentence as asserting impossibility for every choice of $A,B$ is false. This issue occurs in the original PDF as well as its transcription.[p. 2, Question 2(d)](../../../../../lambda-calculus-and-types-examination-paper-of-the-university-of-oxford-2015.md)

To prove necessity, first observe why the ordinary rules cannot hide assumptions. [Structural induction](../../../../../structural-induction.md) on a derivation proves

$$
\operatorname{Subjects}(\Gamma)=FV(t)
\quad\text{whenever }\Gamma\mapsto t:T.
$$

For a variable, both sides are the singleton containing that variable. For [lambda application](../../../../../lambda-application.md), both sides are the [union](../../../../../set-union.md) of the two premise supports. For [lambda abstraction](../../../../../lambda-abstraction.md), both sides delete the bound variable. There is no [universal typing axiom](../../../../../universal-typing-axiom.md) to interrupt this equality.

Now invert the proposed derivation. Each outer [lambda abstraction](../../../../../lambda-abstraction.md) must have been introduced by the abstraction rule, since the other ordinary rules conclude a variable or a [lambda application](../../../../../lambda-application.md). The body must therefore have the [typing judgment](../../../../../typing-judgment.md)

$$
\{x:A,y:B\}\mapsto(\lambda z.x)(yx):A.
$$

The support equality just proved ensures that both displayed assumptions occur; consistency fixes their [simple types](../../../../../simple-type.md) to those specified by the outer [function type](../../../../../function-type.md). Inverting the [lambda application](../../../../../lambda-application.md) gives a [simple type](../../../../../simple-type.md) $C$ for its argument and the following premises:

$$
\{x:A\}\mapsto\lambda z.x:C\Rightarrow A,
\qquad
\{x:A,y:B\}\mapsto yx:C.
$$

There is no flexibility in the supports: $\lambda z.x$ has the single [free variable](../../../../../free-variable.md) $x$, whereas $yx$ has both [free variables](../../../../../free-variable.md) $y,x$. Invert the second [lambda application](../../../../../lambda-application.md). Its two premises must be

$$
\{y:B\}\mapsto y:D\Rightarrow C,
\qquad
\{x:A\}\mapsto x:D
$$

for some [simple type](../../../../../simple-type.md) $D$. The variable rule is the only possible final rule for each premise. It forces $D=A$ and $B=D\Rightarrow C$, yielding $B=A\Rightarrow C$.

Conversely, suppose $B=A\Rightarrow C$. The ordinary rules give

$$
\frac{\{y:A\Rightarrow C\}\mapsto y:A\Rightarrow C
\qquad\{x:A\}\mapsto x:A}
{\{x:A,y:A\Rightarrow C\}\mapsto yx:C},
\qquad
\frac{\{x:A\}\mapsto x:A}
{\{x:A\}\mapsto\lambda z.x:C\Rightarrow A}.
$$

The [typing contexts](../../../../../typing-context.md) are consistent, so another [lambda application](../../../../../lambda-application.md) gives the body type $A$. Two [lambda abstractions](../../../../../lambda-abstraction.md) discharge $y$ and $x$, establishing

$$
\varnothing\mapsto\lambda xy.(\lambda z.x)(yx):
A\Rightarrow((A\Rightarrow C)\Rightarrow A).
$$

This proves sufficiency and supplies a family of counterexamples to the literal impossibility claim. For a concrete failure of the unrestricted claim, choose $A=\alpha$ and $B=\beta$ as atomic [type variables](../../../../../type-variable.md). The [type variable](../../../../../type-variable.md) $\beta$ is not a [function type](../../../../../function-type.md) $\alpha\Rightarrow C$, so no derivation exists for that fixed pair. Here the atomic [type variables](../../../../../type-variable.md) are fixed type expressions, rather than unknowns that one may change during [type inference](../../../../../type-inference.md).

The reason for the restriction is the otherwise discarded [lambda application](../../../../../lambda-application.md) $yx$: the ordinary rules still type-check it. Its subsequent disappearance under [beta reduction](../../../../../beta-reduction.md) does not license reversing that [beta reduction](../../../../../beta-reduction.md) while preserving every [simple type](../../../../../simple-type.md) of the result. The [beta-normal form](../../../../../beta-normal-form.md) $\lambda xy.x$ admits arbitrary $A\Rightarrow(B\Rightarrow A)$, whereas the unreduced [lambda term](../../../../../lambda-term.md) has the additional constraint just derived.

$$
\boxed{\text{The all-}A,B\text{ claim fails; the valid instances have }B=A\Rightarrow C.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Lambda calculus and types](../../../lambda-calculus-and-types-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
