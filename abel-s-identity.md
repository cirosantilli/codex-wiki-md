<h1 id="abel-s-identity">Abel's identity</h1>

↑ **Parent:** [Wronskian](wronskian.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abel's_identity)

For $y\prime\prime+py\prime+qy=0$, the Wronskian satisfies $W\prime=-pW$.

More precisely, let $y_1,y_2$ be [solutions of a differential equation](solution-of-a-differential-equation.md) for the same [homogeneous linear differential equation](homogeneous-linear-differential-equation.md)

$$
y''+p(x)y'+q(x)y=0
$$

on an [interval](interval-mathematics.md) $I$ where $p,q$ are [continuous functions](continuous-function.md). For any $x_0\in I$, [Abel's identity](abel-s-identity.md) gives

$$
W(y_1,y_2)(x)=W(y_1,y_2)(x_0)\exp\left(-\int_{x_0}^x p(s)\,ds\right).
$$

Only the coefficient of $y'$ enters the evolution of the [Wronskian](wronskian.md). In an unnormalized equation $A(x)y''+B(x)y'+C(x)y=0$, first use $p=B/A$ on an [interval](interval-mathematics.md) where $A\ne0$ and the coefficient ratios are [continuous functions](continuous-function.md).[NIST Digital Library of Mathematical Functions; §1.13(i), equation 1.13.5 and the following coefficient-ratio explanation; stated there for analytic coefficients](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)

The proof uses cancellation. Differentiating the [Wronskian](wronskian.md) by the [product rule](product-rule.md) and substituting the common equation gives

$$
\begin{aligned}
W'&=(y_1y_2'-y_1'y_2)'=y_1y_2''-y_1''y_2\\
&=y_1(-py_2'-qy_2)-(-py_1'-qy_1)y_2=-pW.
\end{aligned}
$$

Multiplying this [first-order linear differential equation](first-order-linear-differential-equation.md) by the [integrating factor](integrating-factor.md) $\mu(x)=\exp(\int_{x_0}^x p(s)\,ds)$ gives $(\mu W)'=0$. Since $\mu(x_0)=1$, the constant is $W(x_0)$, proving [Abel's identity](abel-s-identity.md). This argument also covers $W(x_0)=0$ without dividing by $W$.

The [exponential function](exponential-function.md) is positive for real $p$, so a real [Wronskian](wronskian.md) either vanishes everywhere or has a fixed nonzero sign throughout $I$. In the preceding example, $p=-1$ and $W(0)=3$ give $W(x)=3e^x$ immediately. If $p=0$, every [Wronskian](wronskian.md) of two [solutions of a differential equation](solution-of-a-differential-equation.md) for that same equation is constant, regardless of $q$. Thus [Abel's identity](abel-s-identity.md) can certify [linear independence](linear-independence.md) and find the denominator used in [variation of parameters](variation-of-parameters.md) without explicit formulas for both [solutions of a differential equation](solution-of-a-differential-equation.md).

## ↑ Ancestors (9)

1. [Wronskian](wronskian.md)
2. [Second-order linear differential equation](second-order-linear-differential-equation.md)
3. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
4. [Ordinary differential equation](ordinary-differential-equation.md)
5. [Differential equation](differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Abel's identity](abel-s-identity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-2/6b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/8/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/8/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/8/c/solution.md)
- [Wronskian](wronskian.md)
