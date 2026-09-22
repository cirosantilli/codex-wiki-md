<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The delta function in the specified [convolution](../../../../../convolution.md) kernel collapses the $\mathbf k'$ integral to $-i\gamma G$. Set $\lambda=e\gamma$ and $\omega_0^2=k^2+m^2$. Then

$$
G(\mathbf k;\omega)=\frac1{-\omega^2-2i\lambda\omega+\omega_0^2},\qquad G(\mathbf k;\tau)=\int_{-\infty}^{\infty}\frac{d\omega}{2\pi}\frac{e^{-i\omega\tau}}{-\omega^2-2i\lambda\omega+\omega_0^2}.
$$

There is a change of assumptions here: the specified kernel is the transform of **$V=-i\gamma$**, which is not real. These later parts define a formal [analytic continuation](../../../../../analytic-continuation.md) to an effective damped equation, $[\partial_\tau^2+2\lambda\partial_\tau+\omega_0^2]G=\delta(\tau)$; they cannot simultaneously describe the earlier real external potential. The following [pole](../../../../../pole.md) analysis uses that continued operator.

Completing the square gives $D(\omega)=-(\omega+i\lambda)^2+(\omega_0^2-\lambda^2)$, so

$$
\boxed{\omega_\pm=-i\lambda\pm\sqrt{k^2+m^2-\lambda^2}.}
$$

For $e>0$, hence $\lambda>0$, the underdamped regime has two [poles](../../../../../pole.md) at $\pm\Omega-i\lambda$, with $\Omega=\sqrt{k^2+m^2-\lambda^2}>0$. Both lie below the [real axis](../../../../../real-axis.md). In the overdamped regime they lie on the [imaginary axis](../../../../../imaginary-axis.md) at $-i(\lambda\mp\kappa)$, where $\kappa=\sqrt{\lambda^2-k^2-m^2}<\lambda$ for $k^2+m^2>0$; both are again below the [real axis](../../../../../real-axis.md). At equality they coalesce into a [double pole](../../../../../double-pole.md) at $-i\lambda$. If $m<|\lambda|$, the crossover occurs at $k_c=\sqrt{\lambda^2-m^2}$; increasing $k$ moves the two imaginary [poles](../../../../../pole.md) together and then apart horizontally. If $m>|\lambda|$, every $k$ is underdamped; if equal, only $k=0$ is critical.

<a id="3/c/image-underdamped-critically-damped-and-overdamped-pole-positions-for-positive-damping"></a>
![](../../../../../past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2016/paper-1-green-function-poles.png)

**[Figure 2](#3/c/image-underdamped-critically-damped-and-overdamped-pole-positions-for-positive-damping). Underdamped, critically damped and overdamped pole positions for positive damping**.

The sign of $e$ is not specified: for $e<0$ all nonzero-frequency [poles](../../../../../pole.md) are instead in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md), describing [antidamping](../../../../../antidamping.md); for $e=0$ they lie on the [real axis](../../../../../real-axis.md) and a causal prescription is required. When $m=k=0$, one [pole](../../../../../pole.md) is at zero even for nonzero $\lambda$ and a real-axis prescription is again needed. The figure uses illustrative $\lambda=1$, not supplied numerical data.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
