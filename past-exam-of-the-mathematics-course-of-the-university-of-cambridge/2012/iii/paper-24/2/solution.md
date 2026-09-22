<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [function in intension](../../../../../function-in-intension.md) is a finite description of a computation, such as a program or a formal construction expression. A [function in extension](../../../../../function-in-extension.md) is the resulting input-output map, including its domain if it is partial. Different descriptions may have the same extension: the programs that return $x$ directly and that compute $x+0$ describe the same [function](../../../../../function-split.md). Finite descriptions have [Gödel numbers](../../../../../godel-number.md); equality of the resulting [partial computable functions](../../../../../computable-function.md) is a separate semantic question.

The [primitive recursive functions](../../../../../primitive-recursive-function.md) are the smallest class of numerical [functions](../../../../../function-split.md) containing the [zero functions](../../../../../zero-function.md), the [successor function](../../../../../successor-function.md) and all [projection functions](../../../../../projection-function.md), and closed under [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md) and [primitive recursion](../../../../../primitive-recursion.md). More explicitly, from $g:\mathbb N^k\to\mathbb N$ and $h:\mathbb N^{k+2}\to\mathbb N$ the latter operation forms

$$
f(\mathbf x,0)=g(\mathbf x),\qquad f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n)).
$$

For [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md), an $m$-ary $g$ and $k$-ary $h_1,\ldots,h_m$ give $g(h_1(\mathbf x),\ldots,h_m(\mathbf x))$. Zero functions of all allowed arities can be included, with nullary zero included if arity $0$ is part of the coding convention. Every resulting [function](../../../../../function-split.md) is total: the initial functions are total, [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md) preserves totality, and [mathematical induction](../../../../../mathematical-induction.md) on $n$ verifies totality of [primitive recursion](../../../../../primitive-recursion.md). Applying [structural induction for primitive recursive functions](../../../../../structural-induction-for-primitive-recursive-functions.md) then covers all construction expressions.

Use a fixed effective [Gödel numbering](../../../../../godel-numbering.md) of finite tagged construction trees with decidable decoding. A node is tagged as zero, successor, projection, composition, or recursion. The [primitive recursive syntax and arity checking](../../../../../primitive-recursive-syntax-and-arity-checking.md) algorithm first checks that the input decodes as a finite tree, then works upwards from its leaves. A projection tag $(k,j)$ is legal exactly when $1\leq j\leq k$, with output arity $k$. A composition node declares its output arity $k$ and is legal when its outer child has arity $m$, there are exactly $m$ inner children, and each has arity $k$; its arity is $k$. The declared arity also handles the case $m=0$. A recursion node is legal when its base child has arity $k$ and its step child has arity $k+2$; its arity is $k+1$. Zero and successor tags have their declared arities. Ill-formed nodes are rejected. The process terminates because there are only finitely many nodes. Thus, for each fixed $i$,

$$
\boxed{D_i=\{p:p\text{ is a valid primitive-recursive construction of arity }i\}\text{ is decidable}.}
$$

This is a syntactic assertion about [functions in intension](../../../../../function-in-intension.md). It does not assert that arbitrary machine indices computing [primitive recursive functions](../../../../../primitive-recursive-function.md) form a decidable set. That extensional property is nontrivial, hence undecidable by [Rice theorem](../../../../../rice-s-theorem.md). For an explicit reduction, given a program $e$ construct a program that, on every input, waits for $\varphi_e(e)$ to halt and then returns $0$. Its extension is a [primitive recursive function](../../../../../primitive-recursive-function.md) if $e\in K$, and otherwise is nowhere defined and so is not a [primitive recursive function](../../../../../primitive-recursive-function.md). A decision procedure for this latter semantic set would decide the [diagonal halting set](../../../../../diagonal-halting-set.md).

Enumerate the decidable syntax set $D_1$ in increasing code order as $p_0,p_1,\ldots$. There are infinitely many such descriptions; iterating successor after a unary zero expression already supplies infinitely many. Let $F_p$ be the extension of a valid construction and define

$$
U(n,x)=F_{p_n}(x),\qquad \boxed{d(n)=U(n,n)+1.}
$$

To compute $U$, find $p_n$ by the syntax test and interpret its finite construction tree. Evaluate [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md) by evaluating the children, and evaluate [primitive recursion](../../../../../primitive-recursion.md) by the prescribed finite loop of length equal to its final input. Termination follows from the totality argument above, so $U$ and $d$ are [total computable functions](../../../../../total-computable-function.md).

If $d$ were a unary [primitive recursive function](../../../../../primitive-recursive-function.md), some construction $p_j$ would have extension $d$. Then the [diagonal argument](../../../../../diagonal-argument.md) gives

$$
d(j)=F_{p_j}(j)+1=d(j)+1,
$$

which is impossible. **The displayed $d$ is total and computable but not primitive recursive.** Repetitions of extensions in the enumeration cause no problem: every possible extension is represented, which is all the [diagonal argument](../../../../../diagonal-argument.md) needs. The same argument shows that the two-variable interpreter $U$ cannot itself be [primitive recursive](../../../../../primitive-recursive-function.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
