<h1 id="b/7/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Cantor-Schröder-Bernstein theorem](../../../../../cantor-schroder-bernstein-theorem.md) states that [injections](../../../../../injective-function.md) $f:A\to B$ and $g:B\to A$ imply the existence of a [bijection](../../../../../bijection.md) $A\to B$. Here is the injection-chain [formal proof](../../../../../formal-proof.md), so no fixed-point theorem is needed. Define

$$
A_0=A\setminus g(B),\qquad A_{n+1}=g(f(A_n)),\qquad C=\bigcup_{n<\omega}A_n,
$$

and [set](../../../../../set-split.md)

$$
h(a)=\begin{cases}f(a),&a\in C,\\ g^{-1}(a),&a\notin C.\end{cases}
$$

The second branch is defined because $a\notin C$ implies $a\notin A_0$, hence $a\in g(B)$, and the inverse there is unique by [injectivity](../../../../../injective-function.md) of $g$. Each branch is [injective](../../../../../injective-function.md). A collision between branches would have $f(c)=g^{-1}(a)$ with $c\in C$ and $a\notin C$, implying $a=g(f(c))\in C$, a contradiction. Thus $h$ is [injective](../../../../../injective-function.md).

For [surjectivity](../../../../../surjective-function.md) let $b\in B$. If $g(b)\notin C$, then $h(g(b))=b$. If $g(b)\in C$, it is not in $A_0$, so it belongs to some $A_{n+1}=g(f(A_n))$. There is $a\in A_n$ with $g(b)=g(f(a))$; [injectivity](../../../../../injective-function.md) of $g$ gives $b=f(a)=h(a)$. This proves that $h$ is a [bijection](../../../../../bijection.md) and completes the theorem without the [axiom of choice](../../../../../axiom-of-choice.md).

For the comparison of [cardinalities](../../../../../cardinality.md) take the [power set](../../../../../power-set.md) of $\omega$ as the reference [set](../../../../../set-split.md). Its [cardinality](../../../../../cardinality.md) is by definition

$$
\boxed{|\mathcal P(\omega)|=2^{\aleph_0}.}
$$

The remaining parts give explicit [injections](../../../../../injective-function.md) or [bijections](../../../../../bijection.md) comparing each requested [set](../../../../../set-split.md) with this one.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
