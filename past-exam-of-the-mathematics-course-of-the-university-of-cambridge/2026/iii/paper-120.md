# Paper 120

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20120.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20120.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
  - [g](#3/g)
    - [Solution](#3/g/solution)

## 1

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [Kripke model for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-model-for-intuitionistic-propositional-logic) for a propositional language is a poset $(S,\leq)$ together with a persistent forcing relation on atoms: if $w\Vdash p$ and $w\leq v$, then $v\Vdash p$. Extend forcing by

$$
w\Vdash\alpha\wedge\beta\iff w\Vdash\alpha\text{ and }w\Vdash\beta,
$$



$$
w\Vdash\alpha\vee\beta\iff w\Vdash\alpha\text{ or }w\Vdash\beta,
$$

and

$$
w\Vdash\alpha\to\beta\iff
\text{for every }v\geq w, v\Vdash\alpha\Longrightarrow v\Vdash\beta.
$$

**No world forces $\bot$.** Induction proves persistence for every proposition.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Kripke completeness theorem for intuitionistic propositional logic](../../../mathematical-logic.md#kripke-completeness-theorem-for-intuitionistic-propositional-logic) says

$$
\vdash_{IPC}\varphi
\quad\Longleftrightarrow\quad
w\Vdash\varphi
$$

for every world $w$ in every intuitionistic Kripke model.

Take a root $r$ with two incomparable successors $u,v$. Force $p$ but not $q$ at $u$, force $q$ but not $p$ at $v$, and force neither at $r$. Then $r\nVdash p\to q$ because of $u$, and $r\nVdash q\to p$ because of $v$. Hence

$$
r\nVdash(p\to q)\vee(q\to p),
$$

so completeness shows that this proposition is not intuitionistically valid.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

On equivalence classes define

$$
[w]\preceq[v]iff\operatorname{Th}_\varphi(w)\subseteq\operatorname{Th}_\varphi(v),
$$

and, for every atomic proposition $p\in\Phi$, put $[w]\Vdash p$ exactly when $w\Vdash p$. This is well-defined, is a partial order, and makes atomic forcing persistent.

The [filtration of a Kripke model](../../../mathematical-logic.md#filtration-of-a-kripke-model) truth lemma states

$$
[w]\Vdash\psi\iff w\Vdash\psi\qquad(\psi\in\Phi).
$$

Conjunction and disjunction are immediate by induction. For implication, if $w\Vdash\alpha\to\beta$ and $[w]\preceq[v]$, then $\alpha\to\beta$ belongs to $\operatorname{Th}_\varphi(v)$; if $[v]\Vdash\alpha$, induction gives $v\Vdash\alpha$, hence $v\Vdash\beta$ and $[v]\Vdash\beta$. Conversely, if $w\nVdash\alpha\to\beta$, some actual $v\geq w$ forces $\alpha$ but not $\beta$; persistence gives $[w]\preceq[v]$, which witnesses failure in the quotient. Thus every formula in $\Phi$ is preserved.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $T$ consist of all finite nondecreasing paths

$$
(s_0,s_1,\ldots,s_k),qquad s_0\leq_Ss_1\leq_S\cdots\leq_Ss_k,
$$

ordered by initial-segment extension. The one-point path $(s_0)$ is least, and the predecessors of any path are its initial segments, hence linearly ordered. Force an atom at a path exactly when it is forced at the path's endpoint.

The endpoint map $e:T\to S$ is monotone and has the back property: if $e(t)\leq_Ss$, append $s$ to $t$. Induction on propositions therefore gives

$$
t\Vdash_T\psi\iff e(t)\Vdash_S\psi.
$$

In particular the roots force exactly the same propositions. This is the [unravelling of a Kripke model](../../../mathematical-logic.md#unravelling-of-a-kripke-model).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Assume $\nvdash_{IPC}\varphi$. By Kripke completeness there is a rooted countermodel. Unravel it into a tree and retain only the subformulas $\Phi$ of $\varphi$. Whenever a retained node fails an implication $\alpha\to\beta\in\Phi$, retain one successor witnessing $\alpha$ and the failure of $\beta$. Along a branch, passing to a genuinely new witness strictly enlarges the finite theory of subformulas, so at most $n$ witness levels are needed. Identifying repeated equal theories and retaining at most one witness for each failed implication leaves at most $n$ representatives for each of the at most $2^n$ theories. The resulting pruned filtration has at most $n2^n$ worlds and still refutes $\varphi$ by the truth lemma.

**Thus every underivable formula with $n$ subformulas has a countermodel of size at most $n2^n$. The contrapositive proves the claim and is the quantitative [Finite model property of intuitionistic propositional logic](../../../mathematical-logic.md#finite-model-property-of-intuitionistic-propositional-logic).**

## 2

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [Sigma-1 formula](../../../foundations-of-mathematics.md#sigma-1-formula) is a formula equivalent in first-order arithmetic to

$$
\exists y_1\cdots\exists y_k\,\delta,
$$

where $\delta$ is bounded. A [Pi-1 formula](../../../foundations-of-mathematics.md#pi-1-formula) is similarly equivalent to $\forall y_1\cdots\forall y_k\,\delta$ with bounded $\delta$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [diagonal lemma](../../../mathematical-logic.md#diagonal-lemma) states that for every formula $\theta(x)$ with one free variable there is a sentence $\gamma$ such that

$$
PA^-\vdash\gamma\leftrightarrow\theta(\ulcorner\gamma\urcorner).
$$

The same conclusion holds in every theory extending the arithmetic needed to formalize substitution.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [crude incompleteness theorem](../../../mathematical-logic.md#crude-incompleteness-theorem) says that every consistent recursively axiomatized extension $T$ of $PA^-$ is incomplete.

Suppose instead that $T$ were complete. Enumerating proofs until either $\sigma$ or $\neg\sigma$ appears would decide theoremhood, so its characteristic function $\chi_T$ would be total recursive. By the assumed representation theorem, choose a formula $R(x)$ such that $PA^-$ proves $R(\bar n)$ when $\chi_T(n)=1$ and proves $\neg R(\bar n)$ when $\chi_T(n)=0$. The diagonal lemma supplies $\gamma$ with

$$
PA^-\vdash\gamma\leftrightarrow\neg R(\ulcorner\gamma\urcorner).
$$

If $T\vdash\gamma$, then $\chi_T(\ulcorner\gamma\urcorner)=1$, so $T\vdash R(\ulcorner\gamma\urcorner)$ and is inconsistent. If $T\vdash\neg\gamma$, then the characteristic value is zero, so $T\vdash\neg R(\ulcorner\gamma\urcorner)$ and hence $T\vdash\gamma$, again a contradiction. Completeness must therefore fail.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The recursive theory $T=PA^-+\varphi$ is consistent because $\mathbb N\models T$. By the Gödel-Rosser theorem it has an undecidable sentence $\rho$, so both $T+\rho$ and $T+\neg\rho$ are consistent. Exactly one of $\rho,\neg\rho$ is false in $\mathbb N$; add that one to $T$. The first-order completeness theorem gives a model, and the [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem) gives a countable model $M$. Then $M\models PA^-+\varphi$, but $M$ disagrees with $\mathbb N$ on the chosen sentence and is therefore not elementarily equivalent to it.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Disjoint sets $A,B\subseteq\mathbb N$ are [recursively inseparable](../../../foundations-of-mathematics.md#recursively-inseparable-sets) when there is no recursive $C\subseteq\mathbb N$ such that

$$
\boxed{A\subseteq C,
\qquad
B\cap C=\varnothing.}
$$

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Consistency of $PA^-$ makes $A$ and $B$ disjoint. Suppose a recursive set $C$ separated them, and let $R(x)$ represent its total characteristic function in $PA^-$. By the [diagonal lemma](../../../mathematical-logic.md#diagonal-lemma), choose a sentence $\sigma$ satisfying

$$
PA^-\vdash\sigma\leftrightarrow\neg R(\ulcorner\sigma\urcorner).
$$

Put $n=\ulcorner\sigma\urcorner$. If $n\in C$, representability gives $PA^-\vdash R(\bar n)$ and hence $PA^-\vdash\neg\sigma$, so $n\in B$, contradicting $B\cap C=\varnothing$. If $n\notin C$, representability gives $PA^-\vdash\neg R(\bar n)$ and hence $PA^-\vdash\sigma$, so $n\in A\subseteq C$, again a contradiction. Therefore $A$ and $B$ are recursively inseparable.

## 3

↑ **Parent:** [Paper 120](paper-120.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A partial function $f:\mathbb N^k\rightharpoonup\mathbb N$ is [lambda-definable](../../../foundations-of-mathematics.md#lambda-definable-partial-function) if there is a lambda term $F$ such that

$$
F c_{n_1}\cdots c_{n_k}\equiv_\beta c_{f(n_1,\ldots,n_k)}
$$

whenever the value is defined, while outside the domain the application reduces to no [Church numeral](../../../foundations-of-mathematics.md#church-numeral).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Strong normalization theorem for simply typed lambda calculus](../../../foundations-of-mathematics.md#strong-normalization-theorem-for-simply-typed-lambda-calculus) says that every well-typed term has no infinite beta-reduction sequence. In the untyped calculus,

$$
\Omega=(\lambda x.xx)(\lambda x.xx)
$$

reduces to itself and is therefore not strongly normalizing.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The nowhere-defined partial function is represented by

$$
F=\lambda n.\Omega.
$$

For every Church numeral $c_m$, the term $Fc_m$ reduces to $\Omega$ and hence to no numeral. If $F$ had type $Nat\to Nat$, the strong normalization theorem would make every reduction sequence from $F$ finite, contradicting the visible infinite reduction inside $\Omega$. Thus this partial function is lambda-definable by an untypable term of the required kind.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

A closed beta-eta-long normal term of type $\sigma\to\sigma\to\sigma$ must have the form $\lambda x:\sigma.\lambda y:\sigma.t$, where the normal term $t:\sigma$ can only be $x$ or $y$: the pure calculus has no constants or other closed source of a value of the atomic type $\sigma$. Hence the only two beta-eta-equivalence classes are the [Church Booleans](../../../foundations-of-mathematics.md#church-boolean)

$$
\boxed{\top=\lambda x.\lambda y.x,
\qquad
\bot=\lambda x.\lambda y.y.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Take

$$
OR=\lambda a:Bool_\sigma.\lambda b:Bool_\sigma.
\lambda x:\sigma.\lambda y:\sigma.a\,x\,(b\,x\,y).
$$

It has type $Bool_\sigma\to Bool_\sigma\to Bool_\sigma$. If $a\equiv_\beta\top$, the body selects $x$. If $a\equiv_\beta\bot$, it reduces to $bxy$, which selects $x$ exactly when $b\equiv_\beta\top$. Thus it has the stated truth table.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

For $a\in\{0,1\}$ define a typed transition term $D_a:\sigma\to\sigma$ by a nested Boolean choice:

$$
D_a=\lambda x:\sigma.
eq_\sigma,x,q_0,q_{\delta(q_0,a)}
\bigl(eq_\sigma,x,q_1,q_{\delta(q_1,a)}
\bigl(\cdots(eq_\sigma,x,q_{n-2},q_{\delta(q_{n-2},a)},q_{\delta(q_{n-1},a)})\cdots\bigr)\bigr).
$$

Here a Church Boolean acts as an if-then-else operator. The assumed behavior of $eq_\sigma$ gives $D_aq_i\equiv_\beta q_{\delta(q_i,a)}$.

For $w=a_1\cdots a_k$, put

$$
\mathbf w=\lambda x:\sigma.D_{a_k}(D_{a_{k-1}}(\cdots D_{a_1}x\cdots)),
$$

and use $\mathbf\epsilon=\lambda x.x$. Induction on the word length gives

$$
\boxed{\mathbf wq_0\equiv_\beta q_{\delta^*(q_0,w)}.}
$$

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

Given a finite input word $w$, construct the typed term $\mathbf wq_0$ effectively and beta-normalize it. The [Strong normalization theorem for simply typed lambda calculus](../../../foundations-of-mathematics.md#strong-normalization-theorem-for-simply-typed-lambda-calculus) guarantees termination, and confluence gives exactly one of the finitely many normal forms $q_i$. Compare that normal form syntactically with the listed accepting states in $F$. This algorithm accepts exactly when $\delta^*(q_0,w)\in F$, so $L$ is recursive. Equivalently, this is the standard theorem that every language recognized by a [deterministic finite automaton](../../../foundations-of-mathematics.md#deterministic-finite-automaton) is a [regular language](../../../foundations-of-mathematics.md#regular-language) and hence decidable.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
