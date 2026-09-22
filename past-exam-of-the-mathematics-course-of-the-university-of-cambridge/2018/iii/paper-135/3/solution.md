<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The machine characterization is computation by a [Turing machine](../../../../../turing-machine.md): the machine halts with $f(\mathbf n)$ exactly on inputs in the [domain of a partial function](../../../../../domain-of-a-partial-function.md) and does not halt elsewhere. The syntactic characterization is the least class containing the [initial functions of recursion theory](../../../../../initial-function-of-recursion-theory.md) and closed under [composition of partial functions](../../../../../composition-of-partial-functions.md), [primitive recursion](../../../../../primitive-recursion.md) and [unbounded minimization](../../../../../mu-operator.md). Such functions are the [partial recursive functions](../../../../../computable-function.md), equivalently the [partial computable functions](../../../../../computable-function.md).

For clarity, composition here is strict: $g(h_1(\mathbf n),\ldots,h_r(\mathbf n))$ is defined only when every inner value is defined and $g$ is defined on the resulting tuple. Likewise primitive recursion requires all preceding recursive values. The partial minimization $\mu y\,[g(\mathbf n,y)=0]$ is defined when such a $y$ exists and all earlier values are defined and nonzero; an undefined earlier value blocks the search.

A [lambda-definable partial function](../../../../../lambda-definable-partial-function.md) is represented by a closed [untyped lambda calculus](../../../../../untyped-lambda-calculus.md) term $F$ satisfying

$$
f(\mathbf n)=m\iff F\,c_{n_1}\cdots c_{n_k}\equiv_\beta c_m,
\qquad c_n=\lambda a.\lambda b.a^n b.
$$

On an input outside its domain there must be no [Church numeral](../../../../../church-numeral.md) beta-equivalent to the result. A stronger representation can be arranged: undefined inputs have no [head normal form](../../../../../head-normal-form.md).

Here are the components for proving that every partial recursive function is lambda-definable. Zero and projections are immediate; [lambda definition of the successor function](../../../../../lambda-definition-of-the-successor-function.md) uses $\mathrm{Succ}=\lambda n.\lambda a.\lambda b.a(nab)$. [Church Booleans](../../../../../church-boolean.md) encode a conditional by $bUV$, with $\mathrm{True}=\lambda u.\lambda v.u$ and $\mathrm{False}=\lambda u.\lambda v.v$. Put

$$
\begin{aligned}
\mathrm{Pair}&=\lambda a.\lambda b.\lambda k.kab,\\
\mathrm{First}&=\lambda p.p\,\mathrm{True},\qquad \mathrm{Second}=\lambda p.p\,\mathrm{False},\\
\mathrm{Step}&=\lambda p.\mathrm{Pair}\,(\mathrm{Second}\,p)\,(\mathrm{Succ}(\mathrm{Second}\,p)),\\
\mathrm{Pred}&=\lambda n.\mathrm{First}\bigl(n\,\mathrm{Step}\,(\mathrm{Pair}\,c_0\,c_0)\bigr),\\
\mathrm{IsZero}&=\lambda n.n(\lambda z.\mathrm{False})\,\mathrm{True}.
\end{aligned}
$$

Iteration takes $(0,0)$ to $(n-1,n)$ for $n>0$, proving that $\mathrm{Pred}\,c_n$ encodes the [predecessor function](../../../../../predecessor-function.md) and that $\mathrm{IsZero}$ correctly tests zero.

Use a [fixed-point combinator](../../../../../fixed-point-combinator.md) $Y$ and the strict sequencing operation

$$
\mathrm{Force}=\lambda n.\lambda k.n\,(\lambda z.z)\,k.
$$

For any numeral $c_m$, $\mathrm{Force}\,c_m\,K$ reduces to $K$. If the first argument has no [head normal form](../../../../../head-normal-form.md), neither does the whole expression. Thus composition is implemented by nesting $\mathrm{Force}$ on every inner result before applying the outer representing term. This guard is important: an unguarded projection could discard an undefined inner computation.

For [lambda definition of primitive recursion](../../../../../lambda-definition-of-primitive-recursion.md), with $g,h$ already represented by $G,H$, take

$$
\begin{aligned}
R=Y\bigl(\lambda r.\lambda\mathbf x.\lambda n.\;
\mathrm{IsZero}\,n\;(G\mathbf x)\;
\bigl(\mathrm{Force}\,(r\mathbf x(\mathrm{Pred}\,n))\,
(H\mathbf x(\mathrm{Pred}\,n)(r\mathbf x(\mathrm{Pred}\,n)))\bigr)\bigr).
\end{aligned}
$$

The tuple notation abbreviates successive abstractions and applications. On numeral inputs, induction on $n$ proves the required recursion equations, including strict propagation of undefined preceding values. The [beta reduction](../../../../../beta-reduction.md) follows the selected conditional branch only.

For [lambda definition of unbounded minimization](../../../../../lambda-definition-of-unbounded-minimization.md), use

$$
Q=Y\bigl(\lambda q.\lambda\mathbf x.\lambda j.\;
\mathrm{IsZero}(G\mathbf xj)\;j\;(q\mathbf x(\mathrm{Succ}\,j))\bigr),
\qquad F\mathbf x=Q\mathbf x c_0.
$$

This searches in increasing order. An undefined value blocks the zero test; an infinite sequence of nonzero values continues forever; the first zero returns its numeral. Under [normal-order beta reduction](../../../../../normal-order-beta-reduction.md), both failure cases have no [head normal form](../../../../../head-normal-form.md). Structural induction on partial-recursive declarations now supplies the stronger representation claimed above.

Conversely, [beta reduction](../../../../../beta-reduction.md) is an effective operation on finitely encoded [lambda terms](../../../../../lambda-term.md). Enumerate all finite reduction sequences from $F\mathbf c_n$, stopping when a result is a [Church numeral](../../../../../church-numeral.md) in [beta-normal form](../../../../../beta-normal-form.md). If $F\mathbf c_n\equiv_\beta c_m$, the [Church-Rosser theorem](../../../../../church-rosser-theorem.md) gives a reduction to that numeral. It also makes the output unique. The enumeration therefore computes exactly the represented partial function; by the equivalence of the first two characterizations it is partial recursive. Hence

$$
\boxed{\text{partial computable}=\text{partial recursive}=\text{lambda-definable partial}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
