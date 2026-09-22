<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the dynamically regulated interpretation, take $X(0)=S$, $Y(0)=Z(0)=0$, and let X production respond to Y repression after the [ligand](../../../../ligand-biochemistry.md) appears. Define $h=K/S\in(0,1)$. Initially active X drives both Y and Z, giving $Y=Z=S(1-e^{-\alpha t})$. Y reaches $K$ at $t_1=-\ln(1-h)/\alpha$ and switches X production off. X then decays from $S$ to $K$, reaching it at

$$
t_2=t_1+\frac{\ln(1/h)}\alpha=\frac1\alpha\ln\frac1{h(1-h)}.
$$

Until $t_2$, X remains active and Y keeps being produced. Thus $Y_2=S(1-h+h^2)$. At $t_2$, Y production stops, but Y still activates Z. Its subsequent decay crosses $K$ at

$$
\boxed{t_{\max1}=t_3=t_2+\frac1\alpha\ln\frac{Y_2}{K}
=\frac1\alpha\ln\frac{1-h+h^2}{h^2(1-h)}.}
$$

Immediately afterwards both inputs to the Z OR gate are below threshold, so Z production stops and its [derivative](../../../../derivative.md) changes from positive to negative. Since Z has been continuously produced from zero until $t_3$,

$$
\boxed{Z_{\max1}=S(1-e^{-\alpha t_3})
=S\left[1-\frac{h^2(1-h)}{1-h+h^2}\right].}
$$

For $h=1/2$, $t_{\max1}=\ln6/\alpha$ and $Z_{\max1}=5S/6$. Y repression is lifted at $t_3$, but X must first rebuild from a subthreshold value, so Z has a genuine first local maximum before any later response.

**Wording qualification:** if “X is always present at its [steady state](../../../../steady-state.md) [concentration](../../../../concentration.md)” is read as an external clamp maintaining $X=S$ _after_ [ligand](../../../../ligand-biochemistry.md) arrival, it overrides Y's repression and changes the problem. Then $Z=S(1-e^{-\alpha t})$ rises monotonically, with no finite first maximum. The finite-peak result uses the consistent initial-steady-state interpretation in which the stated [negative feedback](../../../../negative-feedback.md) can act.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
