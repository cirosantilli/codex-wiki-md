<h1 id="31b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $t=u+iv$ and $\Phi(t)=\sinh t-t$. Since

$$
\Phi(u+iv)=\sinh u\cos v-u+i(\cosh u\sin v-v),
$$

a [steepest-descent curve](../../../../../../method-of-steepest-descent.md) through the [saddle point](../../../../../../saddle-point.md) $t=0$ lies in

$$
\boxed{\cosh u\sin v-v=0.}
$$

The saddle is cubic rather than simple:

$$
\Phi(t)=\frac{t^3}{6}+O(t^5).
$$

Thus the curves meet the origin in the three descent directions for which $t^3$ is negative real,

$$
\boxed{\arg t=\frac\pi3,\ \pi,\ \frac{5\pi}3.}
$$

One curve is the negative real axis $v=0$, $u<0$. The other two are conjugate curves $v=\pm v_+(u)$ with $u>0$ and $0<v_+(u)<\pi$. Near the origin, $v_+(u)\sim\sqrt3u$, while for $u\to+\infty$ the defining equation gives $\sin v_+\sim2v_+e^{-u}$, so $v_+\to\pi$. Their three asymptotes are therefore

$$
\boxed{v=0\quad(u\to-\infty),\qquad v=\pm\pi\quad(u\to+\infty).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31B](../../31b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
