# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2008/PaperIA_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2008/PaperIA_2.pdf)

**Table of contents**

- [1A](#1a)
  - [Solution](#1a/solution)
- [2A](#2a)
  - [Solution](#2a/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5A](#5a)
  - [Solution](#5a/solution)
  - [i](#5a/i)
    - [Solution](#5a/i/solution)
  - [ii](#5a/ii)
    - [Solution](#5a/ii/solution)
  - [iii](#5a/iii)
    - [Solution](#5a/iii/solution)
  - [iv](#5a/iv)
    - [Solution](#5a/iv/solution)
  - [v](#5a/v)
    - [Solution](#5a/v/solution)
- [6A](#6a)
  - [Solution](#6a/solution)
- [7A](#7a)
  - [Solution](#7a/solution)
- [8A](#8a)
  - [Solution](#8a/solution)
- [9F](#9f)
  - [Solution](#9f/solution)
- [10F](#10f)
  - [i](#10f/i)
    - [Solution](#10f/i/solution)
  - [ii](#10f/ii)
    - [Solution](#10f/ii/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12F](#12f)
  - [Solution](#12f/solution)

## 1A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1a/solution">Solution</h3>

↑ **Parent:** [1A](#1a)

The [complementary solution](../../../differential-equation.md#homogeneous-solution) comes from the characteristic equation $r^4-a^4=0$, whose roots are $a,-a,ia,-ia$. It is therefore

$$
y_h=C_1e^{ax}+C_2e^{-ax}+C_3\cos(ax)+C_4\sin(ax).
$$

For the [resonant exponential particular solution](../../../differential-equation.md#resonant-exponential-particular-solution), the forcing is already a homogeneous exponential, so the [method of undetermined coefficients](../../../differential-equation.md#method-of-undetermined-coefficients) needs the resonant trial $y_p=Kxe^{-ax}$. If $P(r)=r^4-a^4$, the identity $P(D)[xe^{rx}]=P'(r)e^{rx}$ when $P(r)=0$ gives $P'(-a)=-4a^3$. Hence $K=-1/(4a^3)$ and

$$
y=C_1e^{ax}+C_2e^{-ax}+C_3\cos(ax)+C_4\sin(ax)-\frac{x}{4a^3}e^{-ax}.
$$

The decay condition first eliminates the growing exponential, $C_1=0$. A nonzero combination of the sine and cosine has a fixed nonzero amplitude and cannot tend to zero, so $C_3=C_4=0$ as well. Both remaining exponential terms decay because $a>0$. Finally $y(0)=C_2=1$, giving the unique answer

$$
\boxed{y(x)=\left(1-\frac{x}{4a^3}\right)e^{-ax}.}
$$

This is an instance of [resonance in a differential equation](../../../differential-equation.md#resonance-in-a-differential-equation): multiplication by $x$ supplies the [particular solution](../../../differential-equation.md#particular-solution) when the forcing exponent is a simple characteristic root.

## 2A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2a/solution">Solution</h3>

↑ **Parent:** [2A](#2a)

For the [cubic population iteration](../../../dynamical-systems.md#cubic-population-iteration), put $g(u)=\lambda u(1-u^2)$. Its [fixed points](../../../function.md#fixed-point) solve

$$
u=g(u)\quad\Longleftrightarrow\quad u[(\lambda-1)-\lambda u^2]=0.
$$

Thus $u_*=0$ always exists. For $\lambda\ne0$ there are also

$$
\boxed{u_*=\pm\sqrt{1-\frac1\lambda}}
$$

whenever the expression under the square root is positive, namely $\lambda<0$ or $\lambda>1$. At $\lambda=1$ these coincide with zero; at $\lambda=0$ only zero exists.

The criterion for [fixed point stability for an iteration](../../../dynamical-systems.md#fixed-point-stability-for-an-iteration) is $|g'(u_*)|<1$. To justify it, [continuity](../../../calculus.md#continuous-function) of $g'$ gives a small interval around the [fixed point](../../../function.md#fixed-point) where $|g'|\leq q<1$. The [mean value theorem](../../../calculus.md#mean-value-theorem) then gives $|g(u)-u_*|\leq q|u-u_*|$, so this interval is invariant and the error decreases geometrically. This proves local [asymptotic stability](../../../dynamical-systems.md#asymptotic-stability) rather than merely linear boundedness.

Here $g'(u)=\lambda(1-3u^2)$. At zero its value is $\lambda$, so **zero is locally [asymptotically stable](../../../dynamical-systems.md#asymptotic-stability) for $-1<\lambda<1$**. At a nonzero [fixed point](../../../function.md#fixed-point) it is

$$
g'(u_*)=\lambda\left[1-3\left(1-\frac1\lambda\right)\right]=3-2\lambda.
$$

The strict inequality $|3-2\lambda|<1$ is equivalent to $1<\lambda<2$. Both nonzero real [fixed points](../../../function.md#fixed-point) are therefore locally [asymptotically stable](../../../dynamical-systems.md#asymptotic-stability) on that interval. This proves the two requested existence ranges. The strict [derivative](../../../calculus.md#derivative) criterion alone makes no conclusion at the endpoint multipliers of modulus one.

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

The [sampling without replacement](../../../statistical-inference.md#sampling-without-replacement) makes all $\binom n2$ unordered pairs equally likely. The count of red-red pairs is $\binom32=3$, while the count of mixed pairs is $3(n-3)$. Thus their [probabilities](../../../probability-theory.md#probability) satisfy

$$
\frac{3(n-3)}{\binom n2}=3\frac3{\binom n2},
$$

and cancellation gives $n-3=3$. Hence $\boxed{n=6}$, with three black socks. The count of black-black pairs is also $\binom32=3$, so

$$
\boxed{\mathbb P(\text{two black socks})=\frac{\binom32}{\binom62}=\frac15.}
$$

The mixed, red-red and black-black [probabilities](../../../probability-theory.md#probability) are respectively $3/5,1/5,1/5$, which add to one and verify the given ratio.

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

Let $X$ be one score. It has the [discrete uniform distribution](../../../discrete-probability-distribution.md#discrete-uniform-distribution) on $1,\ldots,6$, so its [expected value](../../../probability-theory.md#expected-value) and [second moment](../../../probability-theory.md#second-moment) are

$$
\mathbb EX=\frac{1+2+3+4+5+6}{6}=\frac72,\qquad
\mathbb EX^2=\frac{1^2+2^2+3^2+4^2+5^2+6^2}{6}=\frac{91}{6}.
$$

Therefore

$$
\boxed{\mathbb EX=\frac72,\qquad\operatorname{Var}(X)=\frac{91}{6}-\frac{49}{4}=\frac{35}{12}.}
$$

For [independent](../../../random-variable.md#independent-random-variables) throws, [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) and additivity of [variance](../../../variance.md) give $\mathbb EY_n=7n/2$ and $\operatorname{Var}(Y_n)=35n/12$. The sample average consequently has [expectation](../../../probability-theory.md#expected-value) $7/2$ and [variance](../../../variance.md) $35/(12n)$.

The [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) follows by applying the [Markov inequality](../../../probability-inequality.md#markov-inequality) to the nonnegative square of a centered [random variable](../../../random-variable.md). It gives

$$
\mathbb P\left(\left|\frac{Y_n}{n}-\frac72\right|>\frac32\right)
\leq\frac{35/(12n)}{(3/2)^2}=\frac{35}{27n}.
$$

This is at most $1/10$ if $n\geq350/27$. Thus **$n=13$ suffices**, as does every larger integer. This is the smallest integer guaranteed by this particular [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) bound; it need not be the smallest integer satisfying the actual [probability](../../../probability-theory.md#probability) requirement.

## 5A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5a/solution">Solution</h3>

↑ **Parent:** [5A](#5a)

Measure temperature relative to ambient by $\theta_i=T_i-T_\infty$. [Newton's law of cooling](../../../differential-equation.md#newton-s-law-of-cooling) models ordinary cooling by $\theta_i'=-a\theta_i$, since heat loss is proportional to the excess temperature. The additional negative forcing represents the cooling from the milk, with the temperature drop or rate normalized to one in the chosen units.

The [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) has unit integral and is supported at the instant of addition. It therefore imposes a sudden unit drop for cup 1. The difference $H(t-1)-H(t-2)$ of [Heaviside step functions](../../../analysis.md#heaviside-step-function) is one during the addition interval and zero outside it, giving a unit cooling rate for cup 2. The second temperature is continuous; only its [derivative](../../../calculus.md#derivative) changes at the switching times. The value assigned to a [Heaviside step function](../../../analysis.md#heaviside-step-function) exactly at its jump does not change the integrated solution. This is the [impulse versus finite-duration cooling](../../../differential-equation.md#impulse-versus-finite-duration-cooling) comparison.

<h3 id="5a/i">i</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/i/solution">Solution</h4>

↑ **Parent:** [I](#5a/i)

Before time one, both forcing terms vanish. The [separable differential equation](../../../differential-equation.md#separable-differential-equation) $\theta_i'=-a\theta_i$ gives $\theta_i(t)=C_i e^{-at}$. The initial values give $C_1=C_2=T_0-T_\infty$, and hence

$$
\boxed{T_1(t)=T_2(t)=T_\infty+(T_0-T_\infty)e^{-at},\qquad0\leq t<1.}
$$

In particular the common left-hand limit at time one is $T_\infty+(T_0-T_\infty)e^{-a}$.

<h3 id="5a/ii">ii</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5a/ii)

Integrate the first equation over $(1-\varepsilon,1+\varepsilon)$. The integral of the ordinary cooling term tends to zero as $\varepsilon\downarrow0$, while the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) integrates to one. Thus the [jump condition for an impulse](../../../differential-equation.md#jump-condition-for-an-impulse) is

$$
\boxed{T_1(1^+)-T_1(1^-)=-1.}
$$

After the jump there is no further forcing, so [Newton's law of cooling](../../../differential-equation.md#newton-s-law-of-cooling) gives

$$
T_1(t)-T_\infty=[(T_0-T_\infty)e^{-a}-1]e^{-a(t-1)}.
$$

Equivalently,

$$
\boxed{T_1(t)=T_\infty+(T_0-T_\infty)e^{-at}-e^{-a(t-1)},\qquad t>1.}
$$

The last term has jump minus one at time one and then decays at the same exponential rate as the unforced temperature.

<h3 id="5a/iii">iii</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5a/iii)

On the active interval the excess temperature satisfies $\theta_2'+a\theta_2=-1$. Multiplication by the [integrating factor](../../../differential-equation.md#integrating-factor) $e^{at}$ and integration from time one gives

$$
e^{at}\theta_2(t)-e^a\theta_2(1)=-\int_1^t e^{as}\,ds
=-\frac{e^{at}-e^a}{a}.
$$

There is no impulse in this equation, so [continuity](../../../calculus.md#continuous-function) supplies $\theta_2(1)=(T_0-T_\infty)e^{-a}$. Therefore

$$
\boxed{T_2(t)=T_\infty-\frac1a+
 e^{-at}\left(T_0-T_\infty+\frac{e^a}{a}\right),\qquad1<t<2.}
$$

The equivalent correction to the common unforced temperature is $-(1-e^{-a(t-1)})/a$, which vanishes continuously at the beginning of the interval.

<h3 id="5a/iv">iv</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5a/iv)

At time two, [continuity](../../../calculus.md#continuous-function) of the second temperature gives

$$
\theta_2(2)=(T_0-T_\infty)e^{-2a}-\frac{1-e^{-a}}a.
$$

The forcing then turns off, so [Newton's law of cooling](../../../differential-equation.md#newton-s-law-of-cooling) again gives exponential decay:

$$
\boxed{T_2(t)=T_\infty+(T_0-T_\infty)e^{-at}
-\frac{1-e^{-a}}a e^{-a(t-2)},\qquad t>2.}
$$

Subtracting this from the first temperature and expressing both corrections with the same exponential factor gives

$$
\boxed{T_1(t)-T_2(t)=\left(\frac{e^a-1}{a}-1\right)e^{-a(t-1)},\qquad t>2.}
$$

Because $e^a>1+a$ for $a>0$, this difference is positive. Thus the cup cooled instantaneously is warmer after the addition interval: its cooling occurred earlier and has undergone more subsequent exponential attenuation.

<h3 id="5a/v">v</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/v/solution">Solution</h4>

↑ **Parent:** [V](#5a/v)

During the addition interval, subtracting the formulas in (ii) and (iii) cancels the common unforced temperature:

$$
T_1(t)-T_2(t)=\frac1a-\left(1+\frac1a\right)e^{-a(t-1)}.
$$

This is zero precisely when $e^{-a(t-1)}=1/(1+a)$, so

$$
\boxed{t^*=1+\frac{\log(1+a)}a.}
$$

The inequalities $0<\log(1+a)<a$ give $1<t^*<2$, so using the active-interval formula was justified. The difference has [derivative](../../../calculus.md#derivative) $(1+a)e^{-a(t-1)}>0$, making this crossing unique within that interval. Immediately after time one it is minus one; after time two it is strictly positive by (iv). Hence there is no other equality at any finite time after time one. Both temperatures approach the same ambient limit, but that limiting equality is not an additional crossing.

## 6A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6a/solution">Solution</h3>

↑ **Parent:** [6A](#6a)

With the indicated order of the two solutions, define the [Wronskian](../../../differential-equation.md#wronskian) by

$$
\boxed{W=y_1y_2'-y_1'y_2
=\det\begin{pmatrix}y_1&y_2\\y_1'&y_2'\end{pmatrix}.}
$$

Where $y_1\ne0$, this gives the first-order [linear differential equation](../../../differential-equation.md#linear-differential-equation)

$$
y_2'-\frac{y_1'}{y_1}y_2=\frac{W}{y_1},\qquad
\left(\frac{y_2}{y_1}\right)'=\frac{W}{y_1^2}.
$$

Integrating produces the [reduction of order](../../../differential-equation.md#reduction-of-order) formula

$$
\boxed{y_2(x)=y_1(x)\left[C_2+\int_{x_0}^x\frac{W(s)}{y_1(s)^2}\,ds\right].}
$$

This formula is local on an interval where the known solution does not vanish; an arbitrary nonzero scaling of the [linearly independent](../../../vector-space.md#linear-independence) solution changes the normalization of $W$.

Differentiate the [Wronskian](../../../differential-equation.md#wronskian) and use the differential equation for each solution:

$$
W'=y_1y_2''-y_1''y_2
=y_1(-py_2'-qy_2)-(-py_1'-qy_1)y_2=-pW.
$$

Thus $\boxed{W'+pW=0}$, proving the [Abel identity](../../../differential-equation.md#abel-s-identity), and $W=C\exp(-\int p\,dx)$. For continuous coefficients on a nonsingular interval, [linearly independent](../../../vector-space.md#linear-independence) solutions have $C\ne0$.

For the particular equation, write $s=x-1$. The proposed solution is $y_1=s^2$, with $y_1'=2s$ and $y_1''=2$, so substitution gives $2s^2+2s^2-4s^2=0$. Away from the singular point $x=1$, division by $s^2$ gives $p=1/s$. The [Abel identity](../../../differential-equation.md#abel-s-identity) therefore gives

$$
W=\frac Cs
$$

with a separate constant on each interval lying on one side of the singular point. The [reduction of order](../../../differential-equation.md#reduction-of-order) integral is $\int W/y_1^2\,dx=C\int s^{-5}\,ds=-C/(4s^4)$, so

$$
y_2=C_2s^2-\frac C4s^{-2}.
$$

Choosing $C_2=0$, $C=-4$ gives

$$
\boxed{y_2(x)=(x-1)^{-2},\qquad W(x)=-\frac4{x-1}.}
$$

The nonzero [Wronskian](../../../differential-equation.md#wronskian) proves [linear independence](../../../vector-space.md#linear-independence). Direct substitution also verifies the second solution, since $s^2(6s^{-4})+s(-2s^{-3})-4s^{-2}=0$. These solutions form a [basis](../../../vector-space.md#basis) on either nonsingular interval; the second solution is not defined at $x=1$.

## 7A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7a/solution">Solution</h3>

↑ **Parent:** [7A](#7a)

Write a [power series](../../../real-analysis.md#power-series) $y=\sum_{n\geq0}c_nx^n$. Substitution gives

$$
\sum_{n\geq0}n(n-2)c_nx^{n-1}+4\sum_{n\geq0}c_nx^{n+3}=0.
$$

The lowest coefficients give $c_1=0$, $c_3=0$, with $c_0,c_2$ free. For $n\geq4$, matching the coefficient of $x^{n-1}$ gives the recurrence

$$
\boxed{c_n=-\frac{4c_{n-4}}{n(n-2)}.}
$$

All odd coefficients consequently vanish. For the first solution, $c_0=a$, $c_2=y_1''(0)/2=0$, so the first three nonzero terms, when $a\ne0$, are

$$
\boxed{y_1(x)=a-\frac a2x^4+\frac a{24}x^8+O(x^{12}).}
$$

For the second, $c_0=0$, $c_2=b/2$, giving

$$
\boxed{y_2(x)=\frac b2x^2-\frac b{12}x^6+\frac b{240}x^{10}+O(x^{14}).}
$$

If its prescribed constant is zero, the corresponding solution is identically zero and has no nonzero terms.

For the change of variable, put $y(x)=Y(u)$, $u=x^\alpha$, with $\alpha\ne0$. The [chain rule](../../../calculus.md#chain-rule) gives

$$
xy''-y'+4x^3y
=\alpha^2x^{2\alpha-1}Y_{uu}
+\alpha(\alpha-2)x^{\alpha-1}Y_u+4x^3Y.
$$

After division by $x^{2\alpha-1}$, the coefficient of $Y_u$ is $\alpha(\alpha-2)x^{-\alpha}$ and that of $Y$ is $4x^{4-2\alpha}$. A genuine constant-coefficient equation requires $\alpha=2$, which both removes $Y_u$ and makes the final coefficient constant. The transformed equation is $4Y_{uu}+4Y=0$.

This [quadratic-variable reduction of a singular oscillator](../../../differential-equation.md#quadratic-variable-reduction-of-a-singular-oscillator) yields

$$
\boxed{\alpha=2,\qquad y(x)=A\cos(x^2)+B\sin(x^2).}
$$

It holds on each interval away from zero and both solutions extend smoothly through zero. Here $y(0)=A$ and $y''(0)=2B$, so the specified solutions are exactly $a\cos(x^2)$ and $(b/2)\sin(x^2)$. Their [Taylor series](../../../calculus.md#taylor-series) agree with the recurrences above. Although the original equation has a [regular singular point](../../../complex-analysis.md#regular-singular-point) at zero, these two [linearly independent](../../../vector-space.md#linear-independence) smooth solutions supply the required data there.

## 8A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8a/solution">Solution</h3>

↑ **Parent:** [8A](#8a)

For this [quartic potential with fourfold symmetry](../../../analysis.md#quartic-potential-with-fourfold-symmetry), the first [derivatives](../../../calculus.md#derivative) factor:

$$
f_x=2x(1-x^2-by^2),\qquad f_y=2y(1-y^2-bx^2).
$$

The [critical points](../../../analysis.md#critical-point) are the origin, the four axis points $(\pm1,0),(0,\pm1)$, and four points with both coordinates nonzero. At the latter, $x^2+by^2=y^2+bx^2=1$. Subtracting and using $b\ne1$ gives $x^2=y^2=1/(1+b)$. Thus the complete list is

$$
\boxed{(0,0),\quad(\pm1,0),(0,\pm1),\quad
\left(\pm\frac1{\sqrt{1+b}},\pm\frac1{\sqrt{1+b}}\right),}
$$

where the two signs in the final group are chosen separately.

The [Hessian](../../../calculus.md#hessian-matrix) is

$$
D^2f=\begin{pmatrix}2-6x^2-2by^2&-4bxy\\-4bxy&2-6y^2-2bx^2\end{pmatrix}.
$$

At the origin it is $2I$, so there is a strict [local minimum](../../../analysis.md#local-minimum) with value zero. At an axis point its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $-4$ and $2(1-b)$, giving a [saddle point of a scalar function](../../../analysis.md#saddle-point-of-a-scalar-function) if $b<1$ and a strict [local maximum](../../../analysis.md#local-maximum) if $b>1$. All four axis values are $1/2$.

At a diagonal point the [Hessian](../../../calculus.md#hessian-matrix) has [eigenvalues](../../../linear-operator-theory.md#eigenvalue)

$$
-4,\qquad-\frac{4(1-b)}{1+b}.
$$

Hence these four points are strict [local maxima](../../../analysis.md#local-maximum) for $b<1$ and [saddle points of a scalar function](../../../analysis.md#saddle-point-of-a-scalar-function) for $b>1$. Their value is $1/(1+b)$. None of these [critical points](../../../analysis.md#critical-point) is degenerate when $b\ne1$.

To describe the [level curves](../../../topology.md#level-curve) precisely, use [polar coordinates](../../../calculus.md#polar-coordinates) and write

$$
f=r^2-\frac12q(\theta)r^4,\qquad
q(\theta)=1+\frac{b-1}{2}\sin^2(2\theta)>0.
$$

For a level $f=c$, the possible radii satisfy

$$
\boxed{r^2=\frac{1\pm\sqrt{1-2q(\theta)c}}{q(\theta)},}
$$

retaining only real, nonnegative values. This formula, together with reflection in each axis and interchange of the coordinates, determines the [level curves](../../../topology.md#level-curve). The radial maximum in a direction is $1/(2q)$, attained at $r^2=1/q$. It also proves that the [local maxima](../../../analysis.md#local-maximum) identified above are global: the largest directional value is $1/(1+b)$ on the diagonals if $b<1$, and $1/2$ on the axes if $b>1$.

For negative $c$ only the plus sign gives a positive radius, producing one outer closed [level curve](../../../topology.md#level-curve). At $c=0$ there is the isolated origin and the outer curve $r^2=2/q$. For $0<c<c_s$, where $c_s$ is the saddle value, both radial branches exist in every direction, giving an inner loop around the origin and an outer loop. At $c=c_s$ they meet at the four [saddle points of a scalar function](../../../analysis.md#saddle-point-of-a-scalar-function). Above the saddle value, four separate loops surround the four maxima; they shrink to those points at the maximum value. There are no [level curves](../../../topology.md#level-curve) above it.

For **$0<b<1$**, the saddle value is $c_s=1/2$ and the four high-level loops lie along the diagonals. For **$b>1$**, $c_s=1/(1+b)$ and the four high-level loops lie along the coordinate axes. The sketches show representative values in both regimes; the highlighted [level curve](../../../topology.md#level-curve) is the saddle level.

<a id="8a/image-contours-of-the-fourfold-quartic-potential-with-diagonal-maxima-for-b-less-than-one-and-axis-maxima-for-b-greater-than-one"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2-contours.png)

**[Figure 1](#8a/image-contours-of-the-fourfold-quartic-potential-with-diagonal-maxima-for-b-less-than-one-and-axis-maxima-for-b-greater-than-one). Contours of the fourfold quartic potential, with diagonal maxima for b less than one and axis maxima for b greater than one**.

Finally, at $b=1$ the expression depends only on radius:

$$
f=r^2-\frac12r^4=\frac12-\frac12(r^2-1)^2.
$$

Consequently $\boxed{\max f=1/2\text{, attained exactly on }x^2+y^2=1.}$ The maximum set is the whole unit circle, not merely four isolated points.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/solution">Solution</h3>

↑ **Parent:** [9F](#9f)

Let $G(s)=\mathbb E[s^\xi]$ be the offspring [probability generating function](../../../probability-theory.md#probability-generating-function), and let $G_n(s)=\mathbb E[s^{Z_n}]$, for $0\leq s\leq1$. Given $Z_n=k$, the next generation is a sum of $k$ [independent](../../../random-variable.md#independent-random-variables) offspring counts. Multiplication of their [probability generating functions](../../../probability-theory.md#probability-generating-function) gives

$$
\mathbb E[s^{Z_{n+1}}\mid Z_n=k]=G(s)^k.
$$

Taking [conditional expectation](../../../measure-theory.md#conditional-expectation) and then averaging proves

$$
\boxed{G_{n+1}(s)=G_n(G(s)),\qquad G_0(s)=s.}
$$

Thus $G_n$ is the $n$-fold composition of $G$ with itself. Induction makes this precise: it is true for $n=0$, and composing once more gives the next generation. In particular $G_n\circ G=G\circ G_n$, since both are the same iterated function. This is the generating-function recursion for a [Galton-Watson process](../../../probability-and-statistics.md#galton-watson-process).

Write $m=\mathbb E Z_1=G'(1^-)$, initially assuming it is finite. The [law of total expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\mathbb E[Z_{n+1}\mid Z_n]=mZ_n,
\qquad \mathbb E Z_{n+1}=m\mathbb E Z_n.
$$

Starting at one therefore yields $\boxed{\mathbb E Z_n=m^n}$, with the value at $n=0$ understood to be one even if $m=0$. Equivalently, differentiating the composition at one gives the same recurrence. If the offspring [expectation](../../../probability-theory.md#expected-value) is infinite, every positive generation has infinite [expectation](../../../probability-theory.md#expected-value): a positive chance of at least one parent remains at each finite generation, and conditional on any positive parent count the next expected count is infinite.

For a [Poisson branching process](../../../probability-and-statistics.md#poisson-branching-process), $G(s)=e^{\lambda(s-1)}$. Extinction is absorbing because an empty generation has no parents, so extinction by generation $n$ is precisely $Z_n=0$. Hence $x_n=G_n(0)$. Using the composition in the order $G\circ G_n$ gives

$$
\boxed{x_{n+1}=e^{\lambda(x_n-1)},\qquad x_0=0.}
$$

For example $x_1=e^{-\lambda}$ is the chance of no offspring in the first generation. The recurrence includes the degenerate case $\lambda=0$, where extinction occurs in the first generation with certainty.

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/i">i</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/i/solution">Solution</h4>

↑ **Parent:** [I](#10f/i)

Put $q=1-p$ and track the difference $S_n$ between the numbers of wins. It is a [biased random walk](../../../markov-process.md#biased-random-walk) with increments $+1$ and $-1$, stopped on first reaching $3$ or $-3$.

To finish at $+3$ on game five, there must be four wins for $A$ and one for $B$, with the final game won by $A$. The unique loss for $A$ can be in position one, two or three. If it were in position four or five, the first three games would already have stopped the contest. Each of the three allowed paths remains strictly inside the barriers until the last step and has [probability](../../../probability-theory.md#probability) $p^4q$. By interchanging players, there are also three paths ending at $-3$, each with [probability](../../../probability-theory.md#probability) $pq^4$. Therefore

$$
\boxed{\mathbb P(N=5)=3p^4q+3pq^4=3pq(p^3+q^3).}
$$

For a fair game this is $3/16$. Counting all five-game sequences with final win difference three would overcount paths on which the contest ended earlier.

<h3 id="10f/ii">ii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10f/ii)

This is a [gambler's ruin](../../../markov-process.md#gambler-s-ruin) hitting problem. For $0<p<1$, let $h_j$ be the [probability](../../../probability-theory.md#probability) of reaching $+3$ before $-3$ when the current difference is $j$. Conditioning on the next [independent](../../../random-variable.md#independent-random-variables) game gives

$$
h_j=ph_{j+1}+qh_{j-1}\quad(-2\leq j\leq2),\qquad h_{-3}=0,\quad h_3=1.
$$

Stopping occurs almost surely: conditional on being inside the barriers, three consecutive wins by either player force absorption within the next three games. This event has [probability](../../../probability-theory.md#probability) $p^3+q^3>0$, so the chance of surviving $m$ such blocks is at most $(1-p^3-q^3)^m$, which tends to zero.

If $p\ne q$, the characteristic roots of the interior recurrence are $1$ and $r=q/p$, so $h_j=A+Br^j$. Imposing the two boundary values yields

$$
h_j=\frac{1-r^{j+3}}{1-r^6}.
$$

In particular,

$$
h_0=\frac{1-r^3}{1-r^6}=\frac1{1+r^3}
=\frac{p^3}{p^3+q^3}.
$$

For $p=q=1/2$ the recurrence instead has affine solutions, and the boundary values give $h_j=(j+3)/6$, hence $h_0=1/2$. The deterministic cases $p=0,1$ give zero and one respectively. The formula covers all of them continuously:

$$
\boxed{\mathbb P(A\text{ wins overall})=\frac{p^3}{p^3+(1-p)^3},\qquad0\leq p\leq1.}
$$

The stopping argument and the boundary recurrence show why the answer concerns the first barrier reached rather than the win difference after a predetermined number of games.

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

Write $s=\sqrt{1-\rho^2}>0$. The inverse change of variables is $y=\rho x+sz$, whose [Jacobian determinant](../../../calculus.md#jacobian-determinant) has absolute value $s$. Completing the square gives

$$
\frac{x^2-2\rho xy+y^2}{1-\rho^2}=x^2+z^2.
$$

The [change of variables formula](../../../calculus.md#change-of-variables-formula) therefore transforms the joint [probability density function](../../../continuous-probability-distribution.md#probability-density-function) to

$$
g(x,z)=s f(x,\rho x+sz)
=\frac1{2\pi}e^{-(x^2+z^2)/2}
=\left(\frac{e^{-x^2/2}}{\sqrt{2\pi}}\right)
 \left(\frac{e^{-z^2/2}}{\sqrt{2\pi}}\right).
$$

It factors into two normalized [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) densities. Thus **$X$ and $Z$ are [independent](../../../random-variable.md#independent-random-variables) $N(0,1)$ variables**; factorization proves the requested [independence](../../../random-variable.md#independent-random-variables), rather than simply zero [covariance](../../../variance.md#covariance).

The [standard Gaussian random vector](../../../probability-and-statistics.md#standard-gaussian-random-vector) $(X,Z)$ has a rotation-invariant density. In [polar coordinates](../../../calculus.md#polar-coordinates), $X=r\cos\theta$, $Z=r\sin\theta$, its density with the area factor is $(2\pi)^{-1}re^{-r^2/2}$, so the angular coordinate is uniform on an interval of length $2\pi$.

Put $\alpha=\arcsin\rho\in(-\pi/2,\pi/2)$, so $s=\cos\alpha$ and

$$
Y=\rho X+sZ=r\sin(\theta+\alpha).
$$

In the right half-plane, choose $-\pi/2<\theta<\pi/2$. The additional condition $Y>0$ then requires $-\alpha<\theta<\pi/2$. This wedge has angle $\pi/2+\alpha$; its boundary has [probability](../../../probability-theory.md#probability) zero. Consequently

$$
\boxed{\mathbb P(X>0,Y>0)=\frac14+\frac{\arcsin\rho}{2\pi}.}
$$

At $\rho=0$ this is $1/4$, as required by [independence](../../../random-variable.md#independent-random-variables). The limits as $\rho\to1$ and $\rho\to-1$ are $1/2$ and zero, respectively. The angular calculation is also the geometric [basis](../../../vector-space.md#basis) of the [Gaussian sign-correlation identity](../../../probability-and-statistics.md#gaussian-sign-correlation-identity).

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/solution">Solution</h3>

↑ **Parent:** [12F](#12f)

Use the positive-support convention for the [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) and put $q=1-p$. Differentiating the convergent [geometric series](../../../real-analysis.md#geometric-series) $\sum_{k\geq0}q^k=(1-q)^{-1}$ gives

$$
\sum_{k\geq1}kq^{k-1}=\frac1{(1-q)^2},\qquad
\sum_{k\geq2}k(k-1)q^{k-2}=\frac2{(1-q)^3}.
$$

Consequently

$$
\mathbb EY=p\sum_{k\geq1}kq^{k-1}=\frac1p,\qquad
\mathbb E[Y(Y-1)]=pq\sum_{k\geq2}k(k-1)q^{k-2}=\frac{2q}{p^2}.
$$

Subtracting the square of the [expectation](../../../probability-theory.md#expected-value) from the [second moment](../../../probability-theory.md#second-moment) yields

$$
\boxed{\mathbb EY=\frac1p,\qquad\operatorname{Var}(Y)=\frac{1-p}{p^2}.}
$$

For the die, this is the [coupon collector problem](../../../discrete-probability-distribution.md#coupon-collector-problem). When $r$ scores are still missing, let $W_r$ count rolls up to and including the next newly observed score. Every fresh roll has success [probability](../../../probability-theory.md#probability) $r/6$, so $W_r$ has a [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) of parameter $r/6$. These six successive waiting times are [independent](../../../random-variable.md#independent-random-variables): conditional on the entire past at the start of a stage, its waiting-time distribution depends only on the number $r$, not on the identities of the missing scores. Iterated conditioning therefore factors their joint distribution. The total number of rolls is $N=\sum_{r=1}^6W_r$.

Using [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) gives

$$
\boxed{\mathbb EN=\sum_{r=1}^6\frac6r
=6\left(1+\frac12+\frac13+\frac14+\frac15+\frac16\right)
=\frac{147}{10}=14.7.}
$$

Using [variance additivity for independent random variables](../../../variance.md#variance-additivity-for-independent-random-variables), or the [coupon collector waiting-time variance](../../../discrete-probability-distribution.md#coupon-collector-waiting-time-variance) formula just derived by this decomposition, gives

$$
\operatorname{Var}(N)=\sum_{r=1}^6\frac{1-r/6}{(r/6)^2}
=\sum_{r=1}^6\left[\left(\frac6r\right)^2-\frac6r\right]
=\frac{5369}{100}-\frac{147}{10}=\frac{3899}{100}.
$$

Hence the requested [standard deviation](../../../variance.md#standard-deviation) is

$$
\boxed{\operatorname{sd}(N)=\frac{\sqrt{3899}}{10}\approx6.2442.}
$$

The hint rounds the sum of squares from $53.69$ to $53.7$; using that rounded value gives $\sqrt{39}\approx6.245$, consistent at the precision of the hint. The exact computation preserves the slightly more precise value above.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
