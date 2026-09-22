<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**[Rolle's theorem](../../../../../../rolle-theorem.md)** states that a [continuous function](../../../../../../continuous-function.md) $g:[u,v]\to\mathbb R$ with $u<v$, [differentiable](../../../../../../differentiable-function.md) on $(u,v)$, and satisfying $g(u)=g(v)$ has $g'(c)=0$ for some $c\in(u,v)$.

Fix $x>0$ and set $r=(\sqrt{1+x}-1)/x$. The [function](../../../../../../function-split.md)

$$
g(t)=\sqrt{1+t}-1-rt,\qquad0\leq t\leq x,
$$

is [continuous](../../../../../../continuous-function.md) and [differentiable](../../../../../../differentiable-function.md) as required, and $g(0)=g(x)=0$. By [Rolle's theorem](../../../../../../rolle-theorem.md), some $c\in(0,x)$ satisfies

$$
0=g'(c)=\frac1{2\sqrt{1+c}}-r.
$$

Since $c>0$, this gives $r<1/2$. Multiplying by $x>0$ and adding one proves the strict [square root](../../../../../../square-root.md) bound

$$
\boxed{\sqrt{1+x}<1+x/2\qquad(x>0).}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
