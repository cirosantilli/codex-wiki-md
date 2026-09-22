<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write points of $U$ as $(x,y)$ with $x>0$. For $h>0$, translate $u$ into the domain by

$$
u^h(x,y)=u(x+h,y),
\qquad x>-h.
$$

Continuity of translations in $L^p$ applied to $u,D_xu,D_yu$ gives

$$
u^h|_U\longrightarrow u
\quad\text{in }W^{1,p}(U)
$$

as $h\downarrow0$. Choose a standard [mollifier](../../../../../../mollifier.md) $\rho_\varepsilon$ supported in a ball of radius $\varepsilon<h/2$. For $(x,y)\in U$, the convolution

$$
u_{h,\varepsilon}(x,y)=(\rho_\varepsilon*u^h)(x,y)
$$

only samples points with first coordinate greater than $-h$, so it is well-defined and smooth throughout $U$. The approximation-to-the-identity theorem, applied also to each [weak derivative](../../../../../../weak-derivative.md), allows $\varepsilon(h)<h/2$ to be chosen so that

$$
\|u_{h,\varepsilon(h)}-u^h\|_{W^{1,p}(U)}<h.
$$

Taking $h=1/j$ and using the [triangle inequality](../../../../../../triangle-inequality.md) proves the [density of smooth functions in a Sobolev space](../../../../../../density-of-smooth-functions-in-a-sobolev-space.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
