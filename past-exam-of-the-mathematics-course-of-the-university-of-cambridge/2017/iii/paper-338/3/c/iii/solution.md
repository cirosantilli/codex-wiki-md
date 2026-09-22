<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $k=m/2$ independent reads in each sum, [read noise](../../../../../../../read-noise.md) contributes $kr^2/g^2$ in squared [ADU](../../../../../../../analogue-to-digital-unit.md) units. Hence

$$
\operatorname{Var}(A)=\frac Ng+\frac{kr^2}{g^2},\qquad
E^2\simeq\frac{2}{gN}+\frac{2kr^2}{g^2N^2}.
$$

Using the shot-noise-only formula therefore gives

$$
\boxed{g_{\rm naive}\simeq\frac{g}{1+kr^2/(gN)}<g\quad(r>0).}
$$

The condition for negligible contamination is $gN\gg kr^2$, equivalently a large number of collected [Electrons](../../../../../../../electron.md) per individual frame compared with $r^2$. Summing more identical-level frames does not change that ratio because both $N$ and the read [variance](../../../../../../../variance-split.md) scale with $k$. Measure [read noise](../../../../../../../read-noise.md) from paired [bias images](../../../../../../../detector-bias-frame.md), or fit mean versus noise [variance](../../../../../../../variance-split.md) across several illumination levels: the shot-noise slope determines [detector gain](../../../../../../../detector-conversion-gain.md), while the read term gives an intercept. If $r$ is known, the corrected positive solution satisfies $E^2N^2g^2-2Ng-2kr^2=0$. Offset subtraction removes the mean bias but not the read [variance](../../../../../../../variance-split.md). Correlated read errors need a different [covariance](../../../../../../../covariance.md) calculation.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
