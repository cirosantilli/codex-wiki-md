<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [homogeneous solution](../../../../../homogeneous-solution.md) $h(x)=e^{-x}\cos x$ already has the prescribed endpoint values. Thus $z=y-h$ has zero [boundary conditions](../../../../../boundary-condition.md) and satisfies $\mathcal Lz=f$. The [Green's function](../../../../../green-s-function-split.md) gives

$$
\boxed{y(x)=e^{-x}\cos x+\int_0^{\pi/2}g(x,\xi)f(\xi)\,d\xi}.
$$

Equivalently, splitting the [integral](../../../../../integral-split.md) at $\xi=x$ gives the explicit formula

$$
y(x)=e^{-x}\left[
\cos x\left(1-\int_0^xe^\xi\sin\xi\,f(\xi)\,d\xi\right)
-\sin x\int_x^{\pi/2}e^\xi\cos\xi\,f(\xi)\,d\xi
\right].
$$

Any difference between two solutions would be $e^{-x}(C\cos x+D\sin x)$ with zero endpoint values, forcing $C=D=0$. The displayed solution is therefore unique.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
