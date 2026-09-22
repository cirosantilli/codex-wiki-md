# Derivative criterion for monotonicity

↑ **Parent:** [Monotonic function](monotonic-function.md)

Let $I$ be a [real interval](interval-mathematics.md), and let $f:I\to\mathbb R$ be [differentiable](differentiable-function.md) in its [interior](interior-topology.md) and [continuous](continuous-function.md) at any endpoints belonging to $I$. If the [derivative](derivative.md) satisfies $f'(x)\geq0$ throughout the [interior](interior-topology.md), then $f$ is a [nondecreasing function](nondecreasing-function.md) on $I$. For $x<y$ in $I$, the [mean value theorem](mean-value-theorem.md) supplies $c\in(x,y)$ with

$$
f(y)-f(x)=f'(c)(y-x)\geq0.
$$

Changing $\geq0$ to $\leq0$, $>0$, or $<0$ gives a [nonincreasing function](nonincreasing-function.md), [strictly increasing function](strictly-increasing-function.md), or [strictly decreasing function](strictly-decreasing-function.md), respectively. The endpoint [continuity](continuous-function.md) assumption lets the [mean value theorem](mean-value-theorem.md) apply even when $x$ or $y$ is an endpoint. [OpenStax Calculus Volume 1, mean value theorem and its monotonicity corollary](https://openstax.org/books/calculus-volume-1/pages/4-4-the-mean-value-theorem).

Conversely, if a [nondecreasing function](nondecreasing-function.md) on a [real interval](interval-mathematics.md) is [differentiable](differentiable-function.md) at an interior point $x$, then $f'(x)\geq0$: the [difference quotient](difference-quotient.md) $(f(x+h)-f(x))/h$ is nonnegative for either sign of $h$. A [differentiable](differentiable-function.md) [nonincreasing function](nonincreasing-function.md) has [derivative](derivative.md) $f'(x)\leq0$. Strict [monotonicity](monotonic-function.md) still only forces these weak signs: the [strictly increasing function](strictly-increasing-function.md) $x^3$ has [derivative](derivative.md) zero at zero. The sign of the [derivative](derivative.md) helps locate [intervals](interval-mathematics.md) of [monotonicity](monotonic-function.md) when sketching a graph. [OpenStax Calculus Volume 1, derivatives and the shape of a graph](https://openstax.org/books/calculus-volume-1/pages/4-5-derivatives-and-the-shape-of-a-graph).

The [real interval](interval-mathematics.md) hypothesis matters because a [connected subset of the real line](connected-subset-of-the-real-line.md) contains every point between its inputs. On a disconnected [domain of a function](domain-of-a-function.md), positive [derivatives](derivative.md) need not give a [nondecreasing function](nondecreasing-function.md). For example, take

$$
D=(-2,-1)\cup(1,2),\qquad
f(x)=\begin{cases}x,&-2<x<-1,\\x-10,&1<x<2.\end{cases}
$$

Here $f'(x)=1$ everywhere in $D$, but $-3/2<3/2$ while $f(-3/2)=-3/2>-17/2=f(3/2)$. Each component has a [strictly increasing function](strictly-increasing-function.md), yet their outputs are ordered the wrong way across the gap. This [function](function-split.md) is neither a [nondecreasing function](nondecreasing-function.md) nor a [nonincreasing function](nonincreasing-function.md) on all of $D$; the [mean value theorem](mean-value-theorem.md) cannot cross the missing [interval](interval-mathematics.md).

<a id="image-a-zero-derivative-can-coexist-with-strict-increase-while-a-domain-gap-defeats-the-derivative-test"></a>
![](monotonicity-derivative-and-domain.png)

**[Figure 27](#image-a-zero-derivative-can-coexist-with-strict-increase-while-a-domain-gap-defeats-the-derivative-test). A zero derivative can coexist with strict increase, while a domain gap defeats the derivative test**. Left: the [strictly increasing function](strictly-increasing-function.md) $f(x)=x^3$ and its [derivative](derivative.md) $f'(x)=3x^2$, both zero at the origin. Right: two separate graph segments with [derivative](derivative.md) one on $(-2,-1)\cup(1,2)$, but a lower output on the right component. Open circles exclude the four component endpoints.

## ↑ Ancestors (7)

1. [Monotonic function](monotonic-function.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [A cubic root from existence to a quantitative bracket](a-cubic-root-from-existence-to-a-quantitative-bracket.md)
- [Mean value theorem](mean-value-theorem.md)
