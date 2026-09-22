<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Represent a nonnegative [integer](../../../../../integer.md) $n$ by the [Church numeral](../../../../../church-numeral.md)

$$
\underline n=\lambda f.\lambda x.f^n x.
$$

A closed [lambda term](../../../../../lambda-term.md) $F$ represents a [partial computable function](../../../../../computable-function.md) $f$ if, on inputs in its domain, $F\underline{n_1}\cdots\underline{n_k}$ reduces to the [Church numeral](../../../../../church-numeral.md) of the value, and on other inputs it produces no [Church numeral](../../../../../church-numeral.md). We use [untyped lambda calculus](../../../../../untyped-lambda-calculus.md) and [normal-order beta reduction](../../../../../normal-order-beta-reduction.md).

First every [primitive recursive function](../../../../../primitive-recursive-function.md) has such a representation on all inputs. The [zero function](../../../../../zero-function.md) is represented by a constant $\underline0$, the [projection functions](../../../../../projection-function.md) by $\lambda x_1\cdots x_k.x_i$, and the [successor function](../../../../../successor-function.md) by

$$
\mathsf{Succ}=\lambda n f x.f(nfx).
$$

For [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md), substitute the represented inner functions into the represented outer function:

$$
\lambda\mathbf x.\,G(H_1\mathbf x)\cdots(H_m\mathbf x).
$$

These constituent functions are total, so there is no undefined argument to be discarded.

For [primitive recursion](../../../../../primitive-recursion.md), use [Church Booleans](../../../../../church-boolean.md) and [Church pairs](../../../../../church-pair.md):

$$
\mathsf T=\lambda a b.a,\quad \mathsf F=\lambda a b.b,\quad
\mathsf{Pair}=\lambda a b p.pab,\quad
\mathsf{Fst}=\lambda p.p\mathsf T,\quad
\mathsf{Snd}=\lambda p.p\mathsf F.
$$

If $G,H$ represent the total functions defining a recursion, put

$$
\mathsf{Step}_{\mathbf x}=\lambda p.\,
\mathsf{Pair}\bigl(\mathsf{Succ}(\mathsf{Fst}\,p)\bigr)
\bigl(H\mathbf x(\mathsf{Fst}\,p)(\mathsf{Snd}\,p)\bigr),
$$

and

$$
R=\lambda\mathbf x n.\,
\mathsf{Snd}\bigl(n\mathsf{Step}_{\mathbf x}
(\mathsf{Pair}\,\underline0\,(G\mathbf x))\bigr).
$$

After $j$ iterations the [Church pair](../../../../../church-pair.md) contains the counter $\underline j$ and the recursively computed value at $j$, by [mathematical induction](../../../../../mathematical-induction.md). Thus this [lambda definition of primitive recursion by pair iteration](../../../../../lambda-definition-of-primitive-recursion-by-pair-iteration.md) represents the recursion. A [structural induction for primitive recursive functions](../../../../../structural-induction-for-primitive-recursive-functions.md) now represents every [primitive recursive function](../../../../../primitive-recursive-function.md).

To pass to arbitrary [partial computable functions](../../../../../computable-function.md), use the [Kleene normal form theorem](../../../../../kleene-normal-form-theorem.md) in the following form: for every $f:\mathbb N^k\rightharpoonup\mathbb N$, there are total [primitive recursive functions](../../../../../primitive-recursive-function.md) $C,U$ such that

$$
f(\mathbf x)=U\bigl(\mu t\,[C(\mathbf x,t)=0]\bigr),
$$

with $f$ undefined precisely when no such $t$ exists. The predicate checks codes of valid finite halting histories for the chosen program; $U$ extracts their common output. This expresses [unbounded minimization](../../../../../mu-operator.md) of a total predicate, so no earlier undefined test can interfere with the search.

Let $\widehat C,\widehat U$ be the represented total functions. The [Church numeral zero test](../../../../../church-numeral-zero-test.md) and a [fixed-point combinator](../../../../../fixed-point-combinator.md) are

$$
\mathsf{Zero}=\lambda n.n(\lambda z.\mathsf F)\mathsf T,
\qquad
Y=\lambda h.(\lambda z.h(zz))(\lambda z.h(zz)).
$$

Define the search [lambda term](../../../../../lambda-term.md)

$$
Q=Y\bigl(\lambda q\,\mathbf x\,t.\,
(\mathsf{Zero}(\widehat C\mathbf x t))
(\widehat U t)
(q\mathbf x(\mathsf{Succ}\,t))\bigr),
\qquad F=\lambda\mathbf x.Q\mathbf x\underline0.
$$

All displayed abbreviations expand to finite closed [lambda terms](../../../../../lambda-term.md); $\mathbf x$ stands for the fixed finite tuple of input variables. Because $YH\equiv_\beta H(YH)$, [normal-order beta reduction](../../../../../normal-order-beta-reduction.md) tests $t=0,1,2,\ldots$. At the first successful test the [Church Boolean](../../../../../church-boolean.md) selects $\widehat U t$, which reduces to the correct [Church numeral](../../../../../church-numeral.md). The unused recursive branch is discarded.

If no test succeeds, every finite search step returns to another head search, never exposing a numeral. The term has no [head normal form](../../../../../head-normal-form.md) and hence cannot be [beta equivalent](../../../../../beta-equivalence.md) to a [Church numeral](../../../../../church-numeral.md). This last point is why the output operation occurs inside the successful branch: simply applying a possibly argument-discarding outer function to a divergent search would not justify undefinedness. Therefore **every computable function is representable**, including [partial computable functions](../../../../../computable-function.md) with their correct undefined inputs:

$$
\boxed{\begin{aligned}f(\mathbf n)\downarrow\ &\Longrightarrow\
F\underline{\mathbf n}\to_\beta^*\underline{f(\mathbf n)};
\\ f(\mathbf n)\uparrow\ &\Longrightarrow\text{no numeral result}.\end{aligned}}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
