<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the intended [module](../../../../module-mathematics.md), index a [basis](../../../../basis.md) by $v_k=a_{l-2k}$ for $0\le k\le l$, and use

$$
Hv_k=(l-2k)v_k,\qquad fv_k=v_{k+1},\qquad ev_k=k(l+1-k)v_{k-1},
$$

with $v_{-1}=v_{l+1}=0$. This makes the [basis](../../../../basis.md) endpoints distinct, identifies the lowering operator, and includes its missing raising action at $k=l$. These are the necessary indexing corrections to the printed display. The same definition for $l=0$ supplies the trivial [module](../../../../module-mathematics.md) needed for classification.

Directly on $v_k$,

$$
\begin{aligned}
[H,f]v_k&=-2fv_k,\\
[H,e]v_k&=2ev_k,\\
[e,f]v_k&=((k+1)(l-k)-k(l+1-k))v_k=(l-2k)v_k.
\end{aligned}
$$

These hold at the endpoints too, proving the three defining $\mathfrak{sl}_2$ relations. Finally

$$
\begin{aligned}
\Delta v_k
&=\bigl(4k(l+1-k)+(l-2k)^2+2(l-2k)\bigr)v_k\\
&=\boxed{l(l+2)v_k.}
\end{aligned}
$$

Thus the [Casimir element](../../../../casimir-element.md) acts by that scalar on the whole [module](../../../../module-mathematics.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the representation theory of semisimple Lie algebras course of the University of Oxford](../../../split.md)
5. [Representation theory of semisimple Lie algebras course of the University of Oxford](../../../../representation-theory-of-semisimple-lie-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
