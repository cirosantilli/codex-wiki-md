# Paper 2

↑ **Parent:** [2008](../2008.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2008/PaperNST_IA_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2008/PaperNST_IA_2.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)
- [8](#8)
  - [i](#8/i)
    - [Solution](#8/i/solution)
  - [ii](#8/ii)
    - [Solution](#8/ii/solution)
- [9](#9)
  - [i](#9/i)
    - [Solution](#9/i/solution)
  - [ii](#9/ii)
    - [Solution](#9/ii/solution)
- [10](#10)
  - [Solution](#10/solution)
- [11](#11)
  - [a](#11/a)
    - [i](#11/a/i)
      - [Solution](#11/a/i/solution)
    - [ii](#11/a/ii)
      - [Solution](#11/a/ii/solution)
  - [b](#11/b)
    - [Solution](#11/b/solution)
  - [c](#11/c)
    - [Solution](#11/c/solution)
  - [d](#11/d)
    - [i](#11/d/i)
      - [Solution](#11/d/i/solution)
    - [ii](#11/d/ii)
      - [Solution](#11/d/ii/solution)
    - [iii](#11/d/iii)
      - [Solution](#11/d/iii/solution)
    - [iv](#11/d/iv)
      - [Solution](#11/d/iv/solution)
- [12](#12)
  - [Solution](#12/solution)
- [13](#13)
  - [i](#13/i)
    - [Solution](#13/i/solution)
  - [ii](#13/ii)
    - [Solution](#13/ii/solution)
  - [iii](#13/iii)
    - [Solution](#13/iii/solution)
- [14](#14)
  - [a](#14/a)
    - [Solution](#14/a/solution)
  - [b](#14/b)
    - [i](#14/b/i)
      - [Solution](#14/b/i/solution)
    - [ii](#14/b/ii)
      - [Solution](#14/b/ii/solution)
- [15](#15)
  - [a](#15/a)
    - [i](#15/a/i)
      - [Solution](#15/a/i/solution)
    - [ii](#15/a/ii)
      - [Solution](#15/a/ii/solution)
  - [b](#15/b)
    - [i](#15/b/i)
      - [Solution](#15/b/i/solution)
    - [ii](#15/b/ii)
      - [Solution](#15/b/ii/solution)
- [16](#16)
  - [a](#16/a)
    - [i](#16/a/i)
      - [Solution](#16/a/i/solution)
    - [ii](#16/a/ii)
      - [Solution](#16/a/ii/solution)
    - [iii](#16/a/iii)
      - [Solution](#16/a/iii/solution)
    - [iv](#16/a/iv)
      - [Solution](#16/a/iv/solution)
  - [b](#16/b)
    - [i](#16/b/i)
      - [Solution](#16/b/i/solution)
    - [ii](#16/b/ii)
      - [Solution](#16/b/ii/solution)
- [17](#17)
  - [a](#17/a)
    - [Solution](#17/a/solution)
  - [b](#17/b)
    - [Solution](#17/b/solution)
  - [c](#17/c)
    - [Solution](#17/c/solution)
- [18](#18)
  - [a](#18/a)
    - [Solution](#18/a/solution)
  - [b](#18/b)
    - [Solution](#18/b/solution)
  - [c](#18/c)
    - [Solution](#18/c/solution)
- [19](#19)
  - [a](#19/a)
    - [Solution](#19/a/solution)
  - [b](#19/b)
    - [Solution](#19/b/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [dot product](../../inner-product.md#dot-product) is $\boldsymbol a\cdot\boldsymbol b=2-1+2=3$, and both [vectors](../../vector-space.md#vector) have length $\sqrt6$. The [angle between vectors](../../inner-product.md#angle-between-vectors) therefore satisfies $\cos\theta=3/6=1/2$, giving

$$
\boxed{\theta=\pi/3.}
$$

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [derivative](../../calculus.md#derivative) of $\tan x$ is $1/\cos^2x$. The [fundamental theorem of calculus](../../calculus.md#fundamental-theorem-of-calculus) gives

$$
\boxed{\int_0^{\pi/4}\frac{dx}{\cos^2x}=\tan(\pi/4)-\tan0=1.}
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The integrand is an [odd function](../../calculus.md#odd-function), because $x$ is odd and $\cos x$ is even. Its integral over the symmetric interval is therefore

$$
\boxed{0.}
$$

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The denominator $D=x^2+xy+y^2=(x+y/2)^2+3y^2/4$ is positive away from the origin. The [partial derivatives](../../multivariable-calculus.md#partial-derivative) are

$$
f_x=\frac{y(y^2-x^2)}{D^2},\qquad f_y=\frac{x(x^2-y^2)}{D^2}.
$$

They both vanish exactly on

$$
\boxed{y=x\quad\text{and}\quad y=-x,\qquad(x,y)\ne(0,0).}
$$

These are lines of [stationary points](../../calculus-of-variations.md#stationary-point), with values $1/3$ and $-1$, respectively.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Differentiate the sum of squares in [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system):

$$
\boxed{\nabla(r^2)=(2x,2y,2z)=2\boldsymbol r.}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The [product rule for divergence](../../multivariable-calculus.md#product-rule-for-divergence) gives $\nabla\cdot(r^2\boldsymbol r)=\nabla(r^2)\cdot\boldsymbol r+r^2\nabla\cdot\boldsymbol r$. Since $\nabla\cdot\boldsymbol r=3$, the result is

$$
\boxed{\nabla\cdot(r^2\boldsymbol r)=5r^2.}
$$

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Multiply numerator and denominator by the [complex conjugate](../../complex-analysis.md#complex-conjugate) of $1-i$:

$$
\frac{1+i}{1-i}=\frac{(1+i)^2}2=i.
$$

Thus the [real part](../../complex-analysis.md#real-part) and [imaginary part](../../complex-analysis.md#imaginary-part) are respectively

$$
\boxed{0,\qquad1.}
$$

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is $(1/2-\lambda)(-1/2-\lambda)-2=\lambda^2-9/4$. Its two [roots](../../semisimple-lie-algebra.md#root-of-a-root-system) give the [eigenvalues](../../linear-operator-theory.md#eigenvalue)

$$
\boxed{\lambda=\frac32,\quad-\frac32.}
$$

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

The [Maclaurin series](../../calculus.md#maclaurin-series) $\cos x=1-x^2/2+O(x^4)$ gives $e^{\cos x}=e\exp(-x^2/2+O(x^4))$. The first two nonzero terms are therefore

$$
\boxed{e^{\cos x}=e-\frac e2x^2+O(x^4).}
$$

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/i">i</h3>

↑ **Parent:** [8](#8)

<h4 id="8/i/solution">Solution</h4>

↑ **Parent:** [I](#8/i)

The proposed function has [partial derivatives](../../multivariable-calculus.md#partial-derivative) $u_t=1$ and $u_{xx}=2\alpha$. Substitution in the [heat equation](../../diffusion-equation.md#heat-equation) requires $1=\alpha$, hence

$$
\boxed{\alpha=1.}
$$

The coefficient $\beta$ remains arbitrary.

<h3 id="8/ii">ii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8/ii)

Within this polynomial family, $u(0,0)=0$ already holds and $u(1,0)=1+\beta=0$ gives $\beta=-1$. Thus one solution is

$$
\boxed{u(x,t)=x^2-x+t.}
$$

Two specified point values alone do not give uniqueness among all solutions of the [heat equation](../../diffusion-equation.md#heat-equation).

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/i">i</h3>

↑ **Parent:** [9](#9)

<h4 id="9/i/solution">Solution</h4>

↑ **Parent:** [I](#9/i)

For a [uniform distribution](../../continuous-probability-distribution.md#continuous-uniform-distribution) on the unit square, probability is the ratio of [areas](../../differential-geometry.md#surface-area). The [incircle](../../euclidean-geometry.md#incircle-of-a-triangle) has radius $1/2$, so

$$
\boxed{P(\text{inside circle})=\frac{\pi(1/2)^2}{1}=\frac\pi4.}
$$

<h3 id="9/ii">ii</h3>

↑ **Parent:** [9](#9)

<h4 id="9/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9/ii)

Conditioned on being inside the [circle](../../topology.md#circle), the point is a [uniform random point in a disk](../../probability-theory.md#uniform-random-point-in-a-disk) of radius $1/2$. The annulus from $r$ to $r+dr$ has area $2\pi r\,dr+O(dr^2)$. Dividing by the disk's area gives

$$
\boxed{P(r<R<r+dr\mid R<1/2)=8r\,dr+O(dr^2),\qquad0\leq r<1/2.}
$$

The radial [probability density function](../../continuous-probability-distribution.md#probability-density-function) is $8r$ on $[0,1/2]$ and integrates to one. Without conditioning, the corresponding annulus probability for a point in the original square is $2\pi r\,dr+O(dr^2)$.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

Write $\boldsymbol\Delta=\boldsymbol d-\boldsymbol b$. At an intersection, $\boldsymbol\Delta=\lambda\boldsymbol a-\mu\boldsymbol c$, so its [scalar triple product](../../multilinear-algebra.md#scalar-triple-product) with $\boldsymbol a,\boldsymbol c$ vanishes. The expression in the question is exactly

$$
\boldsymbol a\cdot(\boldsymbol c\times\boldsymbol d)+\boldsymbol c\cdot(\boldsymbol a\times\boldsymbol b)
=\boldsymbol\Delta\cdot(\boldsymbol a\times\boldsymbol c)=0.
$$

Under a shift of origin by $\boldsymbol h$, the direction vectors $\boldsymbol a,\boldsymbol c$ stay fixed, while $\boldsymbol b,\boldsymbol d$ both change by $-\boldsymbol h$. Thus $\boldsymbol\Delta$ and the condition are invariant. For nonparallel lines this is also sufficient for intersection; for parallel lines it only asserts coplanarity and need not imply intersection.

Put $\delta\lambda=\lambda_2-\lambda_1$ and $\delta\mu=\mu_2-\mu_1$. Then $\boldsymbol x_2-\boldsymbol x_1=\delta\lambda\boldsymbol a$ and $\boldsymbol x_4-\boldsymbol x_1=(\boldsymbol x_3-\boldsymbol x_1)+\delta\mu\boldsymbol c$. Bilinearity of the [cross product](../../vector-space.md#cross-product) gives

$$
\begin{aligned}
[(\boldsymbol x_3-\boldsymbol x_1)\times(\boldsymbol x_4-\boldsymbol x_1)]\cdot(\boldsymbol x_2-\boldsymbol x_1)
&=\delta\mu\,\delta\lambda\,[(\boldsymbol\Delta+\mu_1\boldsymbol c-\lambda_1\boldsymbol a)\times\boldsymbol c]\cdot\boldsymbol a\\
&=-\delta\mu\,\delta\lambda\,\boldsymbol\Delta\cdot(\boldsymbol a\times\boldsymbol c)\\
&=\boldsymbol\Delta\cdot[(\boldsymbol x_4-\boldsymbol x_3)\times(\boldsymbol x_2-\boldsymbol x_1)].
\end{aligned}
$$

The [tetrahedron](../../euclidean-geometry.md#tetrahedron) volume is one sixth of the [absolute value](../../real-analysis.md#absolute-value) of this triple product. Sliding either vertex pair along its line preserves $|\delta\lambda|$ or $|\delta\mu|$, because its separation is fixed and the direction vectors are fixed. Thus the volume is unchanged, including the zero-volume coplanar case. This is [tetrahedron volume under sliding opposite edges](../../euclidean-geometry.md#tetrahedron-volume-under-sliding-opposite-edges).

## 11

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11/a">a</h3>

↑ **Parent:** [11](#11)

<h4 id="11/a/i">i</h4>

↑ **Parent:** [A](#11/a)

<h5 id="11/a/i/solution">Solution</h5>

↑ **Parent:** [I](#11/a/i)

Every set of $S$ students is equally likely to be the specified college. There are $\binom NS$ choices in total and $\binom LS$ choices consisting entirely of the specified group. Therefore the [hypergeometric distribution](../../discrete-probability-distribution.md#hypergeometric-distribution) gives

$$
\boxed{P(\text{all lazy})=\frac{\binom LS}{\binom NS}.}
$$

<h4 id="11/a/ii">ii</h4>

↑ **Parent:** [A](#11/a)

<h5 id="11/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11/a/ii)

Choose $n$ students from the $L$ lazy students and $S-n$ from the other $N-L$. Dividing by the total number of possible college memberships gives

$$
\boxed{P(n\text{ lazy})=\frac{\binom Ln\binom{N-L}{S-n}}{\binom NS},\qquad0\leq n\leq S.}
$$

The assumptions ensure all these values are possible. This sampling is without replacement, as required by the [hypergeometric distribution](../../discrete-probability-distribution.md#hypergeometric-distribution).

<h3 id="11/b">b</h3>

↑ **Parent:** [11](#11)

<h4 id="11/b/solution">Solution</h4>

↑ **Parent:** [B](#11/b)

By symmetry, each student in the university has probability $(S/N)(1/S)=1/N$ of being in the college and then selected. Hence the [prior probability](../../bayesian-statistics.md#prior-probability) is

$$
\boxed{P(\text{lazy})=L/N.}
$$

<h3 id="11/c">c</h3>

↑ **Parent:** [11](#11)

<h4 id="11/c/solution">Solution</h4>

↑ **Parent:** [C](#11/c)

The lecture attendances are independent [Bernoulli trials](../../discrete-probability-distribution.md#bernoulli-trial) with success probability $f$. Their count has the [binomial distribution](../../discrete-probability-distribution.md#binomial-distribution):

$$
\boxed{P(k\mid K,f)=\binom Kk f^k(1-f)^{K-k},\qquad0\leq k\leq K.}
$$

<h3 id="11/d">d</h3>

↑ **Parent:** [11](#11)

<h4 id="11/d/i">i</h4>

↑ **Parent:** [D](#11/d)

<h5 id="11/d/i/solution">Solution</h5>

↑ **Parent:** [I](#11/d/i)

Here “absent” denotes absence at both observed lectures. The assumed [independence](../../random-variable.md#independent-random-variables) makes its [conditional probability](../../probability-theory.md#conditional-probability)

$$
\boxed{P(\text{absent}\mid\text{lazy})=(1-1/2)^2=1/4.}
$$

<h4 id="11/d/ii">ii</h4>

↑ **Parent:** [D](#11/d)

<h5 id="11/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11/d/ii)

For attendance probability $9/10$, absence on both independent observations has [conditional probability](../../probability-theory.md#conditional-probability)

$$
\boxed{P(\text{absent}\mid\text{diligent})=(1-9/10)^2=1/100.}
$$

<h4 id="11/d/iii">iii</h4>

↑ **Parent:** [D](#11/d)

<h5 id="11/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#11/d/iii)

The [law of total probability](../../probability-space.md#law-of-total-probability) over the two student groups gives

$$
P(\text{absent})=\frac14\frac LN+\frac1{100}\left(1-\frac LN\right),
\qquad\boxed{P(\text{absent})=\frac{24L+N}{100N}.}
$$

<h4 id="11/d/iv">iv</h4>

↑ **Parent:** [D](#11/d)

<h5 id="11/d/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#11/d/iv)

The [prior probability](../../bayesian-statistics.md#prior-probability) is $1/10$. Using [Bayes' theorem](../../probability-theory.md#bayes-theorem), the [posterior probability](../../bayesian-statistics.md#posterior-probability) after two absences is

$$
\boxed{P(\text{lazy}\mid\text{absent})=\frac{(1/4)(1/10)}{(1/4)(1/10)+(1/100)(9/10)}=\frac{25}{34}\approx0.7353.}
$$

Thus the probability rises from **10% to about 73.5%** within the assumed attendance model. Two absences are 25 times as likely under the lazy model, overcoming the prior odds of $1:9$; they still do not make the classification certain.

## 12

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12/solution">Solution</h3>

↑ **Parent:** [12](#12)

The integrand is even and decays at both infinity and zero, since $a,b>0$. On $x>0$ set $u=\sqrt a\,x-\sqrt b/x$, a strictly increasing bijection onto the whole real line. Then

$$
ax^2+b/x^2=u^2+2\sqrt{ab},\qquad
x=\frac{u+\sqrt{u^2+4\sqrt{ab}}}{2\sqrt a},\qquad
\frac{dx}{du}=\frac1{2\sqrt a}\left(1+\frac u{\sqrt{u^2+4\sqrt{ab}}}\right).
$$

Using evenness for the negative half-axis gives

$$
I(a,b)=\frac{e^{-\sqrt{ab}}}{\sqrt a}\int_{-\infty}^{\infty}e^{-u^2/2}\left(1+\frac u{\sqrt{u^2+4\sqrt{ab}}}\right)du.
$$

The second summand is an integrable [odd function](../../calculus.md#odd-function), so its integral vanishes. The remaining [Gaussian integral](../../integral.md#gaussian-integral) gives

$$
\boxed{I(a,b)=\sqrt{\frac{2\pi}a}\,e^{-\sqrt{ab}}.}
$$

For the second integral use $x=1/t$ separately on each half-axis. The factor $x^{-2}dx$ becomes $-dt$, and reversing the transformed limits yields $J(a,b)=I(b,a)$. Thus

$$
\boxed{J(a,b)=\sqrt{\frac{2\pi}b}\,e^{-\sqrt{ab}}.}
$$

These identities are instances of the [Gaussian integral with an inverse-square term](../../integral.md#gaussian-integral-with-an-inverse-square-term). Splitting at zero before either [change of variables](../../multivariable-calculus.md#change-of-variables-formula) avoids treating a discontinuous transformation as a single bijection.

## 13

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13/i">i</h3>

↑ **Parent:** [13](#13)

<h4 id="13/i/solution">Solution</h4>

↑ **Parent:** [I](#13/i)

The [characteristic equation](../../linear-ordinary-differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation) $(r-3)(r-4)=0$ gives complementary terms $Ce^{3x}+De^{4x}$. A linear [particular solution](../../linear-ordinary-differential-equation.md#particular-solution) is $12x+7$, since its substitution gives $144x$. The initial conditions give $C+D=-7$ and $3C+4D=-12$, hence

$$
\boxed{y=12x+7-16e^{3x}+9e^{4x}.}
$$

<h3 id="13/ii">ii</h3>

↑ **Parent:** [13](#13)

<h4 id="13/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#13/ii)

The complementary [characteristic roots](../../differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) are $-1,-2$. Substituting $A\sin x+B\cos x$ into the differential operator gives $(A-3B)\sin x+(3A+B)\cos x$, so a [particular solution](../../linear-ordinary-differential-equation.md#particular-solution) is $\sin x-3\cos x$. The initial conditions then require $C+D=3$ and $C+2D=1$, giving

$$
\boxed{y=\sin x-3\cos x+5e^{-x}-2e^{-2x}.}
$$

<h3 id="13/iii">iii</h3>

↑ **Parent:** [13](#13)

<h4 id="13/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#13/iii)

The repeated [characteristic root](../../differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) is $-1$, matching the exponential forcing. Put $y=e^{-x}w$; then $y''+2y'+y=e^{-x}w''$, so $w''=8$. The zero initial conditions give $w(0)=w'(0)=0$, hence

$$
\boxed{y=4x^2e^{-x}.}
$$

The extra quadratic factor is the [resonance](../../dynamical-systems.md#resonance) associated with the double root.

## 14

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14/a">a</h3>

↑ **Parent:** [14](#14)

<h4 id="14/a/solution">Solution</h4>

↑ **Parent:** [A](#14/a)

Put $\xi=x-vt$ and $U(\xi)=A\operatorname{sech}^2\xi$. For $A\ne0$, differentiation gives $U''=4U-6U^2/A$ and therefore $U^{(3)}=4U'-(12/A)UU'$. The [Korteweg-De Vries equation](../../integrable-systems.md#korteweg-de-vries-equation) reduces to

$$
(4-v)U'-\left(6+\frac{12}A\right)UU'=0.
$$

Since $U$ is nonconstant, both coefficients must vanish. Thus the nonzero [solitary wave](../../analysis.md#solitary-wave) is

$$
\boxed{A=-2,\qquad v=4,\qquad u=-2\operatorname{sech}^2(x-4t).}
$$

There is also the trivial solution $A=0$, for which $v$ has no effect. The negative amplitude follows from the minus sign of the nonlinear term; it agrees with the [sech-squared solitary wave of the KdV equation](../../integrable-systems.md#sech-squared-solitary-wave-of-the-kdv-equation).

<a id="14/a/image-a-negative-solitary-wave-translates-to-the-right-without-changing-its-profile"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2-negative-kdv-soliton.png)

**[Figure 1](#14/a/image-a-negative-solitary-wave-translates-to-the-right-without-changing-its-profile). A negative solitary wave translates to the right without changing its profile**.

<h3 id="14/b">b</h3>

↑ **Parent:** [14](#14)

<h4 id="14/b/i">i</h4>

↑ **Parent:** [B](#14/b)

<h5 id="14/b/i/solution">Solution</h5>

↑ **Parent:** [I](#14/b/i)

Differentiate the equation for $f$ with respect to $x$, commuting mixed [partial derivatives](../../multivariable-calculus.md#partial-derivative) for a sufficiently smooth solution. With $y=f_x$ this gives

$$
f_{xt}+f_xf_{xx}=kf_{xxx},\qquad\boxed{y_t+yy_x=ky_{xx}.}
$$

This is the [viscous Burgers equation](../../partial-differential-equation.md#viscous-burgers-equation) when $k>0$.

<h4 id="14/b/ii">ii</h4>

↑ **Parent:** [B](#14/b)

<h5 id="14/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#14/b/ii)

For $k\ne0$, the [chain rule](../../calculus.md#chain-rule) gives $g_t=-f_tg/(2k)$ and $g_{xx}=(-f_{xx}/(2k)+f_x^2/(4k^2))g$. Consequently

$$
g_t-kg_{xx}=-\frac g{2k}\left(f_t+\frac12f_x^2-kf_{xx}\right)=0.
$$

Thus

$$
\boxed{g_t=kg_{xx}.}
$$

This is the potential form of the [Cole-Hopf transformation](../../partial-differential-equation.md#cole-hopf-transformation), with $y=-2k\,g_x/g$. For $k>0$ it is a forward [diffusion equation](../../diffusion-equation.md); at $k=0$ the exponential transformation is undefined, while negative $k$ gives a backward heat equation.

## 15

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15/a">a</h3>

↑ **Parent:** [15](#15)

<h4 id="15/a/i">i</h4>

↑ **Parent:** [A](#15/a)

<h5 id="15/a/i/solution">Solution</h5>

↑ **Parent:** [I](#15/a/i)

Integrating the first component in $x$ gives $\phi=x^3y+h(y,z)$. Matching the second requires $h_y=-2yz^2$, so $h=-y^2z^2+k(z)$. Matching the third gives $k'=0$. Thus the field is [conservative](../../multivariable-calculus.md#conservative-vector-field), with [scalar potential](../../classical-field-theory.md#scalar-potential)

$$
\boxed{\phi=x^3y-y^2z^2+C.}
$$

Direct differentiation verifies $\boldsymbol F_1=\nabla\phi$ on all of $\mathbb R^3$.

<h4 id="15/a/ii">ii</h4>

↑ **Parent:** [A](#15/a)

<h5 id="15/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#15/a/ii)

The [curl](../../multivariable-calculus.md#curl) is $\nabla\times\boldsymbol F_2=(2z,3z^2,0)$, which is not identically zero. A gradient of a smooth [scalar potential](../../classical-field-theory.md#scalar-potential) has zero [curl](../../multivariable-calculus.md#curl), so $\boldsymbol F_2$ is **not conservative** on $\mathbb R^3$.

<h3 id="15/b">b</h3>

↑ **Parent:** [15](#15)

<h4 id="15/b/i">i</h4>

↑ **Parent:** [B](#15/b)

<h5 id="15/b/i/solution">Solution</h5>

↑ **Parent:** [I](#15/b/i)

On the first segment, $x=z=0$, so both [line integrals](../../multivariable-calculus.md#line-integral) vanish. On the second, $y=1,z=0$, giving contributions $\int_0^23x^2dx=8$ and $\int_0^22x\,dx=4$. On the last, $x=2,y=1$, the contributions are $\int_0^3-2z\,dz=-9$ and $\int_0^3-6z^2dz=-54$. Therefore

$$
\boxed{\int\boldsymbol F_1\cdot d\boldsymbol r=-1,\qquad\int\boldsymbol F_2\cdot d\boldsymbol r=-50.}
$$

The first also equals $\phi(B)-\phi(A)=8-9=-1$, as the [fundamental theorem for line integrals](../../multivariable-calculus.md#fundamental-theorem-for-line-integrals) predicts.

<h4 id="15/b/ii">ii</h4>

↑ **Parent:** [B](#15/b)

<h5 id="15/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#15/b/ii)

The [parametric curve](../../topology.md#parametric-curve) runs from $t=0$ to $t=1$, with $\boldsymbol r'=(2,3t^2,6t)$. Substitution into the two [line integrals](../../multivariable-calculus.md#line-integral) gives

$$
\boldsymbol F_1(\boldsymbol r(t))\cdot\boldsymbol r'=48t^5-90t^9,\qquad
\boldsymbol F_2(\boldsymbol r(t))\cdot\boldsymbol r'=20t^4-351t^6.
$$

Hence

$$
\boxed{\int\boldsymbol F_1\cdot d\boldsymbol r=-1,\qquad\int\boldsymbol F_2\cdot d\boldsymbol r=-\frac{323}7.}
$$

The first is unchanged because the field is [conservative](../../multivariable-calculus.md#conservative-vector-field). The two different answers for the second exhibit its path dependence, consistent with its nonzero [curl](../../multivariable-calculus.md#curl).

## 16

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16/a">a</h3>

↑ **Parent:** [16](#16)

<h4 id="16/a/i">i</h4>

↑ **Parent:** [A](#16/a)

<h5 id="16/a/i/solution">Solution</h5>

↑ **Parent:** [I](#16/a/i)

The [permutation matrix](../../vector-space.md#permutation-matrix) acts by $A(x,y,z)^T=(y,z,x)^T$. Applying this cyclic permutation three times returns every [vector](../../vector-space.md#vector) to itself, proving $A^3=I$. Explicitly $A^2=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}$ and multiplication once more gives the [identity matrix](../../vector-space.md#identity-matrix).

<h4 id="16/a/ii">ii</h4>

↑ **Parent:** [A](#16/a)

<h5 id="16/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#16/a/ii)

Using $A^3=I$, the matrix power reduces modulo three:

$$
\boxed{A^{3n+2}=A^2=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}.}
$$

<h4 id="16/a/iii">iii</h4>

↑ **Parent:** [A](#16/a)

<h5 id="16/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#16/a/iii)

Since $A^2A=A^3=I=AA^2$, the [inverse matrix](../../matrix-inverse.md) is

$$
\boxed{(A^2)^{-1}=A.}
$$

<h4 id="16/a/iv">iv</h4>

↑ **Parent:** [A](#16/a)

<h5 id="16/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#16/a/iv)

Here $A^{3n+1}=A$, so its [inverse matrix](../../matrix-inverse.md) is

$$
\boxed{(A^{3n+1})^{-1}=A^2.}
$$

<h3 id="16/b">b</h3>

↑ **Parent:** [16](#16)

<h4 id="16/b/i">i</h4>

↑ **Parent:** [B](#16/b)

<h5 id="16/b/i/solution">Solution</h5>

↑ **Parent:** [I](#16/b/i)

With $\nu=0$, the [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) factors into $(1-\lambda)[\lambda^2-\lambda-(\mu^2+4)]$, up to the overall sign convention. The [eigenvalues](../../linear-operator-theory.md#eigenvalue) are $1$ and $(1\pm\sqrt{17+4\mu^2})/2$. Integer values require an odd integer $m$ satisfying $(m-2\mu)(m+2\mu)=17$. The positive integer factorization $17=1\cdot17$ forces $m=9$ and

$$
\boxed{\mu=4.}
$$

The resulting [eigenvalues](../../linear-operator-theory.md#eigenvalue) and corresponding nonzero [eigenvectors](../../linear-operator-theory.md#eigenvector) are

$$
\boxed{\begin{array}{c|c}1&(2,0,-1)^T\\5&(1,2,2)^T\\-4&(2,-5,4)^T\end{array}.}
$$

Any nonzero scalar multiple is equally valid. The factorization also shows that no other positive integer $\mu$ works.

<h4 id="16/b/ii">ii</h4>

↑ **Parent:** [B](#16/b)

<h5 id="16/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#16/b/ii)

For $\nu=5$, $B$ is real symmetric. [Sylvester's criterion](../../quadratic-form.md#sylvester-s-criterion) says that all [eigenvalues](../../linear-operator-theory.md#eigenvalue) are positive exactly when its leading principal [matrix minors](../../vector-space.md#minor-linear-algebra) are positive. These are $1$, $5-4=1$, and $\det B=1-\mu^2$. Therefore

$$
\boxed{-1<\mu<1.}
$$

At either endpoint one [eigenvalue](../../linear-operator-theory.md#eigenvalue) is zero, so the strict positivity requirement excludes it.

## 17

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17/a">a</h3>

↑ **Parent:** [17](#17)

<h4 id="17/a/solution">Solution</h4>

↑ **Parent:** [A](#17/a)

Every harmonic in this [Fourier series](../../fourier-series.md) has period $2L$. Since the first-harmonic coefficient is nonzero, the fundamental [period](../../mathematics.md#period-of-a-function) cannot be smaller: translating by a period $T$ must multiply that nonzero complex coefficient by $e^{i\pi T/L}=1$. Thus, taking $L>0$,

$$
\boxed{T=2L.}
$$

<h3 id="17/b">b</h3>

↑ **Parent:** [17](#17)

<h4 id="17/b/solution">Solution</h4>

↑ **Parent:** [B](#17/b)

Write $h_n=a_n\cos(n\pi x/L)+b_n\sin(n\pi x/L)$. For the partial sum $S_N=a_0/2+\sum_{n=1}^Nh_n$, ordinary multiplication gives

$$
S_N^2=\frac{a_0^2}4+a_0\sum_{n=1}^Nh_n+\sum_{m,n=1}^Nh_mh_n.
$$

On $[-L,L]$, the integrals of every nonconstant sine or cosine vanish. [Fourier orthogonality](../../fourier-series.md#fourier-orthogonality) further gives $\int\cos(m\pi x/L)\cos(n\pi x/L)dx=L\delta_{mn}$ and the same identity for two sines, while every sine-cosine integral is zero. Thus

$$
\frac1{2L}\int_{-L}^LS_N^2dx=\frac{a_0^2}4+\frac12\sum_{n=1}^N(a_n^2+b_n^2).
$$

For square-integrable $f$, its [Fourier partial sums](../../fourier-series.md#fourier-partial-sum) converge to $f$ in [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space), so their squared norms converge to the squared norm of $f$. Passing to the limit proves [Parseval's identity](../../fourier-analysis.md#parseval-identity):

$$
\boxed{\frac1T\int_{-T/2}^{T/2}f(x)^2dx=\left(\frac{a_0}2\right)^2+\frac12\sum_{n=1}^{\infty}(a_n^2+b_n^2).}
$$

Working with finite partial sums before taking the norm limit avoids an unjustified interchange of an infinite double series and integration.

<h3 id="17/c">c</h3>

↑ **Parent:** [17](#17)

<h4 id="17/c/solution">Solution</h4>

↑ **Parent:** [C](#17/c)

The periodic ramp is an [odd function](../../calculus.md#odd-function), so $a_0=a_n=0$. [Integration by parts](../../calculus.md#integration-by-parts) gives

$$
b_n=\frac2\pi\int_0^\pi x\sin(nx)\,dx=\frac{2(-1)^{n+1}}n.
$$

Thus the [Fourier series of a periodic sawtooth](../../fourier-series.md#fourier-series-of-a-periodic-sawtooth) is

$$
\boxed{x=2\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}n\sin(nx),\qquad-\pi<x<\pi.}
$$

The periodic function is smooth at $x=\pi/2$, so the [Dirichlet-Jordan convergence theorem](../../fourier-series.md#dirichlet-jordan-convergence-theorem) permits evaluation there. Even-index terms vanish and odd-index sines alternate in sign, giving

$$
\boxed{1-\frac13+\frac15-\frac17+\cdots=\frac\pi4.}
$$

## 18

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18/a">a</h3>

↑ **Parent:** [18](#18)

<h4 id="18/a/solution">Solution</h4>

↑ **Parent:** [A](#18/a)

For a bounded region $V$ with piecewise smooth closed boundary $S$, outward unit [normal vector](../../differential-geometry.md#normal-vector) $\boldsymbol n$ and continuously differentiable [vector field](../../multivariable-calculus.md#vector-field) $\boldsymbol F$, the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) states $\int_S\boldsymbol F\cdot\boldsymbol n\,dS=\int_V\nabla\cdot\boldsymbol F\,dV$. Here $dS$ is scalar [surface area](../../differential-geometry.md#surface-area), $dV$ is [volume](../../geometry-and-topology.md#volume), and $d\boldsymbol S=\boldsymbol n\,dS$ is the oriented [area element](../../differential-geometry.md#area-element-of-a-surface).

For $\boldsymbol F=\boldsymbol r$, its [divergence](../../multivariable-calculus.md#divergence) is three. The [ellipsoid](../../euclidean-geometry.md#ellipsoid) has semiaxes $a,a,b$, so its [volume](../../geometry-and-topology.md#volume) is $4\pi a^2b/3$, obtained by scaling the unit ball. Consequently

$$
\boxed{\int_S\boldsymbol r\cdot d\boldsymbol S=3\operatorname{Vol}(V)=4\pi a^2b.}
$$

<h3 id="18/b">b</h3>

↑ **Parent:** [18](#18)

<h4 id="18/b/solution">Solution</h4>

↑ **Parent:** [B](#18/b)

Since $\boldsymbol a$ is constant, componentwise differentiation gives $\nabla\cdot(\boldsymbol a\phi)=\sum_ia_i\partial_i\phi=\boldsymbol a\cdot\nabla\phi$. Applying the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) to this [vector field](../../multivariable-calculus.md#vector-field) gives

$$
\boldsymbol a\cdot\int_S\phi\,d\boldsymbol S=\boldsymbol a\cdot\int_V\nabla\phi\,dV.
$$

This holds for every constant [vector](../../vector-space.md#vector) $\boldsymbol a$, so the vector integrals agree. This is the [vector gradient form of the divergence theorem](../../multivariable-calculus.md#vector-gradient-form-of-the-divergence-theorem). With $\phi=z$, the [gradient](../../multivariable-calculus.md#gradient) is the constant unit vector $\boldsymbol e_z$. Therefore

$$
\boxed{\int_S z\,d\boldsymbol S=\frac{4\pi a^2b}3\,\boldsymbol e_z.}
$$

<h3 id="18/c">c</h3>

↑ **Parent:** [18](#18)

<h4 id="18/c/solution">Solution</h4>

↑ **Parent:** [C](#18/c)

The identity $\nabla\cdot(\boldsymbol a\times\boldsymbol v)=\boldsymbol v\cdot(\nabla\times\boldsymbol a)-\boldsymbol a\cdot(\nabla\times\boldsymbol v)$ reduces to $-\boldsymbol a\cdot(\nabla\times\boldsymbol v)$ when $\boldsymbol a$ is constant. In components, this follows by differentiating $\varepsilon_{ijk}a_jv_k$ and using the antisymmetry of the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol). The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) and the cyclic [scalar triple product](../../multilinear-algebra.md#scalar-triple-product) identity now give

$$
\boldsymbol a\cdot\int_S\boldsymbol v\times d\boldsymbol S
=\int_S(\boldsymbol a\times\boldsymbol v)\cdot d\boldsymbol S
=-\boldsymbol a\cdot\int_V\nabla\times\boldsymbol v\,dV.
$$

Since $\boldsymbol a$ is arbitrary,

$$
\boxed{\int_S\boldsymbol v\times d\boldsymbol S=-\int_V\nabla\times\boldsymbol v\,dV.}
$$

The order of the [cross product](../../vector-space.md#cross-product) determines the minus sign, as in the [vector curl form of the divergence theorem](../../multivariable-calculus.md#vector-curl-form-of-the-divergence-theorem).

## 19

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="19/a">a</h3>

↑ **Parent:** [19](#19)

<h4 id="19/a/solution">Solution</h4>

↑ **Parent:** [A](#19/a)

For $c>0$ and $l>0$, the zero-endpoint [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) select the [Fourier sine basis](../../fourier-series.md#fourier-sine-basis) functions $\sin(n\pi x/l)$. [Separation of variables](../../partial-differential-equation.md#separation-of-variables) gives temporal factors with angular [frequencies](../../wave.md#frequency) $\omega_n=n\pi c/l$. Zero initial displacement removes the temporal cosine terms, giving

$$
y(x,t)=\sum_{n=1}^{\infty}a_n\sin(n\pi x/l)\sin(n\pi ct/l).
$$

Differentiating at $t=0$ and using [Fourier orthogonality](../../fourier-series.md#fourier-orthogonality) gives

$$
\boxed{a_n=\frac2{n\pi c}\int_0^lv(x)\sin(n\pi x/l)\,dx.}
$$

The evaluation property of the given initial velocity means $v(x)=\delta(x-l/2)$ in the sense of a [Dirac delta](../../distribution-theory.md#dirac-delta-function), an idealized [impulsively struck fixed-end string](../../wave-equation.md#impulsively-struck-fixed-end-string). Thus $a_n=2\sin(n\pi/2)/(n\pi c)$: every even mode vanishes, while the lowest two excited modes have $n=1,3$. Their ordinary [frequencies](../../wave.md#frequency) and amplitude ratio are

$$
\boxed{f_1=\frac c{2l},\quad f_3=\frac{3c}{2l},\qquad |a_1|:|a_3|=3:1.}
$$

The signed coefficient ratio is $a_3/a_1=-1/3$. The impulse solution is interpreted as a [distributional weak solution](../../partial-differential-equation.md#weak-solution), rather than one with a smooth initial velocity.

<a id="19/a/image-the-two-lowest-string-modes-excited-by-a-midpoint-velocity-impulse-with-their-signed-relative-amplitudes"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2-midpoint-impulse-modes.png)

**[Figure 2](#19/a/image-the-two-lowest-string-modes-excited-by-a-midpoint-velocity-impulse-with-their-signed-relative-amplitudes). The two lowest string modes excited by a midpoint velocity impulse, with their signed relative amplitudes**.

<h3 id="19/b">b</h3>

↑ **Parent:** [19](#19)

<h4 id="19/b/solution">Solution</h4>

↑ **Parent:** [B](#19/b)

For a separated [harmonic function](../../partial-differential-equation.md#harmonic-function) $V=F(x)G(y)$, [Laplace's equation](../../partial-differential-equation.md#laplace-equation) gives $F''/F=-G''/G=-k^2$. Bounded periodic dependence in $x$ has $F=A\cos(kx)+B\sin(kx)$; decay on each half-plane selects $G=e^{-k|y|}$ for $k>0$, when the potential is matched continuously at the sheet. These are the separated decaying modes. General decaying solutions can be superpositions of them; decay alone does not force a single value of $k$.

The prescribed cosine density selects $k=1$ and $V=C\cos x\,e^{-|y|}$. Its normal [derivative](../../calculus.md#derivative) jump is $-2C\cos x$. Matching the stated jump $2\pi\Sigma_0\cos x$ gives

$$
\boxed{V(x,y)=-\pi\Sigma_0\cos x\,e^{-|y|}.}
$$

This is the [gravitational potential of a sinusoidal sheet](../../newton-s-law-of-universal-gravitation.md#gravitational-potential-of-a-sinusoidal-sheet) in the normalization of the question. It is continuous at the sheet and decays on both sides. Since $\Sigma_0\cos x$ changes sign, it can physically describe a Fourier component of a density perturbation rather than an everywhere positive isolated mass sheet.

## ↑ Ancestors (10)

1. [2008](../2008.md)
2. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
