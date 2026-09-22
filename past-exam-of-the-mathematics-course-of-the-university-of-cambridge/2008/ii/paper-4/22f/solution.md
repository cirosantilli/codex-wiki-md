<h1 id="22f/solution">Solution</h1>

↑ **Parent:** [22F](../22f.md)

Let $d=\inf_{v\in V}\|f-v\|$ and choose $v_n\in V$ with $\|f-v_n\|\to d$. The parallelogram identity gives

$$
\|v_n-v_m\|^2
=2\|f-v_n\|^2+2\|f-v_m\|^2-4\left\|f-\frac{v_n+v_m}{2}\right\|^2
\leq2\|f-v_n\|^2+2\|f-v_m\|^2-4d^2\longrightarrow0.
$$

Completeness and closedness give $v_n\to v\in V$, attaining the distance. Put $w=f-v$. For $u\in V$ and real $t$, minimality gives $\|w-tu\|^2\geq\|w\|^2$, so $\operatorname{Re}\langle w,u\rangle=0$. In a complex [Hilbert space](../../../../../hilbert-space-split.md), also replace $u$ with $iu$ to get the imaginary part zero. Therefore

$$
\boxed{f=v+w,\qquad v\in V,\quad w\perp V.}
$$

The decomposition is unique since $V\cap V^\perp=\{0\}$. This proves the required [orthogonal projection](../../../../../orthogonal-projection.md) result rather than assuming it before the averaging argument.

## ↑ Ancestors (10)

1. [22F](../22f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
