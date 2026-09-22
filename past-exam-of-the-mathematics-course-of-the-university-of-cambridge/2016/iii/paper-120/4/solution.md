<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For (1)(a), a [primitive recursive function](../../../../../primitive-recursive-function.md) is obtained by a finite construction from the [zero function](../../../../../zero-function.md), [successor function](../../../../../successor-function.md) and [projection functions](../../../../../projection-function.md), using [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md) and [primitive recursion](../../../../../primitive-recursion.md). The recursion rule, with parameters $\mathbf x$, is

$$
f(\mathbf x,0)=g(\mathbf x),\qquad
f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n)).
$$

Here $g,h$ have already been constructed. All these [functions](../../../../../function-split.md) are total on nonnegative [integers](../../../../../integer.md): the initial functions are total, composition preserves totality, and ordinary [mathematical induction](../../../../../mathematical-induction.md) proves totality of each recursion.

For (1)(b), use a shifted [hyperoperation](../../../../../hyperoperation.md) sequence, beginning with [addition](../../../../../addition.md). Define

$$
H_0(a,0)=a,\qquad H_0(a,b+1)=S(H_0(a,b)),
$$

and, for each fixed $r\geq0$, define

$$
H_{r+1}(a,0)=c_r,\qquad
H_{r+1}(a,b+1)=H_r(a,H_{r+1}(a,b)),
\qquad c_0=0,\quad c_r=1\ (r\geq1).
$$

The first three members are therefore **addition, multiplication and exponentiation**:

$$
\boxed{H_0(a,b)=a+b,\qquad H_1(a,b)=ab,\qquad H_2(a,b)=a^b.}
$$

The [exponentiation](../../../../../exponentiation.md) convention includes $a^0=1$, hence $0^0=1$. The next member iterates [exponentiation](../../../../../exponentiation.md), with $H_3(a,0)=1$; there is no need for an exceptional domain restriction at $a=0$.

For (1)(c), $H_0$ is a [primitive recursive function](../../../../../primitive-recursive-function.md) by its displayed recursion. If $H_r$ is a [primitive recursive function](../../../../../primitive-recursive-function.md), then

$$
g_r(a)=c_r,\qquad h_r(a,b,z)=H_r(a,z)
$$

are [primitive recursive functions](../../../../../primitive-recursive-function.md), using constants, [projection functions](../../../../../projection-function.md) and [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md). [Primitive recursion](../../../../../primitive-recursion.md) applied to $g_r,h_r$ gives $H_{r+1}$. [Mathematical induction](../../../../../mathematical-induction.md) on the fixed rank $r$ proves **every member of the sequence is primitive recursive**. This does not assert that the joint three-variable evaluator $(r,a,b)\mapsto H_r(a,b)$ is a [primitive recursive function](../../../../../primitive-recursive-function.md).

For (2), **as written, the answer is no**: the [empty set](../../../../../empty-set.md) $X=\varnothing$ is [semidecidable](../../../../../recursively-enumerable-set.md), whereas a [total computable function](../../../../../total-computable-function.md) from $\mathbb N$ to $\mathbb N$ always has a nonempty range. This is the only obstruction. To prove the stronger useful statement, suppose $X$ is a nonempty [computably enumerable set](../../../../../recursively-enumerable-set.md) and choose $x_0\in X$. Fix a [Turing machine](../../../../../turing-machine.md) which halts exactly on the inputs in $X$. Its [bounded halting predicate](../../../../../bounded-halting-predicate.md)

$$
B(x,t)=1\quad\Longleftrightarrow\quad
\text{that machine halts on input }x\text{ within }t\text{ steps}
$$

is [primitive recursive](../../../../../primitive-recursive-function.md): encode configurations arithmetically, iterate its total single-step operation $t$ times by [primitive recursion](../../../../../primitive-recursion.md), and check the halt state. A halted configuration is kept fixed. This is a bounded simulation, not unbounded waiting.

Fix a [primitive recursive pairing function](../../../../../primitive-recursive-pairing-function.md) $\langle x,t\rangle$ with [primitive recursive](../../../../../primitive-recursive-function.md) inverse coordinate functions. For example, the Cantor pairing function has inverses obtained by [bounded minimization](../../../../../bounded-minimization.md). Define

$$
f(\langle x,t\rangle)=
\begin{cases}x,&B(x,t)=1,\\x_0,&B(x,t)=0.\end{cases}
$$

The two coordinate functions, the bounded predicate, and the finite case distinction are [primitive recursive functions](../../../../../primitive-recursive-function.md), so $f$ is a [primitive recursive function](../../../../../primitive-recursive-function.md). Its values always lie in $X$. Conversely, if $x\in X$, its computation halts within some finite $t$, and $f(\langle x,t\rangle)=x$. Thus

$$
\boxed{X\ne\varnothing\text{ and }X\text{ semidecidable}
\ \Longrightarrow\ \exists f\text{ primitive recursive with }\operatorname{ran}(f)=X.}
$$

The range need not be a [computable set](../../../../../computable-set.md); deciding whether a value occurs anywhere in this total enumeration is an unbounded search.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
