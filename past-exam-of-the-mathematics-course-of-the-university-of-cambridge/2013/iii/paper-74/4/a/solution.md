<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A decidable $B$ has injective action maps. First prove that evaluation at $1$ distinguishes equivariant functions. Suppose $f(1,a)=g(1,a)$ for every $a$. Fix $m\in M$ and choose $p,q$ with $pmq=p$. For each $a$, equivariance gives

$$
p\cdot f(m,a)=f(pm,p\cdot a)
=f(pm,pm\cdot(q\cdot a))
=pm\cdot f(1,q\cdot a).
$$

The same equation holds for $g$, so these values agree. Cancel the injective action of $p$ on $B$ to obtain $f(m,a)=g(m,a)$. Hence $f=g$. This proves the hinted contrapositive and, more precisely, injectivity of the trace map $f\mapsto(a\mapsto f(1,a))$.

Now suppose $m\cdot f=m\cdot g$ in the exponential. Evaluating this equality at $(1,m\cdot a)$ gives

$$
f(m,m\cdot a)=g(m,m\cdot a),\qquad
m\cdot f(1,a)=m\cdot g(1,a).
$$

Cancel the action of $m$ on $B$. The trace maps agree, so the preceding argument gives $f=g$. Every action map on $B^A$ is therefore injective. By the introductory criterion, **$B^A$ is decidable whenever $B$ is** under the specified [monoid](../../../../../../monoid.md) condition. Neither cancellation in $M$ nor injectivity of its action on $A$ is assumed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
