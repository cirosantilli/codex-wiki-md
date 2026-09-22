<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

A function is [Fréchet differentiable](../../../../../frechet-differentiability.md) at $x$ when there is a [linear map](../../../../../linear-map.md) $A:\mathbb R^n\to\mathbb R^m$ such that

$$
f(x+h)=f(x)+Ah+r(h),\qquad\frac{|r(h)|}{|h|}\longrightarrow0.
$$

This [linear map](../../../../../linear-map.md), which is unique, is the [derivative](../../../../../derivative.md) $Df(x)$.

For the [chain rule](../../../../../chain-rule.md), if $f$ is [differentiable](../../../../../differentiable-function.md) at $x$ and $g$ is [differentiable](../../../../../differentiable-function.md) at $f(x)$, then $g\circ f$ is [differentiable](../../../../../differentiable-function.md) at $x$ and $D(g\circ f)(x)=Dg(f(x))Df(x)$. Indeed write $f(x+h)-f(x)=Ah+r(h)=v(h)$ and $g(f(x)+v)=g(f(x))+Bv+s(v)$, where $r(h)=o(|h|)$, $s(v)=o(|v|)$. Since $v(h)=O(|h|)$, substitution gives

$$
g(f(x+h))-g(f(x))=BAh+Br(h)+s(v(h))=BAh+o(|h|),
$$

which proves the assertion, including paths on which $v(h)=0$.

For $g_1$, write $q=x^2-y^2$. Away from the two diagonal lines, $q\ne0$ and the formula is a composition of smooth functions, hence [differentiable](../../../../../differentiable-function.md). At the origin, $|g_1(x,y)|\leq|x^2-y^2|\leq x^2+y^2$, so its ratio to the displacement length tends to zero. Its [derivative](../../../../../derivative.md) there is therefore zero: this is [quadratic damping restores differentiability at the origin](../../../../../quadratic-damping-restores-differentiability-at-the-origin.md).

At a nonzero point $(a,b)$ with $a=\pm b$, necessarily $a\ne0$. Along the $x$ direction,

$$
\frac{g_1(a+t,b)-g_1(a,b)}t
=(2a+t)\sin\frac1{2at+t^2}.
$$

The denominator inside the sine is locally an invertible function of $t$, with nonzero [derivative](../../../../../derivative.md) $2a$. Choose sequences tending to zero for which its reciprocal equals $2\pi n+\pi/2$ and $2\pi n+3\pi/2$. The quotients tend to $2a$ and $-2a$. Thus even this [directional derivative](../../../../../directional-derivative.md) fails to exist, and the function is not [differentiable](../../../../../differentiable-function.md) there. Consequently

$$
\boxed{\operatorname{Diff}(g_1)=\{(x,y):x\ne y,\ x\ne-y\}\cup\{(0,0)\}.}
$$

For $g_2$, the formula is smooth away from zero. At zero, $|g_2(x,y)|\leq x^2+y^2$, so the same remainder estimate gives zero [derivative](../../../../../derivative.md). Hence

$$
\boxed{\operatorname{Diff}(g_2)=\mathbb R^2,\qquad Dg_2(0,0)=0.}
$$

No limit of the sine factor itself is needed for either [derivative](../../../../../derivative.md) at the origin.

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
