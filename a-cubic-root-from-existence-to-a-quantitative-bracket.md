# A cubic root from existence to a quantitative bracket

↑ **Parent:** [Intermediate value theorem](intermediate-value-theorem.md)

Consider the original worked example $f(x)=x^3+x-1$ on $[0,1]$. First, existence: a [polynomial function](polynomial-function.md) is a [continuous function](continuous-function.md), and $f(0)=-1<0<1=f(1)$. The [intermediate value theorem](intermediate-value-theorem.md) therefore supplies a [zero of a function](zero-of-a-function.md) $r\in(0,1)$, even before its value has been calculated.

Second, uniqueness is a separate argument. The [derivative](derivative.md) is $f'(x)=3x^2+1>0$. The [derivative criterion for monotonicity](derivative-criterion-for-monotonicity.md), obtained from the [mean value theorem](mean-value-theorem.md), makes $f$ a [strictly increasing function](strictly-increasing-function.md). Two distinct [zeros of a function](zero-of-a-function.md) would contradict that strict increase. Thus this [root bracket](root-bracket.md) contains exactly one [zero of a function](zero-of-a-function.md); indeed the same [derivative](derivative.md) argument proves uniqueness on the entire [real line](real-line.md).

Third, localization uses the existing [bisection method](bisection-method.md). Set $[a_0,b_0]=[0,1]$; after $k$ completed halvings, retain $[a_k,b_k]$ with opposite endpoint signs. Each update tests the old [midpoint](midpoint.md) $m_{k-1}=(a_{k-1}+b_{k-1})/2$. The first five exact updates are

$$
\begin{array}{c|c|r|c}
k&\text{tested }m_{k-1}&f(m_{k-1})&\text{retained }[a_k,b_k]\\\hline
1&1/2&-3/8&[1/2,1]\\
2&3/4&11/64&[1/2,3/4]\\
3&5/8&-67/512&[5/8,3/4]\\
4&11/16&51/4096&[5/8,11/16]\\
5&21/32&-2003/32768&[21/32,11/16]
\end{array}
$$

Every retained [root bracket](root-bracket.md) contains $r$ by the [intermediate value theorem](intermediate-value-theorem.md). After ten halvings, exact arithmetic gives

$$
a_{10}=\frac{349}{512},\qquad b_{10}=\frac{699}{1024},\qquad
f(a_{10})=-\frac{220923}{134217728}<0,
\qquad f(b_{10})=\frac{744899}{1073741824}>0.
$$

Hence $0.681640625<r<0.6826171875$. The new [midpoint](midpoint.md) and its [bisection error bound](bisection-error-bound.md) are

$$
m_{10}=\frac{1397}{2048}=0.68212890625,\qquad
|m_{10}-r|\leq\frac{1}{2048}=0.00048828125.
$$

This [midpoint](midpoint.md) is the estimate after the tenth update; the last tested point was $m_9=699/1024$. In general the retained width is $2^{-k}$, so the [bisection error bound](bisection-error-bound.md) is $2^{-(k+1)}$. Nine halvings already suffice for an error at most $10^{-3}$, since $2^{-10}=0.0009765625<10^{-3}$. This guarantee comes from the width of the [root bracket](root-bracket.md), independently of any displayed decimal approximation to the unknown [zero of a function](zero-of-a-function.md). Endpoint signs must be established reliably if evaluations use [floating-point arithmetic](floating-point-arithmetic.md).

<a id="image-the-cubic-x-cubed-plus-x-minus-one-its-unique-root-and-the-first-five-nested-bisection-brackets"></a>
![](intermediate-value-cubic-nested-root-brackets.png)

**[Figure 23](#image-the-cubic-x-cubed-plus-x-minus-one-its-unique-root-and-the-first-five-nested-bisection-brackets). The cubic x cubed plus x minus one: its unique root and the first five nested bisection brackets**.

## ↑ Ancestors (9)

1. [Intermediate value theorem](intermediate-value-theorem.md)
2. [Continuous function](continuous-function.md)
3. [Limit of a function](limit-of-a-function.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
