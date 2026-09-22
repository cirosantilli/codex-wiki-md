<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

At fixed $r$, the leading equation is $(r^2f_0')'=0$. Its solution compatible with the eventual decaying far field and the boundary value at one is $f_0=1/r$. This decay implies $f=O(\epsilon)$ at distances $r=O(\epsilon^{-1})$. Balancing radial [derivatives](../../../../../derivative.md) against the linear screening term identifies

$$
\boxed{\beta=1,\qquad x=\epsilon r.}
$$

The distant region is governed by the [modified Helmholtz equation](../../../../../modified-helmholtz-equation.md); its decaying homogeneous profile is $e^{-x}/x$.

For a [matched asymptotic expansion](../../../../../matched-asymptotic-expansion.md), write the fixed-$r$ approximation as $f=f_0+\epsilon f_1+\epsilon^2f_2+\cdots$, allowing logarithms of $\epsilon$ in the coefficients. Successive equations are

$$
(r^2f_0')'=0,\qquad (r^2f_1')'=0,\qquad (r^2f_2')'=r+1.
$$

The boundary condition imposes $f_0(1)=1$ and $f_1(1)=f_2(1)=0$. Before matching, their integrated forms can be written

$$
f_0=\frac1r,\qquad f_1=C_1\left(1-\frac1r\right),\qquad f_2=\frac r2+\log r+D-\frac{D+1/2}{r}.
$$

In particular a pure power series with parameter-independent coefficients will be insufficient: the [logarithmic overlap creates a switchback term](../../../../../logarithmic-overlap-creates-a-switchback-term.md).

In the distant region set $f=\epsilon F_0(x)+\epsilon^2F_1(x)+\cdots$. The scaled equation is $f_{xx}+2f_x/x-f=xf^3/\epsilon$, so

$$
F_0''+\frac2xF_0'-F_0=0,\qquad F_1''+\frac2xF_1'-F_1=\frac{e^{-3x}}{x^2}.
$$

Decay and leading matching give $F_0=e^{-x}/x$. The [radial modified Helmholtz equation](../../../../../radial-modified-helmholtz-equation.md) gives the supplied particular integral in terms of the [exponential integral](../../../../../exponential-integral.md):

$$
F_1(x)=\alpha\frac{e^{-x}}x+\frac{e^{-x}E_1(2x)-e^xE_1(4x)}{2x}.
$$

As $x\downarrow0$, the [small-argument expansion of the exponential integral](../../../../../small-argument-expansion-of-the-exponential-integral.md) yields

$$
F_1(x)=\frac{\alpha+\tfrac12\log2}{x}+\log x-\alpha+\tfrac32\log2+\gamma-1+O(x\log x),
$$

where $\gamma$ is the [Euler--Mascheroni constant](../../../../../euler-s-constant.md). Substitute $x=\epsilon r$ to compare the two expansions in $1\ll r\ll\epsilon^{-1}$:

$$
\epsilon F_0+\epsilon^2F_1=\frac1r-\epsilon+\epsilon^2\frac r2+\frac{\epsilon}{r}\left(\alpha+\tfrac12\log2\right)+\epsilon^2\left[\log r+\log\epsilon-\alpha+\tfrac32\log2+\gamma-1\right]+\cdots.
$$

The constant at order $\epsilon$ fixes $C_1=-1$. Its $1/r$ coefficient then fixes $\alpha+\tfrac12\log2=1$, and the constant at order $\epsilon^2$ fixes $D$. Hence

$$
\boxed{\alpha=1-\tfrac12\log2,\qquad D=\log\epsilon+2\log2+\gamma-2.}
$$

The required [inner expansion](../../../../../inner-expansion.md) at fixed $r$ is

$$
\boxed{f=\frac1r+\epsilon\left(\frac1r-1\right)+\epsilon^2\left[\frac{r-r^{-1}}2+\log r+\left(\log\epsilon+2\log2+\gamma-2\right)\left(1-\frac1r\right)\right]+o(\epsilon^2).}
$$

At fixed positive $x=\epsilon r$, the [outer expansion](../../../../../outer-expansion.md) is

$$
\boxed{f=\epsilon\frac{e^{-x}}x+\epsilon^2\left[\left(1-\tfrac12\log2\right)\frac{e^{-x}}x+\frac{e^{-x}E_1(2x)-e^xE_1(4x)}{2x}\right]+o(\epsilon^2).}
$$

Both display every term through the requested order, including the $\epsilon^2\log\epsilon$ [switchback term](../../../../../switchback-term.md) in the fixed-$r$ region.

To form an [additive composite expansion](../../../../../additive-composite-expansion.md), subtract the common overlap from the sum of the inner and outer expressions. Their retained common part is

$$
f_{\rm overlap}=\frac1r+\epsilon\left(\frac1r-1\right)+\epsilon^2\left[\frac r2+\log r+D\right].
$$

Thus one composite is $\epsilon F_0(\epsilon r)+\epsilon^2F_1(\epsilon r)-\epsilon^2(D+1/2)/r$. The last term can be screened by multiplying it by $e^{-\epsilon r}$ without changing either retained expansion. This gives a useful exponentially decaying version:

$$
\boxed{f_{\rm comp}(r)=\frac{e^{-\epsilon r}}r\left[1-\epsilon^2(D+1/2)\right]+\epsilon^2F_1(\epsilon r).}
$$

Its boundary value is $1+o(\epsilon^2)$. If exact satisfaction of the boundary value is desired, use instead

$$
f_{\rm comp}^{\rm normalized}(r)=\left[1-\epsilon^2F_1(\epsilon)\right]\frac{e^{-\epsilon(r-1)}}r+\epsilon^2F_1(\epsilon r).
$$

The [small-argument expansion of the exponential integral](../../../../../small-argument-expansion-of-the-exponential-integral.md) shows that this normalized composite has the same two retained expansions; it equals one at $r=1$ and tends to zero at infinity.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 336](../../paper-336-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
