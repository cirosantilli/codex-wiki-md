<h1 id="b/4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $h:\omega\hookrightarrow X$ is an [injection](../../../../../../injective-function.md). Shift its image by defining

$$
g(h(n))=h(n+1),\qquad g(x)=x\quad(x\notin h[\omega]).
$$

The two pieces have disjoint images, so $g$ is injective, but $h(0)$ is omitted. Thus $g$ is not surjective.

Conversely, let $g:X\to X$ be an [injection](../../../../../../injective-function.md) which omits some $a\in X$. The [natural-number recursion theorem](../../../../../../natural-number-recursion-theorem.md) defines $h(0)=a$, $h(n+1)=g(h(n))$. If $h(m)=h(n)$ with $m<n$, repeated injectivity cancels $m$ iterations and gives $a=g^{n-m}(a)$, putting $a$ in the image of $g$, a contradiction. Hence $h$ is injective. Therefore

$$
\boxed{\omega\preceq X\iff X\text{ admits an injective nonsurjective self-map}.}
$$

Choosing one witness $a$ from a single known nonempty set uses no [axiom of choice](../../../../../../axiom-of-choice.md). This is the [Dedekind-infinite characterization](../../../../../../dedekind-infinite-characterization.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [B](../../../../b.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
