<h1 id="14e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First assume $a-b\notin\mathbb Z$ and nonsingular parameters, so the two infinity solutions $w_1$ and $w_2$, obtained by exchanging $a,b$, are independent. Write $F=Aw_1+Bw_2$. Since the power series at $1/z=0$ starts at one, $w_1\sim(-z)^{-a}$ and $w_2\sim(-z)^{-b}$.

In the parameter region $\Re(b-a)>0$, let $z\to-\infty$ in the [Pfaff transformation](../../../../../../pfaff-transformation.md). The $w_2$ term vanishes after multiplication by $(-z)^a$, while $z/(z-1)\to1$ and $(-z)/(1-z)\to1$. The supplied value at one of the [Gauss hypergeometric function](../../../../../../hypergeometric-function.md) therefore gives

$$
A=F(a,c-b;c;1)=\frac{\Gamma(c)\Gamma(b-a)}{\Gamma(b)\Gamma(c-a)}.
$$

Analytic continuation in the parameters extends this coefficient to the nonresonant parameter domain. Exchange $a,b$ to determine $B$. Hence the [hypergeometric connection formula at infinity](../../../../../../hypergeometric-connection-formula-at-infinity.md) is

$$
\boxed{F(a,b;c;z)=\frac{\Gamma(c)\Gamma(b-a)}{\Gamma(b)\Gamma(c-a)}w_1(z)+\frac{\Gamma(c)\Gamma(a-b)}{\Gamma(a)\Gamma(c-b)}w_2(z).}
$$

The branch is $|\arg(-z)|<\pi$. The existence of $F(a,b;c;1)$ alone does not exclude integer $a-b$. At such resonant values the two separate displayed terms can be singular; the correct statement takes their combined parameter limit, which can contain logarithms. This qualification is essential, for example when $a=b$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14E](../../14e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
