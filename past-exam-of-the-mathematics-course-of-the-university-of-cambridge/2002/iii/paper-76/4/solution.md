<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [Church numerals](../../../../../church-numeral.md)

$$
c_n=\lambda f x.f^n x,\qquad \mathsf T=\lambda ab.a,\qquad\mathsf F=\lambda ab.b.
$$

Explicit [lambda terms](../../../../../lambda-term.md) for the successor and zero test are

$$
\mathsf{Succ}=\lambda n f x.f(nfx),\qquad \mathsf{Zero}=\lambda n.n(\lambda z.\mathsf F)\mathsf T.
$$

Direct [beta reduction](../../../../../beta-reduction.md) gives $\mathsf{Succ}\,c_n\equiv_\beta c_{n+1}$, and the [Church numeral zero test](../../../../../church-numeral-zero-test.md) returns $\mathsf T$ exactly at zero. For the predecessor, use the [Church pair](../../../../../church-pair.md) operations

$$
\mathsf{Pair}=\lambda abp.pab,\quad \mathsf{Fst}=\lambda p.p\mathsf T,\quad\mathsf{Snd}=\lambda p.p\mathsf F,
$$

and set

$$
\mathsf{Step}=\lambda p.\mathsf{Pair}(\mathsf{Succ}(\mathsf{Fst}\,p))(\mathsf{Fst}\,p),\qquad \boxed{\mathsf{Pred}=\lambda n.\mathsf{Snd}\bigl(n\mathsf{Step}(\mathsf{Pair}\,c_0\,c_0)\bigr).}
$$

After $j$ iterations this pair holds $(c_j,c_{\max(j-1,0)})$: the initial pair gives the case $j=0$, and one step moves the old first coordinate into the second and increments the first. This proves the predecessor equation, including $\mathsf{Pred}\,c_0\equiv_\beta c_0$.

A total [function](../../../../../function-split.md) is a [lambda-definable function](../../../../../lambda-definable-function.md) when a closed [lambda term](../../../../../lambda-term.md) sends each tuple of numerals to the numeral of its value. Suppose $G,H$ represent total $g,h$, and

$$
r(\mathbf x,0)=g(\mathbf x),\qquad r(\mathbf x,j+1)=h(\mathbf x,j,r(\mathbf x,j)).
$$

For [lambda definition of primitive recursion by pair iteration](../../../../../lambda-definition-of-primitive-recursion-by-pair-iteration.md), put

$$
\mathsf{Step}_{\mathbf x}=\lambda p.\mathsf{Pair}(\mathsf{Succ}(\mathsf{Fst}\,p))(H\mathbf x(\mathsf{Fst}\,p)(\mathsf{Snd}\,p)),\qquad R=\lambda\mathbf x n.\mathsf{Snd}\bigl(n\mathsf{Step}_{\mathbf x}(\mathsf{Pair}\,c_0\,(G\mathbf x))\bigr).
$$

On numeral inputs, induction gives the pair $(c_j,c_{r(\mathbf x,j)})$ after $j$ iterations. The base case is the equation for $G$, and the induction step is exactly the equation for $H$. Hence $R$ represents $r$, proving **closure of total lambda-definable functions under primitive recursion**.

For [unbounded minimization](../../../../../mu-operator.md), the careful closure statement is partial: if total $f(\mathbf x,n)$ is lambda-definable, then

$$
\mu n\,[f(\mathbf x,n)=0]
$$

is a [lambda-definable partial function](../../../../../lambda-definable-partial-function.md), defined when a zero exists and otherwise undefined. It need not be total. With $F$ representing $f$, use a [fixed-point combinator](../../../../../fixed-point-combinator.md) to define

$$
\mathsf{Search}=Y(\lambda s\mathbf x n.\mathsf{Zero}(F\mathbf x n)\,n\,(s\mathbf x(\mathsf{Succ}\,n))),\qquad U=\lambda\mathbf x.\mathsf{Search}\,\mathbf x\,c_0.
$$

Each test terminates because $f$ is total. [Normal-order beta reduction](../../../../../normal-order-beta-reduction.md) chooses the return branch at the first zero and does not evaluate the discarded branch. If there is no zero, the required head computation passes through tests for all $n$, never exposing a numeral; [standardization theorem for beta reduction](../../../../../standardization-theorem-for-beta-reduction.md) rules out a hidden numeral reduct. For partial $f$, the usual [mu operator](../../../../../mu-operator.md) is defined only if all earlier tests terminate and the successful test is zero. This stronger partial closure requires representatives that diverge on undefined inputs, or an explicit strict evaluator; the weaker condition of producing no numeral on undefined inputs alone must not be used as a test for convergence.

The zero function, successor, and projections have immediate numeral representations; [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md) is implemented by substitution on total inputs. Thus every [primitive recursive function](../../../../../primitive-recursive-function.md) is lambda-definable. The [Kleene normal form theorem](../../../../../kleene-normal-form-theorem.md) writes every [partial recursive function](../../../../../computable-function.md) as a total primitive-recursive decoding after a single minimization of a total primitive-recursive computation-history predicate. The search above consequently represents every [partial recursive function](../../../../../computable-function.md), diverging when no successful history exists. Conversely a machine can effectively enumerate the [beta reductions](../../../../../beta-reduction.md) of a fixed representing [lambda term](../../../../../lambda-term.md) on numeral inputs until it finds a [Church numeral](../../../../../church-numeral.md); distinct numerals cannot be beta-equivalent by the [Church-Rosser theorem](../../../../../church-rosser-theorem.md). It computes exactly the represented partial function. Therefore **lambda-definable partial functions are precisely partial computable functions, and the total ones are precisely total computable functions**.

This also gives the full partial minimization closure without assuming that an arbitrary weak representative diverges on every undefined input. Run its effective numeral evaluator successively at $n=0,1,2,\ldots$; stop at the first zero, and run forever if an earlier evaluation fails to terminate or no zero is found. This is exactly the sequential-domain convention for the [mu operator](../../../../../mu-operator.md). The resulting [partial computable function](../../../../../computable-function.md) has a lambda representation by the construction just proved. Thus **partial lambda-definable functions are closed under partial minimization**; a minimized function belongs to the total family only when the required successful search exists for every input.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
