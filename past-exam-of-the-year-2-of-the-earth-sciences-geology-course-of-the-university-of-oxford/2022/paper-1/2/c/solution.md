<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose coordinates $(x,y,z)=(\mathrm{east},\mathrm{north},\mathrm{up})$ and use compression-positive [effective stress](../../../../../effective-stress.md). One possible tensor, in MPa, is

$$
\boxed{\boldsymbol\sigma'=\begin{pmatrix}10&0&0\\0&15&0\\0&0&20.3961\end{pmatrix}.}
$$

Its ordered [principal stresses](../../../../../principal-stress.md) are vertical $\sigma_1'$, north–south $\sigma_2'$ and east–west $\sigma_3'$. On the $55^\circ$ east-dipping plane,

$$
\sigma_n'=\sigma_1'\cos^255^\circ+\sigma_3'\sin^255^\circ,
\qquad
|\tau|=(\sigma_1'-\sigma_3')\sin55^\circ\cos55^\circ,
$$

so $|\tau|/\sigma_n'=0.36397$, as required by the conditional friction estimate. The scale is illustrative: no absolute [stress](../../../../../stress.md) magnitude is supplied. A corresponding total [stress tensor](../../../../../cauchy-stress-tensor.md) is $\boldsymbol\sigma^c=\boldsymbol\sigma'+P_f\mathbf I$ for any specified [isotropic](../../../../../isotropy.md) [pore fluid pressure](../../../../../pore-fluid-pressure.md) $P_f$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
