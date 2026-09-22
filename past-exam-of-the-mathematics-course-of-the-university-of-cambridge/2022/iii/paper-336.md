# Paper 336

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_336.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_336.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 336](paper-336.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $L=\log(1/\epsilon)$. Taking logarithms gives $x^2+\log x=L$. Equivalently, $2x^2=W(2/\epsilon^2)$ in terms of the [Lambert W function](../../../analysis.md#lambert-w-function). Iteration for large $L$ gives $x^2=L-\tfrac12\log L+O((\log L)/L)$ and hence

$$
\boxed{x=\sqrt L-\frac{\log L}{4\sqrt L}
+O\left(\frac{(\log L)^2}{L^{3/2}}\right).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $e^x=1+xg(x)$, where $g=(e^x-1)/x$ is smooth at zero. Then

$$
\int_0^1\frac{dx}{\sqrt{x+\epsilon}}
=2-2\sqrt\epsilon+\epsilon+O(\epsilon^2),
$$

and a uniformly integrable expansion gives

$$
\int_0^1\frac{xg(x)}{\sqrt{x+\epsilon}}dx
=\int_0^1\sqrt x,g(x)dx
-\frac\epsilon2\int_0^1\frac{g(x)}{\sqrt x}dx
+O(\epsilon^{3/2}).
$$

By [integration by parts](../../../calculus.md#integration-by-parts),

$$
\int_0^1\frac{e^x-1}{x^{3/2}}dx=-2(e-1)+2I(0).
$$

Therefore

$$
\boxed{I(\epsilon)=I(0)-2\sqrt\epsilon+[e-I(0)]\epsilon+O(\epsilon^{3/2}).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For $F(t)=\operatorname{sech}\alpha\sinh t-t$, the relevant [saddle point](../../../analysis.md#saddle-point) is $t=\alpha$, where $F(\alpha)=\tanh\alpha-\alpha$ and $F''(\alpha)=\tanh\alpha$. The [method of steepest descent](../../../analysis.md#method-of-steepest-descent) gives

$$
\boxed{J_\nu(\nu\operatorname{sech}\alpha)
\sim\frac{\exp[\nu(\tanh\alpha-\alpha)]}
{\sqrt{2\pi\nu\tanh\alpha}}}
\qquad(\alpha>0).
$$

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

At $\alpha=0$, the ordinary saddles coalesce at zero and $\sinh t-t=t^3/6+O(t^5)$. The contributing scale is $t=O(\nu^{-1/3})$. The standard [cubic saddle-point approximation](../../../analysis.md#cubic-saddle-point-approximation) gives

$$
\boxed{J_\nu(\nu)
\sim\frac{2^{1/3}}{3^{2/3}\Gamma(2/3)}\nu^{-1/3}.}
$$

Equivalently, the coefficient is $2^{1/3}\operatorname{Ai}(0)$.

## 2

↑ **Parent:** [Paper 336](paper-336.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Introduce $T=\epsilon t$ and write $x_0=A(T)\cos[t+\theta(T)]$. Averaging

$$
\frac d{dt}\frac{x^2+\dot x^2}{2}=-\epsilon\dot x^4
$$

over one fast period gives $AA_T=-3A^4/8$ and $\theta_T=0$. The initial data therefore give the [method of multiple scales](../../../differential-equation.md#method-of-multiple-scales) result

$$
\boxed{x(t)\sim\frac{\cos t}{\sqrt{1+3\epsilon t/4}}}
$$

through $t=O(\epsilon^{-1})$.

For the replacement damping, $\sin(\dot x)\dot x=\dot x^2-\dot x^4/6+\cdots$ is even in $\dot x$. Every term has zero resonant projection onto the fundamental over a complete orbit, so the $O(\epsilon)$ slow amplitude and phase equations vanish. Thus

$$
\boxed{x(t)=\cos t+O(\epsilon)}
$$

through $t=O(\epsilon^{-1})$: there is no first-order secular damping, although bounded mean and higher-harmonic corrections occur.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For constant width, [separation of variables](../../../partial-differential-equation.md#separation-of-variables) with $\phi=X(x)\sin(n\pi y/h_0)$ gives

$$
X''+k_n^2X=0,
\qquad
\boxed{k_n^2=k_0^2-\frac{n^2\pi^2}{h_0^2}.}
$$

Hence $X=A_ne^{ik_nx}+B_ne^{-ik_nx}$, with imaginary $k_n$ representing an evanescent mode.

For $X=\epsilon x$ and varying width,

$$
k_n(X)^2=k_0^2-\frac{n^2\pi^2}{h(X)^2},
\qquad
\Theta_n=\frac1\epsilon\int_0^Xk_n(\xi)d\xi.
$$

Projection of the next-order equation onto $\sin(n\pi y/h)$, whose squared norm is proportional to $h$, gives

$$
\boxed{2k_nA_n'+\left(k_n'+k_n\frac{h'}h\right)A_n=0,
\qquad
2k_nB_n'+\left(k_n'+k_n\frac{h'}h\right)B_n=0.}
$$

Thus the [WKB amplitude in a slowly varying duct](../../../analysis.md#wkb-amplitude-in-a-slowly-varying-duct) is

$$
\boxed{
A_n(X)=A_n(0)\left[\frac{k_n(0)h(0)}{k_n(X)h(X)}\right]^{1/2},
\quad
B_n(X)=B_n(0)\left[\frac{k_n(0)h(0)}{k_n(X)h(X)}\right]^{1/2}.}
$$

This applies for $n\geq1$ away from turning points $k_n=0$.

## 3

↑ **Parent:** [Paper 336](paper-336.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The reduced outer equation is $(1+x)y_0'+y_0=0$. Imposing the right boundary condition gives

$$
\boxed{y_{\rm out}=\frac2{1+x}
+\epsilon\left[\frac2{(1+x)^3}-\frac1{2(1+x)}\right]+O(\epsilon^2).}
$$

The condition at $x=0$ requires $X=x/\epsilon$. The first two inner terms are

$$
\boxed{Y_0=2-e^{-X},
\qquad
Y_1=-2X+\frac32+\left(\frac{X^2}{2}-\frac32\right)e^{-X}.}
$$

They match $2+\epsilon(-2X+3/2)$. The [additive composite expansion](../../../differential-equation.md#additive-composite-expansion) is

$$
\boxed{
y_{\rm comp}=\frac2{1+x}
+\epsilon\left[\frac2{(1+x)^3}-\frac1{2(1+x)}\right]
-e^{-x/\epsilon}
+\epsilon\left[\frac12\left(\frac x\epsilon\right)^2-\frac32\right]e^{-x/\epsilon}.}
$$

On $[-1,1]$, the coefficient $1+x$ vanishes at the left endpoint. The ordinary $O(\epsilon)$ exponential layer is replaced by a turning-point endpoint region of width $O(\sqrt\epsilon)$, where all three terms in the equation enter the leading balance.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The outer expansion behaves as $f\sim x^{-1}$ near zero. The terms $x$ and $\epsilon f$ become comparable when $x^2=O(\epsilon)$, so

$$
\boxed{x=\sqrt\epsilon X,
\qquad f=\epsilon^{-1/2}F(X).}
$$

The equation has the exact first integral

$$
xf+\frac\epsilon2f^2=x^2+1+2\epsilon,
$$

where the constant follows from $f(1)=2$. Thus

$$
XF+\frac12F^2=1+\epsilon(X^2+2).
$$

Writing $F=F_0+\epsilon F_1+\cdots$ and choosing the branch matching the positive outer solution gives

$$
F_0=\sqrt{X^2+2}-X,
\qquad
F_1=\sqrt{X^2+2}.
$$

Hence

$$
\boxed{f(x)\sim\epsilon^{-1/2}[\sqrt{X^2+2}-X]
+\epsilon^{1/2}\sqrt{X^2+2},
\qquad X=\frac x{\sqrt\epsilon}.}
$$

Its large-$X$ expansion matches the supplied outer series.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
