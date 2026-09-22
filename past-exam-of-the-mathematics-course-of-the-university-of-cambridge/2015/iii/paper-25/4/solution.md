<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We use [untyped lambda calculus](../../../../../untyped-lambda-calculus.md) and [normal-order beta reduction](../../../../../normal-order-beta-reduction.md). The [Church numeral](../../../../../church-numeral.md) for $n$ is $\overline n=\lambda s.\lambda z.s^n z$. A [lambda term](../../../../../lambda-term.md) represents a partial [function](../../../../../function-split.md) if on numeral inputs it has the correct numeral normal form exactly when the [function](../../../../../function-split.md) is defined. We use a [lambda simulation of a Turing machine](../../../../../lambda-simulation-of-a-turing-machine.md); this also ensures that undefined computations do not accidentally produce an output through an ignored argument.

First all total [primitive recursive functions](../../../../../primitive-recursive-function.md) are lambda-definable. The [initial functions of recursion theory](../../../../../initial-function-of-recursion-theory.md) are represented by

$$
\mathsf{Zero}=\lambda x.\overline0,\qquad\mathsf{Succ}=\lambda n s z.s(nsz),\qquad\mathsf{Proj}_j=\lambda x_1\cdots x_k.x_j.
$$

Composition is obtained by substitution of representing terms. For [primitive recursion](../../../../../primitive-recursion.md) use [Church pairs](../../../../../church-pair.md):

$$
\mathsf{Pair}=\lambda a b p.pab,\qquad\mathsf{Fst}=\lambda p.p(\lambda a b.a),\qquad\mathsf{Snd}=\lambda p.p(\lambda a b.b).
$$

If $G,H$ represent the total [functions](../../../../../function-split.md) in $f(0,\vec x)=g(\vec x)$ and $f(i+1,\vec x)=h(i,f(i,\vec x),\vec x)$, define

$$
\begin{aligned}
\mathsf{Step}_{\vec x}&=\lambda p.\mathsf{Pair}\bigl(\mathsf{Succ}(\mathsf{Fst}\,p)\bigr)\bigl(H(\mathsf{Fst}\,p)(\mathsf{Snd}\,p)\vec x\bigr),\\
F&=\lambda n\vec x.\mathsf{Snd}\bigl(n\,\mathsf{Step}_{\vec x}\,(\mathsf{Pair}\,\overline0\,(G\vec x))\bigr).
\end{aligned}
$$

After $i$ iterations the pair has components $\overline i,\overline{f(i,\vec x)}$. Thus the [Church numeral](../../../../../church-numeral.md) $\overline n$ executes exactly the required $n$ recursion steps. Since these [functions](../../../../../function-split.md) are total on numeral inputs, substitution for composition causes no undefined-argument issue.

Now fix a deterministic [Turing machine](../../../../../turing-machine.md) computing the given [partial computable function](../../../../../computable-function.md). Encode a configuration by its finite control state and two [natural numbers](../../../../../natural-number.md) for the tape portions on the two sides of the head, allowing blank bits beyond the finite nonblank tape. For the [two-stack encoding of a Turing tape](../../../../../two-stack-encoding-of-a-turing-tape.md) with a binary alphabet, let $L$ have the immediately-left cell as its low bit and $R$ have the current cell as its low bit. Reading and removing a bit use remainder and quotient by two. If the machine writes $w\in\{0,1\}$, the updates are

$$
\begin{array}{ll}
\text{move right:}&L'=2L+w,\quad R'=\lfloor R/2\rfloor,\\
\text{move left:}&L'=\lfloor L/2\rfloor,\quad R'=4\lfloor R/2\rfloor+2w+(L\bmod2).
\end{array}
$$

The new state is obtained from a finite transition table. These operations, the initial configuration, the halting test, and output decoding are total [primitive recursive functions](../../../../../primitive-recursive-function.md) on configuration codes. For instance parity alternates by [primitive recursion](../../../../../primitive-recursion.md), and the quotient by two satisfies $q(0)=0$, $q(n+1)=q(n)+(n\bmod2)$. A fixed finite alphabet can be handled by the same stack construction in a larger base. Choose a standard delimited input and output convention, for example unary words in a finite tape alphabet with a distinct blank symbol. Initialization is [primitive recursive](../../../../../primitive-recursive-function.md). On a halting configuration the output is a finite word; decoding can be implemented by a bounded scan of the encoded tape, with a default output for malformed words. This is total [primitive recursive](../../../../../primitive-recursive-function.md) and introduces no additional unbounded search. Use nested [Church pairs](../../../../../church-pair.md) to carry the three fields, and the preceding [primitive recursive](../../../../../primitive-recursive-function.md) representations to obtain [lambda terms](../../../../../lambda-term.md) $\mathsf{Init},\mathsf{Next},\mathsf{Halt},\mathsf{Out}$.

Represent [Church Booleans](../../../../../church-boolean.md) by $\mathsf{True}=\lambda a b.a$ and $\mathsf{False}=\lambda a b.b$. A [Church numeral zero test](../../../../../church-numeral-zero-test.md) is $\mathsf{IsZero}=\lambda n.n(\lambda z.\mathsf{False})\mathsf{True}$. Use a numerical test equal to zero on halting configurations and one otherwise; applying this zero test gives the required Boolean halting test. With the [fixed-point combinator](../../../../../fixed-point-combinator.md)

$$
Y=\lambda f.(\lambda x.f(xx))(\lambda x.f(xx)),\qquad YH\equiv_\beta H(YH),
$$

put

$$
\mathsf{Run}=Y\bigl(\lambda r c.(\mathsf{Halt}\,c)(\mathsf{Out}\,c)(r(\mathsf{Next}\,c))\bigr),\qquad F=\lambda\vec x.\mathsf{Run}(\mathsf{Init}\,\vec x).
$$

Normal-order reduction evaluates the halting test on the current configuration. If it is true, it selects the output branch without evaluating the recursive branch. Otherwise it advances the configuration and repeats. Induction on the number of machine steps shows that a computation halting with output $y$ makes $F\overline{x_1}\cdots\overline{x_k}$ reduce to $\overline y$.

If the machine never halts, the [normal-order beta reduction](../../../../../normal-order-beta-reduction.md) repeatedly takes the recursive branch. Each individual configuration transition and test terminates, but there is always another required transition; hence the reduction never reaches a normal form. The [normal-order normalization theorem](../../../../../normal-order-normalization-theorem.md) says that a [lambda term](../../../../../lambda-term.md) with a [beta-normal form](../../../../../beta-normal-form.md) is normalized by [normal-order beta reduction](../../../../../normal-order-beta-reduction.md). Therefore in the nonhalting case there is no numeral normal form at all. We have proved

$$
\boxed{f(\vec x)\downarrow=y\quad\Longleftrightarrow\quad F\overline{x_1}\cdots\overline{x_k}\text{ has beta-normal form }\overline y.}
$$

[Confluence of beta reduction](../../../../../church-rosser-theorem.md) ensures uniqueness of the resulting numeral. This handles genuinely partial computations. Simply composing terms for partial subcomputations would need extra care, because lambda reduction can discard an unevaluated argument.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
