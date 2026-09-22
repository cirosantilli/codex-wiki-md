<h1 id="b/6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Zero is a strict weak local minimizer and is not a strong local minimizer.** Write $D=\int_0^1u'^2$. For zero endpoint values, [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) applied to

$$
u(x)=(1-x)\int_0^xu'(t)dt-x\int_x^1u'(t)dt
$$

gives $|u(x)|^2\leq x(1-x)D$, hence $\int_0^1x^2u^2\leq D/20$. For sufficiently small slopes, Taylor expansion gives $\tfrac12[\sin(1+u'^2)-\sin1]\geq(\tfrac12\cos1-\varepsilon)u'^2$. Therefore

$$
I(u)-I(0)\geq\left(\frac12\cos1-\varepsilon-\frac1{20}\right)D>0
$$

for a suitably small fixed $\varepsilon$ and every nonzero sufficiently weakly close competitor.

For strong minimality take $a=\sqrt{3\pi/2-1}$ and $u_N(x)=a\operatorname{dist}(x,N^{-1}\mathbb Z)$. Their amplitudes tend to zero but slopes are $\pm a$, so $\sin(1+u_N'^2)=-1$. Thus $I(u_N)\leq-1/2<I(0)=\sin1/2$. Uniform closeness therefore does not prevent a decrease in energy.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../split.md)
7. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
