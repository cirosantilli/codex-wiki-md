<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An arrival at $s\le t$ remains active with probability $1-(t-s)$ when $0\le t-s\le1$, and zero later. By [Poisson thinning](../../../../../../poisson-thinning.md), the detector count is Poisson with mean

$$
m(t)=\lambda\int_{\max(0,t-1)}^t[1-(t-s)]\,ds
=\begin{cases}\lambda(t-t^2/2),&0\le t\le1,\\ \lambda/2,&t\ge1.\end{cases}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
