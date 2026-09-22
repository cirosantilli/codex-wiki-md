# Rolle theorem

↑ **Parent:** [Calculus](calculus-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rolle_theorem)

[Rolle's theorem](rolle-theorem.md) is the equal-endpoint case of the [mean value theorem](mean-value-theorem.md). Let $a<b$ and let the [real-valued function](real-valued-function.md) $f:[a,b]\to\mathbb R$ be [continuous](continuous-function.md) on the [closed interval](closed-real-interval.md) $[a,b]$ and [differentiable](differentiable-function.md) on the [open interval](open-interval.md) $(a,b)$. If $f(a)=f(b)$, there exists $c\in(a,b)$ with $f'(c)=0$. Geometrically, a [tangent line](tangent-line.md) somewhere in the [interior](interior-topology.md) is horizontal, like the [secant line](secant-line.md) joining the endpoints. [OpenStax, Calculus Volume 1, Section 4.4: Rolle's theorem](https://openstax.org/books/calculus-volume-1/pages/4-4-the-mean-value-theorem)

For the [polynomial](polynomial-split.md) $f(x)=x(x-2)$ on $[0,2]$, both endpoint values are zero and the [derivative](derivative.md) is $f'(x)=2x-2$. Thus $c=1$, where $f(1)=-1$, and the horizontal [tangent line](tangent-line.md) is $y=-1$. The horizontal [secant line](secant-line.md) is $y=0$: equal endpoint values do not force the interior [tangent line](tangent-line.md) to pass through those endpoints.

The [absolute value function](absolute-value.md) $f(x)=|x|$ on $[-1,1]$ exposes the importance of [differentiability](differentiability.md). It is [continuous](continuous-function.md) and $f(-1)=f(1)=1$, so the [secant line](secant-line.md) has [slope](slope.md) zero. However,

$$
f'(x)=\begin{cases}-1,&-1<x<0,\\1,&0<x<1,\end{cases}
$$

and the [derivative](derivative.md) does not exist at zero because the [one-sided derivatives](one-sided-derivative.md) disagree. Every existing [derivative](derivative.md) in the [interior](interior-topology.md) is nonzero. The corner fails a hypothesis of both [Rolle's theorem](rolle-theorem.md) and the [mean value theorem](mean-value-theorem.md), so neither conclusion is guaranteed.

<a id="image-rolle-s-theorem-gives-a-horizontal-tangent-line-for-a-polynomial-while-a-corner-defeats-differentiability"></a>
![](rolle-theorem-and-corner-counterexample.png)

**[Figure 15](#image-rolle-s-theorem-gives-a-horizontal-tangent-line-for-a-polynomial-while-a-corner-defeats-differentiability). Rolle's theorem gives a horizontal tangent line for a polynomial, while a corner defeats differentiability**.

For a short proof, the [extreme value theorem](extreme-value-theorem.md) supplies a greatest and a least value on $[a,b]$. If $f$ is a [constant function](constant-function.md), every interior point works. Otherwise at least one of these values differs from the common endpoint value, so it is attained at an interior [extremum](maximum-and-minimum.md). At an interior [local maximum](local-maximum.md) or [local minimum](local-minimum.md), [differentiability](differentiability.md) forces the [derivative](derivative.md) to be zero: the [difference quotients](difference-quotient.md) from the two sides have opposite weak signs and the same [limit](limit-of-a-function.md).

This turns repeated values into information about [derivatives](derivative.md). Two distinct [roots of a polynomial](root-of-a-polynomial.md) force a root of its [derivative](derivative.md) between them; iterating this idea gives the [Rolle root count with multiplicities](rolle-root-count-with-multiplicities.md). More generally, a [differentiable function](differentiable-function.md) with nonzero [derivative](derivative.md) throughout a [real interval](interval-mathematics.md) cannot repeat a value there, hence is [injective](injective-function.md). The beauty is that knowing only two equal values guarantees an exact local feature somewhere between them.

**Table of contents**

- [Rolle root count with multiplicities](rolle-root-count-with-multiplicities.md)

## ↑ Ancestors (6)

1. [Calculus](calculus-split.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/9d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1/11f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/11d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/11d/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-318/2/c/solution.md)
- [Rolle root count with multiplicities](rolle-root-count-with-multiplicities.md)
