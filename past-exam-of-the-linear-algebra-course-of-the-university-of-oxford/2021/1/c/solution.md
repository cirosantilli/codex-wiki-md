<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Let $F$ be the common [field](../../../../field.md). The [dual map](../../../../transpose-of-a-linear-map.md) is $S'(f)=f\circ S$ for $f\in W'$, where $W'$ and $V'$ are the [dual spaces](../../../../dual-space-split.md).

First assume $S'$ is [injective](../../../../injective-function.md). If $S$ were not [surjective](../../../../surjective-function.md), its [image of a linear map](../../../../image-of-a-linear-map.md) $\operatorname{im}S$ would be a [proper vector subspace](../../../../proper-vector-subspace.md) of $W$. Choose a [basis](../../../../basis.md) $w_1,\ldots,w_r$ of $\operatorname{im}S$ and use [basis extension](../../../../basis-extension.md) to obtain a [basis](../../../../basis.md) $w_1,\ldots,w_m$ of $W$, with $r<m$. There is a [linear functional](../../../../linear-functional.md) $f\in W'$ with

$$
f(w_{r+1})=1,\qquad f(w_j)=0\quad(j\ne r+1).
$$

It is nonzero and vanishes on $\operatorname{im}S$, so $S'(f)=f\circ S=0$, contradicting [injectivity](../../../../injective-function.md). Equivalently, the [annihilator of a vector subspace](../../../../annihilator-of-a-vector-subspace.md) $\operatorname{im}S$ would give a nonzero [kernel](../../../../kernel-of-a-linear-map-split.md) for $S'$. Therefore

$$
\boxed{S'\text{ injective}\ \Longrightarrow\ S\text{ surjective}.}
$$

Now assume $S'$ is [surjective](../../../../surjective-function.md). If $0\ne v\in\ker S$, [basis extension](../../../../basis-extension.md) gives a [linear functional](../../../../linear-functional.md) $h\in V'$ with $h(v)=1$: include $v$ in a [basis](../../../../basis.md) and take its [coordinate functional](../../../../coordinate-functional.md). By [surjectivity](../../../../surjective-function.md), $h=S'(f)$ for some $f\in W'$. But

$$
1=h(v)=S'(f)(v)=f(Sv)=f(0)=0,
$$

a contradiction. Hence $\ker S=0$, which proves

$$
\boxed{S'\text{ surjective}\ \Longrightarrow\ S\text{ injective}.}
$$

## ↑ Ancestors (12)

1. [c](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the linear algebra course of the University of Oxford](../../../split.md)
5. [Linear algebra course of the University of Oxford](../../../../linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
