# Lambda calculus and types

↑ **Parent:** [2015](../2015.md)

Solutions to all twelve numbered subparts of the [University of Oxford](../../university-of-oxford.md) [computer science](../../computer-science.md) Finals paper held on 4 June 2015. Question 2(d) has a wording issue: its literal impossibility claim is false, and the solution gives the exact condition for a valid [typing judgment](../../programming-language.md#typing-judgment).[Cover, p. 1; Questions 1–2, p. 2; Question 3, p. 3](../../computer-science-bibliography.md#lambda-calculus-and-types-examination-paper-of-the-university-of-oxford-2015)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Lambda calculus and types](lambda-calculus-and-types.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Choose all auxiliary bound variables fresh for the [free variables](../../mathematical-logic.md#free-variable) of $p,q,r$; [alpha equivalence](../../computability-theory.md#alpha-equivalence) permits this. The operation $\bullet$ is [composition of lambda terms](../../computability-theory.md#composition-of-lambda-terms), so expand its definition and use [beta reduction](../../computability-theory.md#beta-reduction):

$$
\begin{aligned}
(p\bullet q)\bullet r
&\equiv\lambda x.(\lambda y.p(qy))(rx)
\longrightarrow_\beta\lambda x.p(q(rx)),\\
p\bullet(q\bullet r)
&\equiv\lambda x.p((\lambda y.q(ry))x)
\longrightarrow_\beta\lambda x.p(q(rx)).
\end{aligned}
$$

The two [lambda terms](../../computability-theory.md#lambda-term) have the same reduct, up to [alpha equivalence](../../computability-theory.md#alpha-equivalence), hence they are related by [beta equivalence](../../computability-theory.md#beta-equivalence):

$$
\boxed{(p\bullet q)\bullet r=_\beta p\bullet(q\bullet r).}
$$

No [eta conversion](../../computability-theory.md#eta-conversion) is needed for this associativity calculation.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $I\equiv\lambda u.u$ for the [I combinator](../../computability-theory.md#i-combinator), and choose $x$ outside the [free variables](../../mathematical-logic.md#free-variable) of $p$. Both orders of [composition of lambda terms](../../computability-theory.md#composition-of-lambda-terms) first give the same [lambda abstraction](../../computability-theory.md#lambda-abstraction) by [beta reduction](../../computability-theory.md#beta-reduction):

$$
\begin{aligned}
p\bullet I&\equiv\lambda x.p((\lambda u.u)x)
\longrightarrow_\beta\lambda x.px,\\
I\bullet p&\equiv\lambda x.(\lambda u.u)(px)
\longrightarrow_\beta\lambda x.px.
\end{aligned}
$$

The freshness condition is exactly the side condition for [eta conversion](../../computability-theory.md#eta-conversion), which contracts $\lambda x.px$ to $p$. Therefore

$$
\boxed{p\bullet I=_{\beta\eta}p=_{\beta\eta}I\bullet p.}
$$

Here [eta conversion](../../computability-theory.md#eta-conversion) matters: a [free variable](../../mathematical-logic.md#free-variable) $p$ is already in [beta-normal form](../../computability-theory.md#beta-normal-form), as is $\lambda x.px$, and [beta equivalence](../../computability-theory.md#beta-equivalence) alone does not equate them.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The argument order in $p$ is a [cyclic permutation](../../combinatorics.md#cyclic-permutation). Undo it by rotating in the other direction. For $n\geq1$, choose the [lambda term](../../computability-theory.md#lambda-term)

$$
\boxed{q\equiv\lambda z y_1\cdots y_n.\,z\,y_n\,y_1\cdots y_{n-1}.}
$$

Use fresh bound variables throughout. Substituting $qz$ for the first argument of $p$ and then performing [beta reduction](../../computability-theory.md#beta-reduction) gives

$$
\begin{aligned}
(p\bullet q)z
&\longrightarrow_\beta^*p(qz)\\
&\longrightarrow_\beta^*\lambda x_1\cdots x_n.\,(qz)x_2\cdots x_nx_1\\
&\longrightarrow_\beta^*\lambda x_1\cdots x_n.\,zx_1\cdots x_n.
\end{aligned}
$$

Indeed, the arguments received by $qz$ are $y_1=x_2,\ldots,y_{n-1}=x_n,y_n=x_1$, so its last argument moves back to the front. Apply [eta conversion](../../computability-theory.md#eta-conversion) successively, starting with the innermost [lambda abstraction](../../computability-theory.md#lambda-abstraction). At each step the bound variable being removed is absent from the preceding expression. Thus the last expression is related to $z$ by [beta-eta equivalence](../../computability-theory.md#beta-eta-equivalence), and consequently

$$
\boxed{p\bullet q=_{\beta\eta}\lambda z.z=I.}
$$

For the induction needed in the next part, also compute the reverse [composition of lambda terms](../../computability-theory.md#composition-of-lambda-terms):

$$
\begin{aligned}
(q\bullet p)z
&\longrightarrow_\beta^*\lambda y_1\cdots y_n.\,(pz)y_ny_1\cdots y_{n-1}\\
&\longrightarrow_\beta^*\lambda y_1\cdots y_n.\,zy_1\cdots y_n
=_\eta z.
\end{aligned}
$$

So this $q$ is a two-sided inverse. The empty argument list at $n=0$ means $p=\lambda z.z$; choose $q=I$. For $n=1$, both displayed rotations give $\lambda zy_1.zy_1$, which is also related to $I$ by [eta conversion](../../computability-theory.md#eta-conversion). These boundary cases require no exceptional inverse construction.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Use [structural induction](../../foundations-of-mathematics.md#structural-induction) on the construction of $p\in\mathcal R$, with the stronger induction claim that $p$ is an [invertible lambda term](../../computability-theory.md#invertible-lambda-term): there is a [lambda term](../../computability-theory.md#lambda-term) $q$ satisfying both

$$
p\bullet q=_{\beta\eta}I,
\qquad q\bullet p=_{\beta\eta}I.
$$

The base constructor has exactly the two-sided inverse proved in part (c). Strengthening the claim is useful because the inductive construction needs inverses of its constituent [lambda terms](../../computability-theory.md#lambda-term) in both orders.

For the inductive constructor, let $t_i$ be the two-sided inverse supplied for $s_i$. Thus, for a fresh variable $u$, [beta-eta equivalence](../../computability-theory.md#beta-eta-equivalence) gives

$$
s_i(t_i u)=_{\beta\eta}u,
\qquad t_i(s_i u)=_{\beta\eta}u
\qquad(1\leq i\leq n).
$$

For $n\geq1$, define

$$
\boxed{q\equiv\lambda z y_1\cdots y_n.\,
z(t_1y_n)(t_2y_1)\cdots(t_ny_{n-1}).}
$$

This [lambda term](../../computability-theory.md#lambda-term) reverses the [cyclic permutation](../../combinatorics.md#cyclic-permutation) and applies the appropriate inverse to each argument. First use [beta reduction](../../computability-theory.md#beta-reduction) to expand one order of [composition of lambda terms](../../computability-theory.md#composition-of-lambda-terms):

$$
\begin{aligned}
(p\bullet q)z
&\longrightarrow_\beta^*\lambda x_1\cdots x_n.\,
(qz)(s_2x_2)\cdots(s_nx_n)(s_1x_1)\\
&\longrightarrow_\beta^*\lambda x_1\cdots x_n.\,
z(t_1(s_1x_1))(t_2(s_2x_2))\cdots(t_n(s_nx_n))\\
&=_{\beta\eta}\lambda x_1\cdots x_n.\,zx_1\cdots x_n
=_\eta z.
\end{aligned}
$$

For the other order, [beta reduction](../../computability-theory.md#beta-reduction) gives

$$
\begin{aligned}
(q\bullet p)z
&\longrightarrow_\beta^*\lambda y_1\cdots y_n.\,
(pz)(t_1y_n)(t_2y_1)\cdots(t_ny_{n-1})\\
&\longrightarrow_\beta^*\lambda y_1\cdots y_n.\,
z(s_2(t_2y_1))\cdots(s_n(t_ny_{n-1}))(s_1(t_1y_n))\\
&=_{\beta\eta}\lambda y_1\cdots y_n.\,zy_1\cdots y_n
=_\eta z.
\end{aligned}
$$

These computations close the stronger induction. For $n=1$, each formula has the single argument involving $s_1$ and $t_1$; for $n=0$, the constructor is $I$ and its inverse is $I$. Every construction is finite, so the inverse is a finite [lambda term](../../computability-theory.md#lambda-term). There is no requirement that this inverse itself belong to $\mathcal R$.

$$
\boxed{\forall p\in\mathcal R\;\exists q:\quad
p\bullet q=_{\beta\eta}I=q\bullet p.}
$$

## 2

↑ **Parent:** [Lambda calculus and types](lambda-calculus-and-types.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [universal typing axiom](../../computability-theory.md#universal-typing-axiom) supplies $\varnothing\mapsto q:\star$ for every [lambda term](../../computability-theory.md#lambda-term) $q$. Use this as the argument premise of the [lambda application](../../computability-theory.md#lambda-application) rule. The empty [typing context](../../programming-language.md#typing-context) is consistent with $\Gamma$, and its [union](../../set.md#set-union) with $\Gamma$ is $\Gamma$:

$$
\frac{\Gamma\mapsto p:\star\Rightarrow A
\qquad \varnothing\mapsto q:\star}
{\Gamma\cup\varnothing\mapsto pq:A}.
$$

Hence

$$
\boxed{\Gamma\mapsto pq:A\quad\text{for every }q.}
$$

The [free variables](../../mathematical-logic.md#free-variable) of $q$ need not appear in the resulting [typing context](../../programming-language.md#typing-context): the [universal typing axiom](../../computability-theory.md#universal-typing-axiom) deliberately assigns $\star$ without recording them.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Choose $\star$ as the domain of the new [function type](../../programming-language.md#function-type). Since $x\notin\operatorname{Subjects}(\Gamma)$, the assumption $x:\star$ is consistent with $\Gamma$ and deleting $x$ leaves $\Gamma$ unchanged. The [lambda abstraction](../../computability-theory.md#lambda-abstraction) rule gives

$$
\frac{\Gamma\mapsto p:A}
{\Gamma\mapsto\lambda x.p:\star\Rightarrow A}.
$$

Use the [universal typing axiom](../../computability-theory.md#universal-typing-axiom) for $q$, then the [lambda application](../../computability-theory.md#lambda-application) rule:

$$
\frac{\Gamma\mapsto\lambda x.p:\star\Rightarrow A
\qquad\varnothing\mapsto q:\star}
{\Gamma\mapsto(\lambda x.p)q:A}.
$$

Therefore

$$
\boxed{\Gamma\mapsto(\lambda x.p)q:A\quad\text{for every }q.}
$$

The condition is about the [typing context](../../programming-language.md#typing-context), not the [free variables](../../mathematical-logic.md#free-variable) of $p$. Some occurrences of $x$ in $p$ might have been hidden by a use of the [universal typing axiom](../../computability-theory.md#universal-typing-axiom); the derivation above still follows the printed rules.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Begin with the variable [typing judgment](../../programming-language.md#typing-judgment) $\{x:A\}\mapsto x:A$. Because $z$ is absent from this [typing context](../../programming-language.md#typing-context), the [lambda abstraction](../../computability-theory.md#lambda-abstraction) rule permits $z$ to have type $\star$:

$$
\frac{\{x:A\}\mapsto x:A}
{\{x:A\}\mapsto\lambda z.x:\star\Rightarrow A}.
$$

Assign the entire [lambda application](../../computability-theory.md#lambda-application) $yx$ type $\star$ using the [universal typing axiom](../../computability-theory.md#universal-typing-axiom), without attempting to assign a [function type](../../programming-language.md#function-type) to $y$. Then

$$
\frac{\{x:A\}\mapsto\lambda z.x:\star\Rightarrow A
\qquad\varnothing\mapsto yx:\star}
{\{x:A\}\mapsto(\lambda z.x)(yx):A}.
$$

Although $y$ is a [free variable](../../mathematical-logic.md#free-variable) of the body, it is absent from its recorded [typing context](../../programming-language.md#typing-context). Consequently the [lambda abstraction](../../computability-theory.md#lambda-abstraction) rule allows any [simple type](../../programming-language.md#simple-type) $B$ for $y$. Abstract over $y$ and then $x$:

$$
\frac{\displaystyle
\frac{\{x:A\}\mapsto(\lambda z.x)(yx):A}
{\{x:A\}\mapsto\lambda y.(\lambda z.x)(yx):B\Rightarrow A}}
{\varnothing\mapsto\lambda xy.(\lambda z.x)(yx):A\Rightarrow(B\Rightarrow A)}.
$$

The side condition for $y$ holds because $y$ is absent; the side condition for $x$ holds because its recorded [simple type](../../programming-language.md#simple-type) is $A$. Thus

$$
\boxed{\varnothing\mapsto\lambda xy.(\lambda z.x)(yx):A\Rightarrow(B\Rightarrow A)
\quad\text{for all }A,B\text{ in }\mathrm{TA}_\lambda^\star.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The exact restriction in the ordinary [simply typed lambda calculus](../../computability-theory.md#simply-typed-lambda-calculus) is

$$
\boxed{\varnothing\mapsto\lambda xy.(\lambda z.x)(yx):A\Rightarrow(B\Rightarrow A)
\quad\Longleftrightarrow\quad
B=A\Rightarrow C\text{ for some simple type }C.}
$$

Thus the unrestricted choice of $A,B$ available in part (c) fails. A reading of the printed sentence as asserting impossibility for every choice of $A,B$ is false. This issue occurs in the original PDF as well as its transcription.[p. 2, Question 2(d)](../../computer-science-bibliography.md#lambda-calculus-and-types-examination-paper-of-the-university-of-oxford-2015)

To prove necessity, first observe why the ordinary rules cannot hide assumptions. [Structural induction](../../foundations-of-mathematics.md#structural-induction) on a derivation proves

$$
\operatorname{Subjects}(\Gamma)=FV(t)
\quad\text{whenever }\Gamma\mapsto t:T.
$$

For a variable, both sides are the singleton containing that variable. For [lambda application](../../computability-theory.md#lambda-application), both sides are the [union](../../set.md#set-union) of the two premise supports. For [lambda abstraction](../../computability-theory.md#lambda-abstraction), both sides delete the bound variable. There is no [universal typing axiom](../../computability-theory.md#universal-typing-axiom) to interrupt this equality.

Now invert the proposed derivation. Each outer [lambda abstraction](../../computability-theory.md#lambda-abstraction) must have been introduced by the abstraction rule, since the other ordinary rules conclude a variable or a [lambda application](../../computability-theory.md#lambda-application). The body must therefore have the [typing judgment](../../programming-language.md#typing-judgment)

$$
\{x:A,y:B\}\mapsto(\lambda z.x)(yx):A.
$$

The support equality just proved ensures that both displayed assumptions occur; consistency fixes their [simple types](../../programming-language.md#simple-type) to those specified by the outer [function type](../../programming-language.md#function-type). Inverting the [lambda application](../../computability-theory.md#lambda-application) gives a [simple type](../../programming-language.md#simple-type) $C$ for its argument and the following premises:

$$
\{x:A\}\mapsto\lambda z.x:C\Rightarrow A,
\qquad
\{x:A,y:B\}\mapsto yx:C.
$$

There is no flexibility in the supports: $\lambda z.x$ has the single [free variable](../../mathematical-logic.md#free-variable) $x$, whereas $yx$ has both [free variables](../../mathematical-logic.md#free-variable) $y,x$. Invert the second [lambda application](../../computability-theory.md#lambda-application). Its two premises must be

$$
\{y:B\}\mapsto y:D\Rightarrow C,
\qquad
\{x:A\}\mapsto x:D
$$

for some [simple type](../../programming-language.md#simple-type) $D$. The variable rule is the only possible final rule for each premise. It forces $D=A$ and $B=D\Rightarrow C$, yielding $B=A\Rightarrow C$.

Conversely, suppose $B=A\Rightarrow C$. The ordinary rules give

$$
\frac{\{y:A\Rightarrow C\}\mapsto y:A\Rightarrow C
\qquad\{x:A\}\mapsto x:A}
{\{x:A,y:A\Rightarrow C\}\mapsto yx:C},
\qquad
\frac{\{x:A\}\mapsto x:A}
{\{x:A\}\mapsto\lambda z.x:C\Rightarrow A}.
$$

The [typing contexts](../../programming-language.md#typing-context) are consistent, so another [lambda application](../../computability-theory.md#lambda-application) gives the body type $A$. Two [lambda abstractions](../../computability-theory.md#lambda-abstraction) discharge $y$ and $x$, establishing

$$
\varnothing\mapsto\lambda xy.(\lambda z.x)(yx):
A\Rightarrow((A\Rightarrow C)\Rightarrow A).
$$

This proves sufficiency and supplies a family of counterexamples to the literal impossibility claim. For a concrete failure of the unrestricted claim, choose $A=\alpha$ and $B=\beta$ as atomic [type variables](../../programming-language.md#type-variable). The [type variable](../../programming-language.md#type-variable) $\beta$ is not a [function type](../../programming-language.md#function-type) $\alpha\Rightarrow C$, so no derivation exists for that fixed pair. Here the atomic [type variables](../../programming-language.md#type-variable) are fixed type expressions, rather than unknowns that one may change during [type inference](../../programming-language.md#type-inference).

The reason for the restriction is the otherwise discarded [lambda application](../../computability-theory.md#lambda-application) $yx$: the ordinary rules still type-check it. Its subsequent disappearance under [beta reduction](../../computability-theory.md#beta-reduction) does not license reversing that [beta reduction](../../computability-theory.md#beta-reduction) while preserving every [simple type](../../programming-language.md#simple-type) of the result. The [beta-normal form](../../computability-theory.md#beta-normal-form) $\lambda xy.x$ admits arbitrary $A\Rightarrow(B\Rightarrow A)$, whereas the unreduced [lambda term](../../computability-theory.md#lambda-term) has the additional constraint just derived.

$$
\boxed{\text{The all-}A,B\text{ claim fails; the valid instances have }B=A\Rightarrow C.}
$$

## 3

↑ **Parent:** [Lambda calculus and types](lambda-calculus-and-types.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Take an infinite supply of variables and the two distinguished constants of [combinatory logic](../../computability-theory.md#combinatory-logic), the [K combinator](../../computability-theory.md#k-combinator) and the [S combinator](../../computability-theory.md#s-combinator). The [combinatory logic terms](../../computability-theory.md#combinatory-logic-term) are exactly the finite expressions generated by

$$
\boxed{T::=x\mid\mathbf K\mid\mathbf S\mid(TT).}
$$

Thus every variable and each distinguished constant is a [combinatory logic term](../../computability-theory.md#combinatory-logic-term), and the application of two [combinatory logic terms](../../computability-theory.md#combinatory-logic-term) is a [combinatory logic term](../../computability-theory.md#combinatory-logic-term). Nothing else is a [combinatory logic term](../../computability-theory.md#combinatory-logic-term). Application associates to the left, so $ABC$ means $(AB)C$; it is not assumed to be associative. The [I combinator](../../computability-theory.md#i-combinator) can be used as the abbreviation $\mathbf I\equiv\mathbf{SKK}$, without adding a new primitive constant.

The basic equality is the least relation containing the two axiom schemes

$$
\boxed{\mathbf KAB=A,\qquad\mathbf SABC=AC(BC)}
$$

for all [combinatory logic terms](../../computability-theory.md#combinatory-logic-term) $A,B,C$, and closed under the rules of [equational reasoning](../../foundations-of-mathematics.md#equational-reasoning):

$$
\frac{}{A=A},\qquad
\frac{A=B}{B=A},\qquad
\frac{A=B\quad B=C}{A=C},
\qquad
\frac{A=B\quad C=D}{AC=BD}.
$$

The final rule permits replacing equal [combinatory logic terms](../../computability-theory.md#combinatory-logic-term) inside either side of an application; repeated use permits replacement at any depth. Uniform [substitution](../../algebra.md#substitution-algebra) of [combinatory logic terms](../../computability-theory.md#combinatory-logic-term) for variables preserves equality, either included as a rule or proved by induction on these derivations, since the displayed axioms are schemes. No rule equating two [combinatory logic terms](../../computability-theory.md#combinatory-logic-term) merely because they agree after an extra argument belongs to this basic theory. Its equality is the symmetric, reflexive and transitive closure of [weak combinatory reduction](../../computability-theory.md#weak-combinatory-reduction).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $[x]A$ for the paper's [bracket abstraction](../../computability-theory.md#bracket-abstraction) and $I\equiv\mathbf{SKK}$ for the [I combinator](../../computability-theory.md#i-combinator). Prove the result by [structural induction](../../foundations-of-mathematics.md#structural-induction) following the three clauses of [bracket abstraction](../../computability-theory.md#bracket-abstraction).

For $A\equiv x$, the rules for the [S combinator](../../computability-theory.md#s-combinator) and the [K combinator](../../computability-theory.md#k-combinator) give

$$
([x]x)B\equiv\mathbf{SKK}B
=\mathbf KB(\mathbf KB)=B
\equiv x[B/x].
$$

If $x$ does not occur in $A$, then [substitution](../../algebra.md#substitution-algebra) for $x$ leaves $A$ unchanged and

$$
([x]A)B\equiv\mathbf KAB=A\equiv A[B/x].
$$

These two cases cover all variables and constants as well as applications not containing $x$.

In the remaining case, $A\equiv CD$ and $x$ occurs in at least one of $C,D$. The [bracket abstraction](../../computability-theory.md#bracket-abstraction) clause, the rule for the [S combinator](../../computability-theory.md#s-combinator), the induction hypotheses and compatibility of equality with application give

$$
\begin{aligned}
([x](CD))B
&\equiv\mathbf S([x]C)([x]D)B\\
&=(([x]C)B)(([x]D)B)\\
&=C[B/x]D[B/x]\\
&\equiv(CD)[B/x].
\end{aligned}
$$

The last line is the defining application clause of [substitution](../../algebra.md#substitution-algebra). Therefore

$$
\boxed{([x]A)B=A[B/x]\quad\text{for all }A,B.}
$$

The conclusion is equality in [combinatory logic](../../computability-theory.md#combinatory-logic); it need not be literal identity of strings. There are no binders in a [combinatory logic term](../../computability-theory.md#combinatory-logic-term), so this [substitution](../../algebra.md#substitution-algebra) introduces no [variable capture](../../computability-theory.md#variable-capture).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Again write $[x]A$ for [bracket abstraction](../../computability-theory.md#bracket-abstraction). In [combinatory logic](../../computability-theory.md#combinatory-logic), all variable occurrences are [free variables](../../mathematical-logic.md#free-variable). Under $x\neq y$ and $x\notin FV(B)$, [substitution](../../algebra.md#substitution-algebra) for $y$ preserves the presence or absence of $x$:

$$
x\in FV(C[B/y])\quad\Longleftrightarrow\quad x\in FV(C).
$$

An existing $x$ is not replaced because $x\neq y$; replacing $y$ cannot introduce an $x$ because $B$ contains none. This ensures that the same clause of [bracket abstraction](../../computability-theory.md#bracket-abstraction) applies before and after [substitution](../../algebra.md#substitution-algebra).

Use [structural induction](../../foundations-of-mathematics.md#structural-induction) on $A$, respecting those clauses. If $A\equiv x$, then

$$
([x]x)[B/y]\equiv\mathbf{SKK}
\equiv[x]x
\equiv[x](x[B/y]),
$$

because [substitution](../../algebra.md#substitution-algebra) leaves the [S combinator](../../computability-theory.md#s-combinator), the [K combinator](../../computability-theory.md#k-combinator) and $x$ unchanged.

If $x$ is absent from $A$, it is also absent from $A[B/y]$. Therefore

$$
([x]A)[B/y]
\equiv(\mathbf KA)[B/y]
\equiv\mathbf K(A[B/y])
\equiv[x](A[B/y]).
$$

This includes $A\equiv y$: even when $B$ is a large application, the absence of $x$ means [bracket abstraction](../../computability-theory.md#bracket-abstraction) still produces $\mathbf KB$.

Finally, let $A\equiv CD$ with $x$ occurring in $C$ or $D$. By the occurrence observation, $x$ also occurs in $C[B/y]$ or $D[B/y]$, so the application clause applies on both sides. Apply the induction hypotheses:

$$
\begin{aligned}
([x](CD))[B/y]
&\equiv\bigl(\mathbf S([x]C)([x]D)\bigr)[B/y]\\
&\equiv\mathbf S\bigl(([x]C)[B/y]\bigr)\bigl(([x]D)[B/y]\bigr)\\
&\equiv\mathbf S\bigl([x](C[B/y])\bigr)\bigl([x](D[B/y])\bigr)\\
&\equiv[x]\bigl(C[B/y]D[B/y]\bigr)\\
&\equiv[x]\bigl((CD)[B/y]\bigr).
\end{aligned}
$$

Every step uses the definitions of [substitution](../../algebra.md#substitution-algebra) and [bracket abstraction](../../computability-theory.md#bracket-abstraction), without applying the equality axioms for the [S combinator](../../computability-theory.md#s-combinator) or the [K combinator](../../computability-theory.md#k-combinator). Thus the result is the stronger syntactic identity

$$
\boxed{([x]A)[B/y]\equiv[x](A[B/y]).}
$$

The side condition on $B$ is essential for this identity. For example, substituting $x$ for $y$ in $[x]y\equiv\mathbf Ky$ gives $\mathbf Kx$, whereas $[x](y[x/y])\equiv[x]x\equiv\mathbf{SKK}$, a different string.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Successive [bracket abstractions](../../computability-theory.md#bracket-abstraction) are processed from the inside out: $[x][y]((\mathbf Kx)y)$. Retain $I\equiv(\mathbf S\mathbf K)\mathbf K$ only as a temporary abbreviation for the [I combinator](../../computability-theory.md#i-combinator). Since $y$ is absent from $\mathbf Kx$, the first [bracket abstraction](../../computability-theory.md#bracket-abstraction) is

$$
[y]((\mathbf Kx)y)
\equiv\mathbf S\bigl(\mathbf K(\mathbf Kx)\bigr)I.
$$

For the outer [bracket abstraction](../../computability-theory.md#bracket-abstraction), $x$ is absent from $I$ and the [S combinator](../../computability-theory.md#s-combinator), while it occurs in $\mathbf K(\mathbf Kx)$. Hence

$$
\begin{aligned}
[x]\bigl(\mathbf S(\mathbf K(\mathbf Kx))I\bigr)
&\equiv\mathbf S\bigl([x](\mathbf S(\mathbf K(\mathbf Kx)))\bigr)(\mathbf KI),\\
[x](\mathbf S(\mathbf K(\mathbf Kx)))
&\equiv\mathbf S(\mathbf K\mathbf S)\bigl([x](\mathbf K(\mathbf Kx))\bigr),\\
[x](\mathbf K(\mathbf Kx))
&\equiv\mathbf S(\mathbf K\mathbf K)\bigl([x](\mathbf Kx)\bigr),\\
[x](\mathbf Kx)
&\equiv\mathbf S(\mathbf K\mathbf K)I.
\end{aligned}
$$

Substituting upward and then expanding $I$ gives the following fully bracketed string, consisting solely of the [S combinator](../../computability-theory.md#s-combinator), the [K combinator](../../computability-theory.md#k-combinator) and parentheses:

$$
\boxed{
\left(
\left(\mathbf S
\left(
\left(\mathbf S(\mathbf K\mathbf S)\right)
\left(
\left(\mathbf S(\mathbf K\mathbf K)\right)
\left(\left(\mathbf S(\mathbf K\mathbf K)\right)\left((\mathbf S\mathbf K)\mathbf K\right)\right)
\right)
\right)
\right)
\left(\mathbf K\left((\mathbf S\mathbf K)\mathbf K\right)\right)
\right).
}
$$

For readability, the same result with the usual left association convention and the temporary abbreviation is

$$
\mathbf S\bigl(\mathbf S(\mathbf K\mathbf S)
(\mathbf S(\mathbf K\mathbf K)(\mathbf S(\mathbf K\mathbf K)I))\bigr)(\mathbf KI).
$$

The syntactic result comes from the specified [bracket abstraction](../../computability-theory.md#bracket-abstraction) algorithm. Replacing it by the shorter [K combinator](../../computability-theory.md#k-combinator), despite agreement after two arguments, would not answer the requested computation. As a check using the result of part (b), applying the computed [combinatory logic term](../../computability-theory.md#combinatory-logic-term) to $u,v$ gives $\mathbf Kuv=u$.

## ↑ Ancestors (8)

1. [2015](../2015.md)
2. [Past exam of the computer science course of the University of Oxford](../../past-exam-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
4. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
5. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
6. [University of Oxford](../../university-of-oxford.md)
7. [List of universities](../../README.md#list-of-universities)
8. [Codex Wiki](../../README.md)
