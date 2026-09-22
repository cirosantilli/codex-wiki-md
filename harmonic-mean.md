# Harmonic mean

↑ **Parent:** [Arithmetic mean](arithmetic-mean.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_mean)

The harmonic mean of a nonempty finite list of positive [real numbers](real-number.md) is the [multiplicative inverse](multiplicative-inverse.md) of the [arithmetic mean](arithmetic-mean.md) of their inverses:

$$
H=\frac{n}{\sum_{i=1}^n1/x_i},\qquad \frac nH=\sum_{i=1}^n\frac1{x_i}.
$$

For two inputs, $H=2x_1x_2/(x_1+x_2)$. Replacing each input by $H$ preserves the [sum](sum.md) of inverses, making it useful when a fixed amount divided by a rate determines a cost or duration. This positive-input definition avoids division by zero; negative inputs need not retain the usual averaging or ordering properties. [NIST Digital Library of Mathematical Functions, §1.2(iv), equation 1.2.19: harmonic mean](https://dlmf.nist.gov/1.2.iv).

Travel two legs of equal [length](length.md) $d$ at positive [speeds](speed.md) $v_1,v_2$, with no stops. Their travel [times](time-in-physics.md) are $d/v_1$ and $d/v_2$, so the average [speed](speed.md) is

$$
v_{\mathrm{avg}}=\frac{2d}{d/v_1+d/v_2}=\frac{2}{1/v_1+1/v_2}.
$$

For two $60\,\mathrm{km}$ legs at $30$ and $60\,\mathrm{km/h}$, the [times](time-in-physics.md) are two hours and one hour. **The average [speed](speed.md) is $120/3=40\,\mathrm{km/h}$.** The same [speeds](speed.md) maintained for one hour each instead cover $90\,\mathrm{km}$ in two hours, giving the [arithmetic mean](arithmetic-mean.md) $45\,\mathrm{km/h}$. A slower equal-distance leg occupies more [time](time-in-physics.md), so the data being averaged must include what is held equal. This is total distance traveled divided by elapsed [time](time-in-physics.md); a return journey can have zero average [velocity](velocity.md) while keeping a positive average [speed](speed.md). [University of Cambridge, Underground Mathematics: equal-distance and equal-time speed averages](https://undergroundmathematics.org/introducing-calculus/average-speed/averages).

<a id="image-equal-distance-travel-gives-a-harmonic-mean-equal-time-travel-gives-an-arithmetic-mean"></a>
![](harmonic-mean-equal-distance-travel.png)

**[Figure 7](#image-equal-distance-travel-gives-a-harmonic-mean-equal-time-travel-gives-an-arithmetic-mean). Equal-distance travel gives a harmonic mean; equal-time travel gives an arithmetic mean**. Two original idealized journeys use the same [speeds](speed.md), $30$ and $60\,\mathrm{km/h}$. On the left each leg has [length](length.md) $60\,\mathrm{km}$, taking a total of three hours. On the right each leg lasts one hour, taking two hours and covering $90\,\mathrm{km}$. Dashed straight lines show the corresponding average [speeds](speed.md). The diagrams omit stops and transition duration and show cumulative distance traveled rather than signed [displacement](displacement.md).

The [arithmetic-geometric mean inequality](arithmetic-geometric-mean-inequality.md) applied to the inverses gives $H\leq G$; together with $G\leq A$ it yields the comparison in [geometric mean](geometric-mean.md). For two inputs the arithmetic–harmonic gap has the exact form

$$
A-H=\frac{(x_1-x_2)^2}{2(x_1+x_2)}\geq0.
$$

For $30$ and $60$ the gap is five. With one positive input held fixed and another approaching zero, the [harmonic mean](harmonic-mean.md) approaches zero too: a very slow fixed-distance leg dominates the travel [time](time-in-physics.md). Unequal leg [lengths](length.md) instead require a [weighted harmonic mean](weighted-harmonic-mean.md).

**Table of contents**

- [Weighted harmonic mean](weighted-harmonic-mean.md)

## ↑ Ancestors (9)

1. [Arithmetic mean](arithmetic-mean.md)
2. [Weighted arithmetic mean](weighted-arithmetic-mean.md)
3. [Sum](sum.md)
4. [Summation](summation.md)
5. [Addition](addition.md)
6. [Arithmetic](arithmetic-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Geometric mean](geometric-mean.md)
- [Harmonic mean](harmonic-mean.md)
- [Layered porous permeability](layered-porous-permeability.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-80/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-38/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-39/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/3/c/ii/solution.md)
- [Total-effort formula for a proportional contest with outside effort](total-effort-formula-for-a-proportional-contest-with-outside-effort.md)
- [Weighted harmonic mean](weighted-harmonic-mean.md)
