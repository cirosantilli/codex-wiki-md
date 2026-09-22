<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [slope substitution for equations involving x y'-y](../../../../../slope-substitution-for-equations-involving-x-y-y.md): put $v=y/x$ on the positive interval containing the initial point. Then $xy'-y=x^2v'$, so $x^2v'=\cot v$. Near $v(1)=\pi/4$, separating variables gives $\tan v\,dv=dx/x^2$. Integration yields $\ln|\cos v|=1/x+C$. The initial value fixes the sign and constant, giving

$$
\cos\frac yx=\frac1{\sqrt2}e^{1/x-1}.
$$

Choose the [inverse cosine](../../../../../arccosine.md) branch that agrees with $v(1)=\pi/4$. The solution is

$$
\boxed{y(x)=x\arccos\left(\frac{e^{1/x-1}}{\sqrt2}\right),\qquad x>\frac1{1+\tfrac12\ln2}.}
$$

On this interval the argument lies strictly between zero and one and the original cotangent is defined. At the finite lower endpoint, $v\to0$ and the cotangent becomes singular, so that endpoint is excluded from the maximal interval of the [initial value problem](../../../../../initial-value-problem.md). The slope substitution here is valid without classifying the original equation as homogeneous in the usual $y'=F(y/x)$ sense.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [11](../../11.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
