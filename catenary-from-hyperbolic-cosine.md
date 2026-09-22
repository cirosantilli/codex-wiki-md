# Catenary from hyperbolic cosine

↑ **Parent:** [Hyperbolic cosine](hyperbolic-cosine.md)

A [catenary](catenary.md) is the static shape of an ideal flexible, inextensible chain hanging under its own [gravitational weight](weight-physics.md) in a [uniform gravitational field](uniform-gravitational-field.md), with uniform [linear mass density](linear-mass-density.md) along its [arc length](arc-length.md). With the lowest point above $x=0$, one convenient vertical origin gives

$$
y(x)=a\cosh(x/a),\qquad a>0.
$$

Here $a$ has units of [length](length.md). The supports and the chain's [arc length](arc-length.md) determine the scale and position; horizontal and vertical shifts give the general [catenary](catenary.md). [Robert Hunt, Cambridge Mathematical Methods II: worked example, The Catenary](https://www.damtp.cam.ac.uk/user/reh10/lectures/nst-mmii-handout3.pdf)

For $a=1$, the three points at $x=-1,0,1$ have heights $\cosh1\approx1.543081$, $1$, and $\cosh1\approx1.543081$. If heights should instead be measured from the lowest point, subtract $a$:

$$
y_{\mathrm{shifted}}(x)=a\bigl(\cosh(x/a)-1\bigr).
$$

The same three heights are then approximately $0.543081$, $0$, and $0.543081$. The shift changes the vertical origin and preserves the [catenary](catenary.md) shape.

<a id="image-a-hanging-chain-follows-a-scaled-hyperbolic-cosine-with-an-optional-shift-of-its-lowest-point-to-zero"></a>
![](hyperbolic-cosine-catenary.png)

**[Figure 12](#image-a-hanging-chain-follows-a-scaled-hyperbolic-cosine-with-an-optional-shift-of-its-lowest-point-to-zero). A hanging chain follows a scaled hyperbolic cosine, with an optional shift of its lowest point to zero**. The left panel marks $x=-1,0,1$ on $y=\cosh x$. The right panel puts the lowest point at zero, compares three positive scales $a$, and shows the local [parabola](parabola.md) $y=x^2/2$ for $a=1$.

The scale also measures [tension](tension.md): if $H>0$ is its constant horizontal component, $\mu$ is the [linear mass density](linear-mass-density.md), and $g$ is the magnitude of [gravitational acceleration](gravitational-acceleration.md), then $a=H/(\mu g)$. A short [force](force-split.md) balance explains this. For the portion from the lowest point to $x\geq0$, with [arc length](arc-length.md) $s(x)$, vertical [tension](tension.md) balances its [gravitational weight](weight-physics.md) and horizontal [tension](tension.md) gives

$$
Hy'(x)=\mu g\,s(x),\qquad s'(x)=\sqrt{1+y'(x)^2}.
$$

Applying [differentiation](differentiation.md) yields $ay''=\sqrt{1+y'^2}$. The proposed [hyperbolic cosine](hyperbolic-cosine.md) solves this [differential equation](differential-equation-split.md), because $y'=\sinh(x/a)$ and $ay''=\cosh(x/a)=\sqrt{1+\sinh^2(x/a)}$. This is the mechanism behind the shape, under the stated ideal chain assumptions.

The same identity simplifies the [arc length](arc-length.md) between symmetric supports at $x=\pm b$:

$$
L=\int_{-b}^b\sqrt{1+y'(x)^2}\,dx=\int_{-b}^b\cosh(x/a)\,dx=2a\sinh(b/a).
$$

For $a=b=1$, $L\approx2.350402$, exceeding the horizontal span of two. A larger $a$ at fixed $b$ gives a shallower sag: the [Taylor series](taylor-series.md) gives $a(\cosh(x/a)-1)=x^2/(2a)+x^4/(24a^3)+\cdots$. Thus a [parabola](parabola.md) is a local approximation, while the exact ideal chain shape is a [catenary](catenary.md). The useful connection is that the same [hyperbolic Pythagorean identity](hyperbolic-pythagorean-identity.md) controls its coordinates, [force](force-split.md) balance, and [arc length](arc-length.md).

## ↑ Ancestors (9)

1. [Hyperbolic cosine](hyperbolic-cosine.md)
2. [Hyperbolic function](hyperbolic-function.md)
3. [Exponential function](exponential-function.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
