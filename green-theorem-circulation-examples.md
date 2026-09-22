# Green theorem circulation examples

↑ **Parent:** [Green theorem](green-theorem.md)

Take the [vector field](vector-field.md) $F=(-2y,3x)$. Its scalar [curl](curl.md) is the constant $3-(-2)=5$, so [Green theorem](green-theorem.md) predicts that its positively oriented boundary [line integral](line-integral.md) is five times the enclosed [area](surface-area.md). This one field makes both a round and a rectangular calculation transparent.

For the [circle](circle.md) $x^2+y^2=4$, choose the counterclockwise [parametric equations](parametric-equation.md) $\gamma(t)=(2\cos t,2\sin t)$, $0\leq t\leq2\pi$. Direct substitution in the [line integral](line-integral.md) gives

$$
\oint_C(-2y\,dx+3x\,dy)
=\int_0^{2\pi}(8\sin^2t+12\cos^2t)\,dt
=20\pi.
$$

The interior [double integral](double-integral.md) is shorter: the [disk](disk-mathematics.md) has [area](surface-area.md) $4\pi$, hence $\iint_D5\,dA=20\pi$. Reversing the [boundary orientation](boundary-orientation.md) gives $-20\pi$.

For the [rectangle](rectangle.md) $D=[0,3]\times[0,2]$, traverse its bottom, right, top, and left edges in that order. The four [line integrals](line-integral.md) are respectively

$$
\int_0^3 0\,dx=0,\qquad
\int_0^2 9\,dy=18,\qquad
\int_3^0(-4)\,dx=12,\qquad
\int_2^0 0\,dy=0.
$$

Their sum is $30$, agreeing with $\iint_D5\,dA=5\cdot3\cdot2$. In both examples the path geometry changes the separate contributions, while constant [curl](curl.md) makes only [area](surface-area.md) matter to the final answer.

<a id="image-one-vector-field-two-positively-oriented-boundaries-scalar-curl-five-gives-circulation-twenty-pi-around-the-radius-two-circle-and-thirty-around-the-three-by-two-rectangle"></a>
![](green-theorem-circle-rectangle-circulation.png)

**[Figure 9](#image-one-vector-field-two-positively-oriented-boundaries-scalar-curl-five-gives-circulation-twenty-pi-around-the-radius-two-circle-and-thirty-around-the-three-by-two-rectangle). One vector field, two positively oriented boundaries: scalar curl five gives circulation twenty pi around the radius-two circle and thirty around the three-by-two rectangle**.

## ↑ Ancestors (9)

1. [Green theorem](green-theorem.md)
2. [Vector calculus](vector-calculus.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
