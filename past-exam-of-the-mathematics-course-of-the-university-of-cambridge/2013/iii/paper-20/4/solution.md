<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In the [simply typed lambda calculus](../../../../../simply-typed-lambda-calculus.md), types are generated from atomic types by the arrow constructor $A\to B$. A [typed lambda term](../../../../../typed-lambda-term.md) is a [lambda term](../../../../../lambda-term.md) equipped with a derivation of a judgement $\Gamma\vdash t:A$, where the context assigns types to its free variables. The basic typing rules are

$$
\frac{x:A\in\Gamma}{\Gamma\vdash x:A},\qquad
\frac{\Gamma,x:A\vdash t:B}{\Gamma\vdash\lambda x.t:A\to B},\qquad
\frac{\Gamma\vdash f:A\to B\quad\Gamma\vdash u:A}{\Gamma\vdash fu:B}.
$$

The [Implicational Curry-Howard correspondence](../../../../../implicational-curry-howard-correspondence.md) reads atomic types as propositions and $A\to B$ as [logical implication](../../../../../logical-implication.md). A typed variable is an assumption, abstraction is the [implication introduction rule](../../../../../implication-introduction-rule.md) discharging that assumption, and application is the [implication elimination rule](../../../../../implication-elimination-rule.md). Consequently a [typed lambda term](../../../../../typed-lambda-term.md) is a proof in implicational [Intuitionistic propositional logic](../../../../../intuitionistic-propositional-logic.md), and a [natural deduction](../../../../../natural-deduction.md) proof recursively supplies such a term. For example, $\lambda x.x:A\to A$ expresses implication reflexivity. Products, sums, and the empty type extend the correspondence to conjunction, disjunction, and falsity; pure arrow types give precisely the implicational fragment. [Beta reduction](../../../../../beta-reduction.md) removes an introduction followed immediately by its elimination, matching proof simplification.

A **[Church numeral](../../../../../church-numeral.md)** is

$$
\boxed{\overline n=\lambda f.\lambda x.f^n x},\qquad
\overline0=\lambda f.\lambda x.x,
$$

where $f^n x$ means $n$ repetitions of application. At base type $A$, it has type $C_A=(A\to A)\to A\to A$. The following [Church numeral arithmetic](../../../../../church-numeral-arithmetic.md) terms use left-associated application:

$$
\begin{aligned}
\mathsf{Succ}&=\lambda n f x.f(nfx),\\
\mathsf{Add}&=\lambda m n f x.mf(nfx),\\
\mathsf{Mul}&=\lambda m n f x.m(nf)x,\\
\mathsf{Pow}&=\lambda m n f x.(nm)fx.
\end{aligned}
$$

Their concise conclusions are

$$
\boxed{\mathsf{Succ}\,\overline n\equiv_\beta\overline{n+1},\quad
\mathsf{Add}\,\overline m\,\overline n\equiv_\beta\overline{m+n},\quad
\mathsf{Mul}\,\overline m\,\overline n\equiv_\beta\overline{mn},\quad
\mathsf{Pow}\,\overline m\,\overline n\equiv_\beta\overline{m^n}.}
$$

For successor, the initial $f$ adds one application. For addition, the inner $nfx$ supplies $n$ applications and $mf$ supplies $m$ more. For multiplication, the repeated operation $nf$ applies $f$ $n$ times, and $m$ repetitions give $mn$. For exponentiation, $\overline n$ iterates the operation $\overline m$ on $f$: each iteration replaces a function $g$ by its $m$-fold iterate, yielding $f^{m^n}$. Zero iterations give $f$, so this encoding takes $m^0=1$, including $0^0=1$. The explicit outer $f,x$ abstractions make the result the standard [Church numeral](../../../../../church-numeral.md) even at exponent zero, without needing eta equivalence.

Successor, addition, and multiplication operate on the same $C_A$. The displayed exponentiation term has type $C_A\to C_{A\to A}\to C_A$: its exponent iterates an operation on functions. Thus the numeral syntax admits several type instances; one should not force every occurrence into one fixed monomorphic Church type.

The **[Y combinator](../../../../../fixed-point-combinator.md)** is the [fixed-point combinator](../../../../../fixed-point-combinator.md)

$$
\boxed{Y=\lambda g.(\lambda x.g(xx))(\lambda x.g(xx)).}
$$

For $X_g=(\lambda x.g(xx))(\lambda x.g(xx))$, [beta reduction](../../../../../beta-reduction.md) gives $Yg\to_\beta X_g\to_\beta gX_g$. Since $X_g\equiv_\beta Yg$, we obtain $Yg\equiv_\beta g(Yg)$. This allows a recursive program body to receive a representation of itself.

Here the computation is in the [untyped lambda calculus](../../../../../untyped-lambda-calculus.md). The self-application $xx$ would require a simple type satisfying $A=A\to B$, impossible for finite simple types. Accordingly $Y$ is not a [typed lambda term](../../../../../typed-lambda-term.md) of the simply typed system. The [Strong normalization theorem for simply typed lambda calculus](../../../../../strong-normalization-theorem-for-simply-typed-lambda-calculus.md) also rules out a universal divergent fixed-point operator there.

To obtain a [lambda representation of partial computable functions](../../../../../lambda-representation-of-partial-computable-functions.md), encode machine configurations as finite data using [Church numerals](../../../../../church-numeral.md), [Church pairs](../../../../../church-pair.md), and [Church Booleans](../../../../../church-boolean.md). Initial configuration, one transition, the halting test, and output extraction are [primitive recursive functions](../../../../../primitive-recursive-function.md), represented by [lambda terms](../../../../../lambda-term.md) through the initial functions, composition, and [lambda definition of primitive recursion by pair iteration](../../../../../lambda-definition-of-primitive-recursion-by-pair-iteration.md). If these representations are $\mathsf{Init}$, $\mathsf{Next}$, $\mathsf{Halt}$, and $\mathsf{Out}$, define

$$
\mathsf{Run}=Y(\lambda r c.\mathsf{Halt}\,c\,(\mathsf{Out}\,c)\,(r(\mathsf{Next}\,c))),\qquad
\mathsf{Compute}=\lambda n.\mathsf{Run}(\mathsf{Init}\,n).
$$

Use [normal-order beta reduction](../../../../../normal-order-beta-reduction.md) so the [Church Boolean](../../../../../church-boolean.md) halting test selects one branch without evaluating the unused recursive branch. A halting computation follows finitely many transitions and returns the [Church numeral](../../../../../church-numeral.md) of the output. A nonhalting computation forces successive tests forever and has no [head normal form](../../../../../head-normal-form.md); by [normal-order normalization theorem](../../../../../normal-order-normalization-theorem.md), it cannot be [beta equivalent](../../../../../beta-equivalence.md) to a [Church numeral](../../../../../church-numeral.md). Thus **every [partial computable function](../../../../../computable-function.md) is represented**, with divergence preserved; every [total computable function](../../../../../total-computable-function.md) is the halting special case. This explains the role of $Y$ in computational universality while keeping the typed proof interpretation precise.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
