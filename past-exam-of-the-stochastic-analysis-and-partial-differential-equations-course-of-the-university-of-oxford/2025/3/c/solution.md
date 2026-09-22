<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $f$ in the [generator domain](../../../../generator-domain.md) $D(L)$. The [semigroup commutation with its unbounded generator](../../../../semigroup-commutation-with-its-unbounded-generator.md) implies $P_tf\in D(L)$ and

$$
\frac d{dt}P_tf=P_tLf=LP_tf.
$$

Indeed, applying the bounded operator $P_t$ to the difference quotient at zero gives the right derivative $P_tLf$; [strong continuity](../../../../strong-continuity.md) gives the full orbit derivative for $t>0$. Now [integration by parts](../../../../integration-by-parts.md) in the [Bochner integral](../../../../bochner-integral.md) yields

$$
\begin{aligned}
R_\lambda Lf
&=\int_0^\infty e^{-\lambda t}P_tLf\,dt
=\int_0^\infty e^{-\lambda t}\frac d{dt}P_tf\,dt\\
&=\left[e^{-\lambda t}P_tf\right]_0^\infty
+\lambda\int_0^\infty e^{-\lambda t}P_tf\,dt
=-f+\lambda R_\lambda f.
\end{aligned}
$$

The boundary term at infinity vanishes because $\|e^{-\lambda t}P_tf\|\leq e^{-\lambda t}\|f\|$. The derivative integral exists as a [Bochner integral](../../../../bochner-integral.md), since its integrand is bounded in [norm](../../../../norm.md) by $e^{-\lambda t}\|Lf\|$.

Multiplying this identity by $\lambda$ gives

$$
\lambda(\lambda R_\lambda-I)f=\lambda R_\lambda(Lf).
$$

Part (b) applies to the fixed vector $Lf\in E$, so

$$
\boxed{\lambda(\lambda R_\lambda-I)f\longrightarrow Lf
\quad\text{in }E\qquad(f\in D(L)).}
$$

The bounded operators $L_\lambda=\lambda^2R_\lambda-\lambda I$ are the [Yosida approximation](../../../../yosida-approximation.md) of the [semigroup generator](../../../../infinitesimal-generator-of-a-semigroup.md). The proof only applies the unbounded operator $L$ to $f\in D(L)$; the contraction and limit arguments then act on the ordinary vector $Lf$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
