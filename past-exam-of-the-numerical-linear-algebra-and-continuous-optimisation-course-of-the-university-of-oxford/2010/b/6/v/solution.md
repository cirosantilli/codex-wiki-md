<h1 id="b/6/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

At the current exact path point $v(\mu)$, stationarity is already zero and $Cy=\mu e$. Therefore $F_{\bar\mu}(v(\mu))=(0,(\mu-\bar\mu)e)^T$. Its [Newton correction](../../../../../newton-correction.md) solves

$$
\boxed{J(v(\mu))\Delta v_N=\begin{pmatrix}0\\(\bar\mu-\mu)e\end{pmatrix}.}
$$

The matrix has no explicit dependence on the barrier parameter, so comparison with part (iv) gives

$$
\boxed{\Delta v_N=(\bar\mu-\mu)v'(\mu)}
$$

when $J$ is nonsingular. If it is singular, the displayed vector is still a solution of the correction equations, but uniqueness of the correction cannot be inferred from differentiability of the path alone.

This step is exactly the tangent predictor in the stated first-order [Taylor expansion](../../../../../taylor-expansion.md). For nearby positive $\bar\mu$, it approximates the new path point with error $o(|\bar\mu-\mu|)$; a bounded second path derivative improves this to $O((\bar\mu-\mu)^2)$. Continuity also preserves strict positivity for sufficiently small parameter changes. Larger changes may require damping to keep both the constraint values and multiplier estimates positive.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
