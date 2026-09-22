# Primitive recursive pairing function

↑ **Parent:** [Pairing function](pairing-function.md)

A [primitive recursive pairing function](primitive-recursive-pairing-function.md) is a [pairing function](pairing-function.md) whose encoding [function](function-split.md) and both coordinate [functions](function-split.md) of its [inverse function](inverse-function.md) are [primitive recursive functions](primitive-recursive-function.md). Thus the [bijection](bijection.md) can be used in either direction inside a construction by [primitive recursion](primitive-recursion.md) and [function composition in recursion theory](function-composition-in-recursion-theory.md). A decoder that is merely a [computable function](computable-function.md) would not establish this stronger closure property. Sutner's definition of a primitive recursive pairing system explicitly includes the decoding [functions](function-split.md); his more general systems need only be [injective](injective-function.md), whereas a [pairing function](pairing-function.md) here is a [bijection](bijection.md).[Klaus Sutner, Primitive Recursion, slide 9: primitive recursive encoding and unpairing functions](https://www.cs.cmu.edu/~cdm/resources/02-coding.pdf)

The [Cantor pairing function](cantor-pairing-function.md) is a [primitive recursive pairing function](primitive-recursive-pairing-function.md). For its encoding, construct the [triangular numbers](triangular-number.md) directly by [primitive recursion](primitive-recursion.md):

$$
T(0)=0,\qquad T(s+1)=T(s)+s+1,\qquad \pi(x,y)=T(x+y)+y.
$$

Since [addition](addition.md) is [primitive recursive](primitive-recursive-function.md), so are $T$ and $\pi$ by [primitive recursion](primitive-recursion.md) and [function composition in recursion theory](function-composition-in-recursion-theory.md). This establishes the claim without treating [division](division-mathematics.md) by two as an unexplained primitive operation.

For decoding, use [bounded minimization](bounded-minimization.md) to define

$$
s(z)=\min\{t\in\mathbb N_0:t\leq z\ \text{and}\ z<T(t+1)\}.
$$

The bound is valid for every [natural number](natural-number.md) $z$: $T(z+1)=(z+1)(z+2)/2>z$, so the candidate $t=z$ always succeeds. The search includes zero; when $z=0$, it immediately returns $s(0)=0$. If $s(z)>0$, the preceding candidate failed, which gives $T(s(z))\leq z$; when $s(z)=0$, that lower [inequality](inequality-mathematics.md) follows from $T(0)=0$. Thus this search finds exactly the diagonal in the [Cantor pairing function](cantor-pairing-function.md) inverse, with

$$
T(s(z))\leq z<T(s(z)+1).
$$

The comparison is [primitive recursive](primitive-recursive-function.md), and [bounded minimization](bounded-minimization.md) of a [primitive recursive](primitive-recursive-function.md) predicate is [primitive recursive](primitive-recursive-function.md). Therefore $s$ is a [primitive recursive function](primitive-recursive-function.md). Recover the coordinates by

$$
R(z)=z-T(s(z)),\qquad L(z)=s(z)-R(z).
$$

In constructions on the [natural numbers](natural-number.md), implement these [subtractions](subtraction.md) using the [primitive recursive](primitive-recursive-function.md) operation $a\mathbin{\dot{-}}b=\max(a-b,0)$: apply the [predecessor function](predecessor-function.md) $b$ times to $a$ by [primitive recursion](primitive-recursion.md). On these inputs it agrees with ordinary [subtraction](subtraction.md), since the diagonal [inequalities](inequality-mathematics.md) imply $0\leq R(z)\leq s(z)$. Consequently $L$ and $R$ are [primitive recursive functions](primitive-recursive-function.md), and $\pi(L(z),R(z))=z$. Zimmermann proves the relevant closure under [bounded minimization](bounded-minimization.md) and the primitive recursive character of the Cantor encoding and coordinate decoding; his convention adds the first coordinate, so its coordinates are exchanged relative to $\pi$ here.[Karl-Heinz Zimmermann, Computability Theory, §2.3, Proposition 2.26 and Propositions 2.32–2.34, printed pages 18 and 21–22](https://tore.tuhh.de/bitstream/11420/1312/1/book.pdf)

For a worked [bounded minimization](bounded-minimization.md), take $z=18$. Candidates $t=0,1,2,3,4$ give $T(t+1)=1,3,6,10,15$, none exceeding $18$. Candidate $t=5$ gives $T(6)=21>18$, so $s(18)=5$, $R(18)=3$, and $L(18)=2$. The search bound was $18$; it terminates much earlier in this example. The bound proves membership in the [primitive recursive functions](primitive-recursive-function.md); it is not a claim that scanning all candidates is the fastest implementation.

For each fixed $k\geq1$, define a [tuple](finite-tuple.md) encoder by

$$
E_1(a_1)=a_1,\qquad E_{k+1}(a_1,\ldots,a_{k+1})=\pi(E_k(a_1,\ldots,a_k),a_{k+1}).
$$

Each $E_k$ and each coordinate decoder is [primitive recursive](primitive-recursive-function.md), by finitely many applications of [function composition in recursion theory](function-composition-in-recursion-theory.md) to $\pi,L,R$. For the three-entry [tuple](finite-tuple.md) encoded as $257$, applying $R$ returns $4$, applying $L$ returns $18$, and then $L(18)=2$, $R(18)=3$. The [tuple](finite-tuple.md) length remains part of the agreed convention, as explained for a general [pairing function](pairing-function.md).

This makes [primitive recursive pairing functions](primitive-recursive-pairing-function.md) useful for encoding several evolving values as one state in [primitive recursion](primitive-recursion.md). For example, store consecutive [Fibonacci numbers](fibonacci-number.md) as $c(0)=\pi(0,1)$ and update by

$$
c(n+1)=\pi(R(c(n)),L(c(n))+R(c(n))).
$$

The codes start $2,4,8,18$, decoding to $(0,1),(1,1),(1,2),(2,3)$. Every step uses [primitive recursive](primitive-recursive-function.md) encoding, decoding and [addition](addition.md); a single numerical state therefore carries the two values needed for the next step. This is also the reason a suitable [Gödel numbering](godel-numbering.md) should permit sufficiently simple decoding: representation should preserve the class of [functions](function-split.md) being studied.

## ↑ Ancestors (6)

1. [Pairing function](pairing-function.md)
2. [Computability theory](computability-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Nonempty computably enumerable sets are primitive recursive ranges](nonempty-computably-enumerable-sets-are-primitive-recursive-ranges.md)
- [Pairing function](pairing-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-20/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-120/4/solution.md)
- [Primitive recursive pairing function](primitive-recursive-pairing-function.md)
