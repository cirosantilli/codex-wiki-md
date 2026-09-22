# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2002/PaperIA_4.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2002/PaperIA_4.pdf)

**Table of contents**

- [1C](#1c)
  - [Solution](#1c/solution)
  - [i](#1c/i)
    - [Solution](#1c/i/solution)
  - [ii](#1c/ii)
    - [Solution](#1c/ii/solution)
  - [iii](#1c/iii)
    - [Solution](#1c/iii/solution)
  - [iv](#1c/iv)
    - [Solution](#1c/iv/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3E](#3e)
  - [Solution](#3e/solution)
- [4E](#4e)
  - [Solution](#4e/solution)
- [5F](#5f)
  - [Solution](#5f/solution)
- [6F](#6f)
  - [a](#6f/a)
    - [Solution](#6f/a/solution)
  - [b](#6f/b)
    - [Solution](#6f/b/solution)
  - [c](#6f/c)
    - [Solution](#6f/c/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [Solution](#7b/a/solution)
  - [b](#7b/b)
    - [Solution](#7b/b/solution)
- [8B](#8b)
  - [Solution](#8b/solution)
- [9E](#9e)
  - [Solution](#9e/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11E](#11e)
  - [Solution](#11e/solution)
- [12E](#12e)
  - [Solution](#12e/solution)

## 1C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1c/solution">Solution</h3>

↑ **Parent:** [1C](#1c)

An [injective function](../../../algebra.md#injective-function) satisfies $f(a)=f(a')\Rightarrow a=a'$ for all $a,a'\in A$. A [surjective function](../../../algebra.md#surjective-function) $g:A\to B$ satisfies: for every $b\in B$, some $a\in A$ has $g(a)=b$. The following arguments apply to [function composition](../../../algebra.md#function-composition) with the stated domains and codomains.

<h3 id="1c/i">i</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/i/solution">Solution</h4>

↑ **Parent:** [I](#1c/i)

Let $c\in C$. Since $g$ is [surjective](../../../algebra.md#surjective-function), choose $b\in B$ with $g(b)=c$. Since $f$ is [surjective](../../../algebra.md#surjective-function), choose $a\in A$ with $f(a)=b$. Then $(g\circ f)(a)=g(b)=c$. Thus every element of $C$ has a preimage, proving that $g\circ f$ is [surjective](../../../algebra.md#surjective-function).

<h3 id="1c/ii">ii</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1c/ii)

Suppose $(g\circ f)(a)=(g\circ f)(a')$. The [injectivity](../../../algebra.md#injective-function) of $g$ implies $f(a)=f(a')$, and the [injectivity](../../../algebra.md#injective-function) of $f$ then implies $a=a'$. Hence $g\circ f$ is [injective](../../../algebra.md#injective-function).

<h3 id="1c/iii">iii</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1c/iii)

If $f(a)=f(a')$, applying $g$ gives $(g\circ f)(a)=(g\circ f)(a')$. The [injectivity](../../../algebra.md#injective-function) of $g\circ f$ implies $a=a'$, so $f$ is [injective](../../../algebra.md#injective-function).

<h3 id="1c/iv">iv</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1c/iv)

For any $c\in C$, the [surjectivity](../../../algebra.md#surjective-function) of $g\circ f$ supplies $a\in A$ with $g(f(a))=c$. Therefore $f(a)\in B$ is a preimage of $c$ under $g$, proving [surjectivity](../../../algebra.md#surjective-function) of $g$.

For the requested counterexample, take $A=C=\{0\}$, $B=\{0,1\}$, $f(0)=0$, and $g(0)=g(1)=0$. The [function composition](../../../algebra.md#function-composition) is the identity [bijection](../../../function.md#bijection) of the singleton, but $f$ is not [surjective](../../../algebra.md#surjective-function) and $g$ is not [injective](../../../algebra.md#injective-function).

## 2C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

The base case $n=1$ is the [product rule](../../../calculus.md#product-rule). Suppose the [Leibniz rule](../../../calculus.md#leibniz-rule) holds at order $n$. Taking one more [derivative](../../../calculus.md#derivative) of each term and collecting the coefficient of $f^{(n+1-r)}g^{(r)}$ gives

$$
(fg)^{(n+1)}=\sum_{r=0}^{n+1}\left[\binom nr+\binom n{r-1}\right]f^{(n+1-r)}g^{(r)}.
$$

Here [binomial coefficients](../../../combinatorics.md#binomial-coefficient) outside $0\le r\le n$ are zero. For $1\le r\le n$, the factorial definition proves [Pascal's identity](../../../combinatorics.md#pascal-s-rule) directly:

$$
\binom nr+\binom n{r-1}=\frac{n!}{r!(n-r)!}+\frac{n!}{(r-1)!(n-r+1)!}=\frac{(n+1)!}{r!(n+1-r)!}=\binom{n+1}r.
$$

At $r=0,n+1$, the identity is $1+0=1$. Substitution gives the required order-$n+1$ formula, completing the [induction](../../../foundations-of-mathematics.md#mathematical-induction).

## 3E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3e/solution">Solution</h3>

↑ **Parent:** [3E](#3e)

Put $A=g\sin\alpha>0$ and $v=\dot x$. Multiplying the equation by $xv$ gives

$$
\frac d{dt}\frac{(xv)^2}2=Ax^2\dot x=\frac d{dt}\frac{Ax^3}3,
$$

so its [first integral](../../../differential-equation.md#first-integral) is

$$
\boxed{x^2v^2=\frac{2A}3x^3+c},\qquad v=\sqrt{\frac{2A}3x+\frac c{x^2}}.
$$

These level curves give the positive [phase plane](../../../dynamical-systems.md#phase-plane) for the [avalanche front with linear mass entrainment](../../../classical-mechanics.md#avalanche-front-with-linear-mass-entrainment). For $c<0$, the curve starts at $v=0$, $x=(-3c/(2A))^{1/3}$ and rises. For $c>0$, it diverges as $x\downarrow0$, has a minimum at $x=(3c/A)^{1/3}$, and then rises. The $c=0$ curve is $v=\sqrt{2Ax/3}$. Forward-time arrows have increasing $x$; at a zero-velocity endpoint the equation gives $\ddot x=A>0$.

<a id="3e/image-avalanche-phase-trajectories-approaching-the-linear-entrainment-asymptote"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4-avalanche-phase-plane.png)

**[Figure 1](#3e/image-avalanche-phase-trajectories-approaching-the-linear-entrainment-asymptote). Avalanche phase trajectories approaching the linear-entrainment asymptote**.

Every forward-moving trajectory has $x\to\infty$: after it has entered $v>0$, a bounded limiting $x$ would force a zero of the displayed positive-branch speed ahead of it, but its only possible zero is the lower endpoint. For large $x$,

$$
\frac{v}{\sqrt{2Ax/3}}=\sqrt{1+\frac{3c}{2Ax^3}}\longrightarrow1,\qquad v-\sqrt{2Ax/3}\longrightarrow0.
$$

Expanding the equation as $x\ddot x+v^2=Ax$ and substituting the [first integral](../../../differential-equation.md#first-integral) gives

$$
\boxed{\ddot x=\frac A3-\frac c{x^3}\longrightarrow\frac13g\sin\alpha}.
$$

Thus both the asymptotic [phase plane](../../../dynamical-systems.md#phase-plane) trajectory and the limiting [acceleration](../../../classical-mechanics.md#acceleration) are independent of the initial data.

## 4E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4e/solution">Solution</h3>

↑ **Parent:** [4E](#4e)

Apply the rotating-vector derivative rule first to the position [vector](../../../vector-space.md#vector) and then to its [velocity](../../../classical-mechanics.md#velocity). Since $\boldsymbol\omega$ is constant,

$$
\mathbf v=\mathbf v'+\boldsymbol\omega\times\mathbf x,\qquad \mathbf a=\mathbf a'+2\boldsymbol\omega\times\mathbf v'+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x).
$$

For example, the derivative of $\mathbf v'$ contributes $\mathbf a'+\boldsymbol\omega\times\mathbf v'$, while that of $\boldsymbol\omega\times\mathbf x$ contributes the other two terms. This is the [equation of motion in a rotating frame](../../../classical-mechanics.md#equation-of-motion-in-a-rotating-frame). The mutual [central forces](../../../physics.md#central-force) are unchanged in form because rotations preserve lengths and differences of position vectors. [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) for particle $i$ becomes

$$
m\mathbf a_i'=\sum_{j\ne i}\mathbf F_{ij}+e(\mathbf v_i'+\boldsymbol\omega\times\mathbf x_i)\times\mathbf B-2m\boldsymbol\omega\times\mathbf v_i'-m\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x_i).
$$

Set $\boldsymbol\omega=-e\mathbf B/(2m)$. The velocity-dependent [Lorentz force](../../../electromagnetism.md#lorentz-force) is $e\mathbf v_i'\times\mathbf B=-e\mathbf B\times\mathbf v_i'$, and it cancels the [Coriolis force](../../../physics.md#coriolis-force) $-2m\boldsymbol\omega\times\mathbf v_i'=e\mathbf B\times\mathbf v_i'$. The remaining terms combine to $m\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x_i)$ and are quadratic in the [magnetic field](../../../electromagnetism.md#magnetic-field). Neglecting them gives

$$
\boxed{m\mathbf a_i'=\sum_{j\ne i}\mathbf F_{ij}+O(B^2)},
$$

identical to the zero-field equations to first order. The [Larmor theorem](../../../electromagnetism.md#larmor-theorem) requires the common charge-to-mass ratio; a mixture with different ratios cannot use one rotating frame to cancel every magnetic term.

## 5F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5f/solution">Solution</h3>

↑ **Parent:** [5F](#5f)

A [set](../../../set.md) is [countable](../../../set-theory.md#countable-set) if it is finite or admits an [injection](../../../algebra.md#injective-function) into the natural numbers; an infinite [countable set](../../../set-theory.md#countable-set) can equivalently be listed as a sequence. Let $A=\bigcup_{i\ge1}A_i$ with each $A_i$ [countable](../../../set-theory.md#countable-set). Choose an enumeration of each nonempty $A_i$, allowing repetition if it is finite. List the pairs $(i,j)\in\mathbb N^2$ in successive finite diagonals of constant $i+j$ and output the $j$th member of $A_i$. This lists every member of $A$, so $A$ is [countable](../../../set-theory.md#countable-set); empty sets contribute nothing, and repetitions can be removed by retaining first occurrences. This is the [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) theorem, in the usual setting with [axiom of countable choice](../../../set-theory.md#axiom-of-countable-choice) for selecting the enumerations.

Each positive-length interval $J_i$ has a nonempty interior containing a [rational number](../../../number-theory.md#rational-number) by the [density of the rational numbers](../../../number-theory.md#density-of-the-rational-numbers). Fix one enumeration of the [rational numbers](../../../number-theory.md#rational-number) and let $q_i$ be its first member in the interior of $J_i$. Disjointness gives $i\ne j\Rightarrow q_i\ne q_j$, so $i\mapsto q_i$ is an [injection](../../../algebra.md#injective-function) of $I$ into a [countable set](../../../set-theory.md#countable-set). Hence $I$ is [countable](../../../set-theory.md#countable-set). This proof of the [countability of disjoint positive-length intervals](../../../set-theory.md#countability-of-disjoint-positive-length-intervals) uses a fixed enumeration and needs no arbitrary simultaneous choice of rationals.

## 6F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6f/a">a</h3>

↑ **Parent:** [6F](#6f)

<h4 id="6f/a/solution">Solution</h4>

↑ **Parent:** [A](#6f/a)

First, [finite additivity of a set function](../../../function.md#finite-additivity-of-a-set-function) gives $f(\varnothing)=0$, since $f(\varnothing)=2f(\varnothing)$. Put $w_s=f(\{s\})$. Decomposing any subset into its singleton elements and using [induction](../../../foundations-of-mathematics.md#mathematical-induction) gives $f(A)=\sum_{s\in A}w_s$. Fix $s\in S$ and let $r$ be the number of sets $A_i$ containing it. Its total coefficient in the alternating intersection sum is zero if $r=0$, and otherwise is

$$
\sum_{k=1}^r(-1)^{k+1}\binom rk=1-(1-1)^r=1
$$

by the [binomial theorem](../../../combinatorics.md#binomial-theorem). These are exactly the coefficients in $f(\bigcup_iA_i)$. Summing against $w_s$ proves the required [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) for the additive [set function](../../../function.md#set-function), including signed weights.

<h3 id="6f/b">b</h3>

↑ **Parent:** [6F](#6f)

<h4 id="6f/b/solution">Solution</h4>

↑ **Parent:** [B](#6f/b)

Take the finite ambient [set](../../../set.md) $S=\bigcup_iA_i$ and the additive [set function](../../../function.md#set-function) $f(A)=|A|$. Disjoint subsets have additive [cardinality](../../../set-theory.md#cardinality), so (a) applies and gives

$$
\boxed{\left|\bigcup_{i=1}^nA_i\right|=\sum_{\varnothing\ne J\subseteq\{1,\ldots,n\}}(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|}.
$$

This is the finite [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle).

<h3 id="6f/c">c</h3>

↑ **Parent:** [6F](#6f)

<h4 id="6f/c/solution">Solution</h4>

↑ **Parent:** [C](#6f/c)

In the [set](../../../set.md) of all $n!$ [permutations](../../../combinatorics.md#permutation), let $A_i$ consist of those fixing $i$. For a prescribed collection of $k$ fixed points, its intersection has $(n-k)!$ members. Applying the [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) to the complement of $\bigcup_iA_i$ gives the number of [derangements](../../../combinatorics.md#derangement-of-a-permutation):

$$
\boxed{d_n=\sum_{k=0}^n(-1)^k\binom nk(n-k)!=n!\sum_{k=0}^n\frac{(-1)^k}{k!}}.
$$

The convergent [power series](../../../real-analysis.md#power-series) for the [exponential function](../../../calculus.md#exponential-function) at $-1$ therefore gives $\boxed{d_n/n!\longrightarrow e^{-1}}$.

## 7B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/solution">Solution</h4>

↑ **Parent:** [A](#7b/a)

For each $1\le j\le p-1$, [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) gives $j^p\equiv j\pmod p$. Since $p$ is odd,

$$
\boxed{\sum_{j=1}^{p-1}j^p\equiv\sum_{j=1}^{p-1}j=\frac{p(p-1)}2\equiv0\pmod p}.
$$

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/solution">Solution</h4>

↑ **Parent:** [B](#7b/b)

Put $m=(p-1)/2$, so the requested modulus is $pm$. The [factorial](../../../combinatorics.md#factorial) $(p-1)!$ is divisible by $m$, and so is $p-1=2m$. Also, [Wilson's theorem](../../../number-theory.md#wilson-s-theorem) gives $(p-1)!\equiv-1\equiv p-1\pmod p$. Because $m$ and $p$ are [coprime integers](../../../number-theory.md#coprime-integers), their product divides the difference. Thus the [Wilson factorial congruence modulo a triangular number](../../../number-theory.md#wilson-factorial-congruence-modulo-a-triangular-number) is

$$
\boxed{(p-1)!\equiv p-1\pmod{p(p-1)/2}}.
$$

The displayed residue lies in the standard range even at $p=3$.

## 8B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8b/solution">Solution</h3>

↑ **Parent:** [8B](#8b)

For $b>1$, [Euler's theorem](../../../number-theory.md#euler-s-theorem) allows $d=\varphi(b)>0$, since $a,b$ are [coprime integers](../../../number-theory.md#coprime-integers). At $b=1$ every congruence holds and one may take $d=1$. Let $y$ be the [multiplicative order](../../../number-theory.md#multiplicative-order) of $a$ modulo $b$. Write a nonnegative exponent $x=qy+r$ with $0\le r<y$ using the [Euclidean division](../../../number-theory.md#euclidean-division). Then $a^x\equiv a^r\pmod b$, so $a^x\equiv1$ implies $r=0$ by minimality of $y$. Thus $y\mid x$. Negative exponents, if included, give the same conclusion using the inverse residue of $a$.

A [prime divisor of a Fermat number](../../../number-theory.md#prime-divisor-of-a-fermat-number) $F_n=2^{2^n}+1$ is odd, and satisfies $2^{2^n}\equiv-1\pmod p$. Therefore $2^{2^{n+1}}\equiv1\pmod p$, so its [multiplicative order](../../../number-theory.md#multiplicative-order) divides $2^{n+1}$. It does not divide $2^n$, since $-1\ne1$ modulo the odd prime. Every divisor of $2^{n+1}$ is a power of two, hence

$$
\boxed{\operatorname{ord}_p(2)=2^{n+1}}.
$$

By [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) and the divisibility just proved, $2^{n+1}\mid p-1$, giving $\boxed{p\equiv1\pmod{2^{n+1}}}$.

## 9E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9e/solution">Solution</h3>

↑ **Parent:** [9E](#9e)

For distinct positions and positive masses, [Newton's law of universal gravitation](../../../classical-mechanics.md#newton-s-law-of-universal-gravitation) gives

$$
m_i\ddot{\mathbf x}_i=-G\sum_{j\ne i}m_im_j\frac{\mathbf x_i-\mathbf x_j}{|\mathbf x_i-\mathbf x_j|^3}.
$$

The proposed [homothetic gravitational motion](../../../classical-mechanics.md#homothetic-gravitational-motion) has $\ddot{\mathbf x}_i=-(2/9)t^{-4/3}\mathbf a_i$ and pair distances $t^{2/3}|\mathbf a_i-\mathbf a_j|$, so cancellation of $t^{-4/3}$ gives the time-independent equations

$$
\boxed{\frac29\mathbf a_i=G\sum_{j\ne i}m_j\frac{\mathbf a_i-\mathbf a_j}{|\mathbf a_i-\mathbf a_j|^3}}.
$$

These define a [Newtonian central configuration](../../../classical-mechanics.md#newtonian-central-configuration) with this choice of scale. For

$$
\Phi=\frac19\sum_i m_i|\mathbf a_i|^2+\sum_{i<j}\frac{Gm_im_j}{|\mathbf a_i-\mathbf a_j|},
$$

[differentiation](../../../calculus.md#differentiation) in $\mathbf a_i$ gives $\nabla_{\mathbf a_i}\Phi=(2/9)m_i\mathbf a_i-G\sum_{j\ne i}m_im_j(\mathbf a_i-\mathbf a_j)/|\mathbf a_i-\mathbf a_j|^3=0$, exactly the displayed equations. The double sum in the paper counts each pair twice, so it agrees with this expression.

Multiply the configuration equations by $m_i$ and sum. Pair contributions cancel, giving $\sum_i m_i\mathbf a_i=0$. Thus the total [linear momentum](../../../classical-mechanics.md#momentum) is $\mathbf P=(2/3)t^{-1/3}\sum_i m_i\mathbf a_i=0$. Each position is parallel to its [velocity](../../../classical-mechanics.md#velocity), so every $m_i\mathbf x_i\times\dot{\mathbf x}_i=0$ and the total [angular momentum](../../../classical-mechanics.md#angular-momentum) is zero. About any other fixed point $\mathbf b$, it is $\mathbf L_{\mathbf b}=\mathbf L_O-\mathbf b\times\mathbf P=\boxed{\mathbf0}$.

## 10E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

A [central force](../../../physics.md#central-force) has zero [torque](../../../classical-mechanics.md#torque), so $h=r^2\dot\theta$ is constant and the [angular momentum](../../../classical-mechanics.md#angular-momentum) is $mh$. The [areal velocity](../../../classical-mechanics.md#areal-velocity) is $h/2$. Put $u=1/r$ and let primes denote angular [derivatives](../../../calculus.md#derivative). Then $\dot r=-hu'$, $\ddot r=-h^2u^2u''$, and $r\dot\theta^2=h^2u^3$. The radial equation with inward force magnitude $f(u)$ is $m(\ddot r-r\dot\theta^2)=-f(u)$, giving the [Binet equation](../../../classical-mechanics.md#binet-equation)

$$
\boxed{u''+u=\frac{f(u)}{mh^2u^2}}.
$$

Choose the angular origin along a diameter of a radius-$R$ circle through $O$. Its polar equation is $r=2R\cos\theta$, so $u=(2R)^{-1}\sec\theta$ on $-\pi/2<\theta<\pi/2$. Since $(\sec\theta)''+\sec\theta=2\sec^3\theta$, substitution gives $u''+u=8R^2u^3$ and hence

$$
\boxed{f(u)=cu^5,\qquad c=8mh^2R^2>0}.
$$

The force is **attractive**. For fixed force coefficient $c$ and mass, $R|mh|=\sqrt{mc/8}$, so $R$ is inversely proportional to the magnitude of the [angular momentum](../../../classical-mechanics.md#angular-momentum). The time along the circle is

$$
\boxed{T=\int_{-\pi/2}^{\pi/2}\frac{r^2}{|h|}\,d\theta=\frac{2\pi R^2}{|h|}=4\sqrt2\,\pi\sqrt{\frac mc}R^3}.
$$

This [circular orbit through an inverse-fifth-power singularity](../../../classical-mechanics.md#circular-orbit-through-an-inverse-fifth-power-singularity) reaches the force center at the two endpoints of this angular interval. The integral is finite; continuation through the singular collision is not specified by the force law alone.

## 11E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11e/solution">Solution</h3>

↑ **Parent:** [11E](#11e)

Neglecting gravity, the [equation of motion](../../../classical-mechanics.md#equation-of-motion) is $m\ddot{\mathbf x}=a\dot{\mathbf x}\times\mathbf x/r^3$, where $r=|\mathbf x|>0$. Dotting with the [velocity](../../../classical-mechanics.md#velocity) gives $d(m|\dot{\mathbf x}|^2/2)/dt=0$, because a [cross product](../../../vector-space.md#cross-product) is perpendicular to its factors. Thus the [speed](../../../classical-mechanics.md#speed) is constant. The [vector triple product](../../../calculus.md#vector-triple-product) gives

$$
\frac d{dt}(m\mathbf x\times\dot{\mathbf x})=\frac a{r^3}\mathbf x\times(\dot{\mathbf x}\times\mathbf x)=a\left(\frac{\dot{\mathbf x}}r-\frac{\mathbf x(\mathbf x\cdot\dot{\mathbf x})}{r^3}\right)=a\frac d{dt}\frac{\mathbf x}r.
$$

Hence the [generalized angular momentum in a radial monopole field](../../../classical-mechanics.md#generalized-angular-momentum-in-a-radial-monopole-field) is

$$
\boxed{\mathbf L=m\mathbf x\times\dot{\mathbf x}-a\frac{\mathbf x}r=\text{constant}}.
$$

Dotting with $\mathbf x$ gives $\mathbf L\cdot\mathbf x=-ar$, or $\widehat{\mathbf L}\cdot\widehat{\mathbf x}=-a/|\mathbf L|$. For $\mathbf L\ne0$, the direction of $\mathbf x$ therefore makes the fixed angle $\boxed{\cos\beta=-a/|\mathbf L|}$ with the axis $\mathbf L$, describing a [right circular conical surface](../../../geometry-and-topology.md#right-circular-conical-surface) with vertex at the North Pole. Orthogonality gives $|\mathbf L|^2=m^2|\mathbf x\times\dot{\mathbf x}|^2+a^2$, so this cosine is in $[-1,1]$. Radial motion gives a degenerate cone; when $a=0$ and the ordinary [angular momentum](../../../classical-mechanics.md#angular-momentum) is nonzero the cone is the usual orbital plane. If $\mathbf L=0$, the norm identity forces $a=0$ and $\mathbf x\times\dot{\mathbf x}=0$, giving a radial straight line.

## 12E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12e/solution">Solution</h3>

↑ **Parent:** [12E](#12e)

The [moment of inertia](../../../classical-mechanics.md#moment-of-inertia) of a uniform length-$2l$ rod about its transverse central axis is

$$
\boxed{I=\frac M{2l}\int_{-l}^ls^2\,ds=\frac13Ml^2}.
$$

The [kinetic energy decomposition about the center of mass](../../../classical-mechanics.md#kinetic-energy-decomposition-about-the-center-of-mass) gives $\boxed{T=MV^2/2+Ml^2\dot\theta^2/6}$ for center [speed](../../../classical-mechanics.md#speed) $V$ and rod angle $\theta$.

For a falling arch with $0<\alpha<\pi/2$, the symmetric [two hinged rods with both ends sliding on a floor](../../../classical-mechanics.md#two-hinged-rods-with-both-ends-sliding-on-a-floor) have the following motion. The hinge remains vertically over the arch center. Their centers are $\mathbf R_\pm=(\pm l\cos\theta,l\sin\theta)$, so each has squared [speed](../../../classical-mechanics.md#speed) $l^2\dot\theta^2$. Total [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is $T=4Ml^2\dot\theta^2/3$, and total gravitational [potential energy](../../../classical-mechanics.md#potential-energy) is $U=2Mgl\sin\theta$. [Conservation of energy](../../../physics.md#conservation-of-energy) from rest at angle $\alpha$ gives $\dot\theta^2=3g(\sin\alpha-\sin\theta)/(2l)$. At the hinge impact $\theta=0$, its height derivative is $2l\cos\theta\dot\theta$, giving

$$
\boxed{v_{\rm hinge}=\sqrt{6gl\sin\alpha}}.
$$

The floor-contact assumption is consistent: differentiating the energy relation gives $\ddot\theta=-3g\cos\theta/(4l)$, and the normal reaction on each outer endpoint is $N=Mg[1+9\sin^2\theta-6\sin\alpha\sin\theta]/4$. Completing the square shows $N\ge Mg\cos^2\alpha/4\ge0$ throughout the fall.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
