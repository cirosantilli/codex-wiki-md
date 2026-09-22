<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use [untyped lambda calculus](../../../../../untyped-lambda-calculus.md) and [normal-order beta reduction](../../../../../normal-order-beta-reduction.md). Write $c_n=\lambda f x.f^n x$ for the [Church numeral](../../../../../church-numeral.md) of $n$. We will construct a closed term $F$ such that

$$
F c_{n_1}\cdots c_{n_k}\longrightarrow_\beta^*c_{f(\mathbf n)}
$$

when $f(\mathbf n)$ is defined, and with no [head normal form](../../../../../head-normal-form.md) otherwise. The latter condition implies that the result is not in [beta equivalence](../../../../../beta-equivalence.md) with any [Church numeral](../../../../../church-numeral.md), so both definedness and the output are represented.

First represent all total [primitive recursive functions](../../../../../primitive-recursive-function.md). The [zero function](../../../../../zero-function.md) is $\lambda\mathbf x.c_0$, the [successor function](../../../../../successor-function.md) is

$$
\mathsf{Succ}=\lambda n f x.f(nfx),
$$

and the $i$th [projection function](../../../../../projection-function.md) is $\lambda x_1\cdots x_k.x_i$. [Function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md) is represented by $\lambda\mathbf x.G(H_1\mathbf x)\cdots(H_r\mathbf x)$. This composition claim is used here for total [functions](../../../../../function-split.md), whose inner terms all reduce to numerals.

For [primitive recursion](../../../../../primitive-recursion.md) use [Church pairs](../../../../../church-pair.md) and iteration. Put

$$
\mathsf T=\lambda a b.a,\quad\mathsf F=\lambda a b.b,\quad\mathsf{Pair}=\lambda a b p.pab,\quad\mathsf{Fst}=\lambda p.p\mathsf T,\quad\mathsf{Snd}=\lambda p.p\mathsf F.
$$

Suppose $G,H$ represent the total constituents of $f(\mathbf x,0)=g(\mathbf x)$ and $f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n))$. Define

$$
\begin{aligned}
\mathsf{Step}_{\mathbf x}&=\lambda p.\mathsf{Pair}\bigl(\mathsf{Succ}(\mathsf{Fst}\,p)\bigr)\bigl(H\mathbf x(\mathsf{Fst}\,p)(\mathsf{Snd}\,p)\bigr),\\
R&=\lambda\mathbf x n.\mathsf{Snd}\bigl(n\mathsf{Step}_{\mathbf x}(\mathsf{Pair}\,c_0\,(G\mathbf x))\bigr).
\end{aligned}
$$

After $j$ iterations the pair reduces to $\mathsf{Pair}\,c_j\,c_{f(\mathbf x,j)}$, by [mathematical induction](../../../../../mathematical-induction.md) on $j$. Its second projection is the required result. This [lambda definition of primitive recursion by pair iteration](../../../../../lambda-definition-of-primitive-recursion-by-pair-iteration.md) and [structural induction](../../../../../structural-induction.md) on the primitive recursive construction give terms for all [primitive recursive functions](../../../../../primitive-recursive-function.md).

For an arbitrary [partial computable function](../../../../../computable-function.md) use the [Kleene normal form theorem](../../../../../kleene-normal-form-theorem.md) with its program index fixed. There are total [primitive recursive functions](../../../../../primitive-recursive-function.md) $C(\mathbf x,s)$ and $U(s)$ such that $C$ is zero exactly when $s$ codes a valid halting computation history on $\mathbf x$, and $U$ extracts that history's output. Checking finite coded configurations and each transition is primitive recursive. Determinism ensures that every accepted history on an input has the same output. Hence

$$
f(\mathbf x)=U(\mu s\,[C(\mathbf x,s)=0]).
$$

If the input computation never halts, no history is accepted. Let $\widehat C,\widehat U$ be the total numeral-representing terms already obtained. The [Church numeral zero test](../../../../../church-numeral-zero-test.md) is $\mathsf{Zero}=\lambda n.n(\lambda z.\mathsf F)\mathsf T$, returning $\mathsf T$ exactly on zero. A [Church Boolean](../../../../../church-boolean.md) applied to two arguments selects the appropriate branch without evaluating the other.

Take the [fixed-point combinator](../../../../../fixed-point-combinator.md) $Y=\lambda h.(\lambda z.h(zz))(\lambda z.h(zz))$. For the input tuple define

$$
G_{\mathbf x}=\lambda r s.\bigl(\mathsf{Zero}(\widehat C\mathbf x s)\bigr)\,(\widehat U s)\,(r(\mathsf{Succ}\,s)),\qquad F=\lambda\mathbf x.(YG_{\mathbf x})c_0.
$$

Expanding the displayed abbreviations gives a genuine finite [combinator](../../../../../combinator.md). At a numeral code $c_j$, the total predicate computation terminates. If it returns a positive numeral, the false [Church Boolean](../../../../../church-boolean.md) selects the next search code. If it returns zero, the true [Church Boolean](../../../../../church-boolean.md) selects $\widehat U c_j$, which reduces to the output numeral. If the least accepted code is $s$, a finite [sequence](../../../../../sequence.md) of these tests reaches it and then produces $c_{U(s)}$.

If there is no accepted code, every test is false and head reduction moves through codes $0,1,2,\ldots$ forever. At no finite point can a head variable or an outer numeral abstraction be produced: the applied search term must first unfold the fixed point and evaluate the next total test, and the decoder branch is always discarded. Thus it has no [head normal form](../../../../../head-normal-form.md). The standard head-normalization property, or the [Church-Rosser theorem](../../../../../church-rosser-theorem.md) together with normalization of normal-order reduction, rules out [beta equivalence](../../../../../beta-equivalence.md) to a numeral. In particular, we have avoided a lazy-composition pitfall: an outer [function](../../../../../function-split.md) that discards an argument need not force a divergent inner computation. The decoder is reached only after the guarded search succeeds. This proves [lambda representation of partial computable functions](../../../../../lambda-representation-of-partial-computable-functions.md):

$$
\boxed{f(\mathbf n)\downarrow=m\Rightarrow F\mathbf c_{\mathbf n}\equiv_\beta c_m,\qquad f(\mathbf n)\uparrow\Rightarrow F\mathbf c_{\mathbf n}\text{ has no head normal form.}}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
