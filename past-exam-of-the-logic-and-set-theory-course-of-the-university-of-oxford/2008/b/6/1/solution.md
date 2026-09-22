<h1 id="b/6/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Kuratowski ordered pair](../../../../../kuratowski-ordered-pair.md)

$$
\langle a,b\rangle=\{\{a\},\{a,b\}\}.
$$

The [axiom of pairing](../../../../../axiom-of-pairing.md) first produces $\{a\}$ by pairing $a$ with itself, then $\{a,b\}$, and then the pair of these two [sets](../../../../../set-split.md). The [axiom of extensionality](../../../../../axiom-of-extensionality.md) supplies the usual uniqueness of each specified [set](../../../../../set-split.md). In particular, no use of [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) is needed to construct a single [ordered pair](../../../../../ordered-pair.md) from two given [sets](../../../../../set-split.md).

To recover the coordinates from $P=\langle a,b\rangle$, observe that

$$
\bigcap P=\{a\},\qquad \bigcup P=\{a,b\}.
$$

The first [equality](../../../../../equality-mathematics.md) recovers $a$. Once $a$ is known, the second recovers $b$: if its [union](../../../../../set-union.md) is the [singleton](../../../../../singleton-mathematics.md) $\{a\}$ then $b=a$, and otherwise $b$ is its unique element different from $a$. Hence [equality](../../../../../equality-mathematics.md) of two encoded pairs forces [equality](../../../../../equality-mathematics.md) of both coordinates, including the degenerate case $a=b$.

**The first [ordered triple](../../../../../ordered-triple.md) encoding works.** If

$$
\langle a,\langle b,c\rangle\rangle=\langle a',\langle b',c'\rangle\rangle,
$$

[injectivity](../../../../../injective-function.md) of the [ordered pair](../../../../../ordered-pair.md) construction first gives $a=a'$ and $\langle b,c\rangle=\langle b',c'\rangle$, and a second application gives $b=b'$ and $c=c'$. The construction uses only two successive [ordered pair](../../../../../ordered-pair.md) constructions, so is a [set](../../../../../set-split.md) as well.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [6](../../6.md)
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
