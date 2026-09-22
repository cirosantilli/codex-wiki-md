<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Sobolev space](../../../../../sobolev-space-split.md) and [norm](../../../../../norm.md) are

$$
H^1(a,b)=\{v\in L^2(a,b):v'\text{ exists weakly and belongs to }L^2(a,b)\},\qquad
\|v\|_{H^1}^2=\|v\|_2^2+\|v'\|_2^2.
$$

In one dimension these functions have continuous representatives and well-defined endpoint traces. [integration by parts](../../../../../integration-by-parts.md) gives the weak problem: find $u\in H^1(a,b)$ such that $a(u,v)=\ell(v)$ for all $v\in H^1(a,b)$, where

$$
a(u,v)=\int_a^b(u'v'+x^2uv)\,dx+u(a)v(a)+u(b)v(b),\qquad
\ell(v)=\int_a^bfv\,dx+A v(a)+B v(b).
$$

Indeed the integration boundary term is $-u'(b)v(b)+u'(a)v(a)$; substituting $u'(a)=u(a)-A$ and $u'(b)=B-u(b)$ gives the two positive boundary terms on the left.

If $0\notin[a,b]$, put $m=\min_{[a,b]}x^2>0$. Then $a(v,v)\geq\|v'\|_2^2+m\|v\|_2^2\geq\min(1,m)\|v\|_{H^1}^2$. If $0\in[a,b]$, the supplied [trace](../../../../../matrix-trace.md) inequality gives

$$
\|v\|_{H^1}^2\leq(1+\widetilde c)\bigl(\|v'\|_2^2+v(a)^2+v(b)^2\bigr)\leq(1+\widetilde c)a(v,v).
$$

Thus the form is **coercive in both cases**. The [trace](../../../../../matrix-trace.md) theorem and boundedness of $x^2$ give continuity of $a$ and $\ell$, and the [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) gives [existence](../../../../../existence.md) and [uniqueness](../../../../../uniqueness.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
