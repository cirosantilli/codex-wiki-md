<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Linear [eccentricity damping](../../../../../../eccentricity-damping.md) adds $-z/\tau$ to the complex equation:

$$
\dot z=(iA-\tau^{-1})z+i\sum_k\nu_ke^{i(g_kt+\beta_k)}.
$$

Its solution is

$$
\boxed{z(t)=C e^{(iA-1/\tau)t}
+\sum_{k=1}^2
\frac{\nu_k}{g_k-A-i/\tau}e^{i(g_kt+\beta_k)}}.
$$

Unlike the undamped free eccentricity, the homogeneous term decays exponentially. The forced response survives, acquires a phase lag, and has finite amplitude

$$
\frac{|\nu_k|}{\sqrt{(g_k-A)^2+\tau^{-2}}}.
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
