# Paper 3

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2007/PaperIB_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2007/PaperIB_3.pdf)

**Table of contents**

- [1G](#1g)
  - [Solution](#1g/solution)
- [2A](#2a)
  - [Solution](#2a/solution)
- [3H](#3h)
  - [Solution](#3h/solution)
  - [i](#3h/i)
    - [Solution](#3h/i/solution)
  - [ii](#3h/ii)
    - [Solution](#3h/ii/solution)
- [4A](#4a)
  - [a](#4a/a)
    - [Solution](#4a/a/solution)
  - [b](#4a/b)
    - [Solution](#4a/b/solution)
- [5F](#5f)
  - [Solution](#5f/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7B](#7b)
  - [Solution](#7b/solution)
- [8C](#8c)
  - [Solution](#8c/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
- [10G](#10g)
  - [i](#10g/i)
    - [Solution](#10g/i/solution)
  - [ii](#10g/ii)
    - [Solution](#10g/ii/solution)
- [11G](#11g)
  - [i](#11g/i)
    - [Solution](#11g/i/solution)
  - [ii](#11g/ii)
    - [Solution](#11g/ii/solution)
- [12A](#12a)
  - [Solution](#12a/solution)
- [13H](#13h)
  - [Solution](#13h/solution)
- [14H](#14h)
  - [Solution](#14h/solution)
- [15E](#15e)
  - [Solution](#15e/solution)
- [16B](#16b)
  - [Solution](#16b/solution)
- [17E](#17e)
  - [Solution](#17e/solution)
- [18D](#18d)
  - [Solution](#18d/solution)
- [19F](#19f)
  - [Solution](#19f/solution)
- [20C](#20c)
  - [Solution](#20c/solution)

## 1G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1g/solution">Solution</h3>

↑ **Parent:** [1G](#1g)

An element of the [general linear group over a finite field](../../../finite-group-theory.md#general-linear-group-over-a-finite-field) is an invertible $2\times2$ [matrix](../../../vector-space.md#matrix). Its columns must form an ordered [basis](../../../vector-space.md#basis) of $\mathbb F_p^2$. There are $p^2-1$ choices for the first column. Its [linear span](../../../vector-space.md#linear-span) contains $p$ vectors, so there are $p^2-p$ choices for a second column outside that [linear span](../../../vector-space.md#linear-span). Thus the [order of a general linear group over a finite field](../../../finite-group-theory.md#order-of-a-general-linear-group-over-a-finite-field) is

$$
\boxed{|GL_2(\mathbb F_p)|=(p^2-1)(p^2-p)=p(p-1)^2(p+1).}
$$

The [determinant](../../../linear-algebra.md#determinant) is a surjective [group homomorphism](../../../group-theory.md#group-homomorphism) $GL_2(\mathbb F_p)\to\mathbb F_p^\times$: for each $a\ne0$, the diagonal [matrix](../../../vector-space.md#matrix) $\operatorname{diag}(a,1)$ has [determinant](../../../linear-algebra.md#determinant) $a$. Its [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is the [special linear group over a finite field](../../../finite-group-theory.md#special-linear-group-over-a-finite-field). The [first isomorphism theorem](../../../group-theory.md#first-isomorphism-theorem) gives $|GL_2|/|SL_2|=p-1$, hence

$$
\boxed{|SL_2(\mathbb F_p)|=p(p^2-1).}
$$

## 2A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2a/solution">Solution</h3>

↑ **Parent:** [2A](#2a)

Choose orthonormal coordinates with origin $P$ and horizontal axis $l$. The [Euclidean reflection](../../../linear-algebra.md#reflection-mathematics) and [planar rotation](../../../linear-algebra.md#planar-rotation) have [matrices](../../../vector-space.md#matrix)

$$
S=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad R_\alpha=\begin{pmatrix}\cos\alpha&-\sin\alpha\\\sin\alpha&\cos\alpha\end{pmatrix}.
$$

Their [function composition](../../../algebra.md#function-composition) therefore satisfies the [composition of a plane rotation and a reflection](../../../linear-algebra.md#composition-of-a-plane-rotation-and-a-reflection) identity

$$
R_\alpha S=\begin{pmatrix}\cos\alpha&\sin\alpha\\\sin\alpha&-\cos\alpha\end{pmatrix}=R_{\alpha/2}S R_{-\alpha/2}.
$$

Conjugating by a [planar rotation](../../../linear-algebra.md#planar-rotation) transports the horizontal reflection axis to the line at angle $\alpha/2$. Equivalently, the vector $e=(\cos(\alpha/2),\sin(\alpha/2))$ is fixed, whereas its perpendicular $e_\perp=(-\sin(\alpha/2),\cos(\alpha/2))$ is sent to $-e_\perp$. Consequently **the fixed line is the line through $P$ obtained by rotating $l$ through $\alpha/2$, and $\tau\rho$ is reflection in that line**. Angles of an unoriented line are understood modulo $\pi$, so this description is independent of the representative chosen for $\alpha$ modulo $2\pi$.

## 3H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3h/solution">Solution</h3>

↑ **Parent:** [3H](#3h)

A real-valued function $f$ on an interval $I$ is [uniformly continuous](../../../topological-analysis.md#uniform-continuity) when

$$
\forall\varepsilon>0\ \exists\delta>0\ \forall x,y\in I:\quad |x-y|<\delta\ \Longrightarrow\ |f(x)-f(y)|<\varepsilon.
$$

The essential point in [uniform continuity](../../../topological-analysis.md#uniform-continuity) is that $\delta$ is independent of the locations of $x$ and $y$. **Uniform continuity on the whole real line does not imply boundedness**: $f(x)=x$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) with constant $1$, hence [uniformly continuous](../../../topological-analysis.md#uniform-continuity), but is unbounded.

<h3 id="3h/i">i</h3>

↑ **Parent:** [3H](#3h)

<h4 id="3h/i/solution">Solution</h4>

↑ **Parent:** [I](#3h/i)

Take $x_n=2\pi n$ and $y_n=2\pi n+1/n$. Then $|y_n-x_n|=1/n\to0$, while

$$
f(x_n)=0,\qquad f(y_n)=\left(2\pi n+\frac1n\right)\sin\frac1n\longrightarrow2\pi.
$$

The [sequential criterion for uniform continuity](../../../topological-analysis.md#sequential-criterion-for-uniform-continuity) would force $f(y_n)-f(x_n)\to0$. These pairs contradict it: for example, for all sufficiently large $n$ their output separation is greater than $\pi$, despite arbitrarily small input separation. Thus **$x\sin x$ is not uniformly continuous on $\mathbb R$**.

<h3 id="3h/ii">ii</h3>

↑ **Parent:** [3H](#3h)

<h4 id="3h/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3h/ii)

The [derivative](../../../calculus.md#derivative) is $f'(x)=-4x^3e^{-x^4}$. Its absolute value is [continuous](../../../calculus.md#continuous-function) and tends to zero as $x\to\pm\infty$, so it is bounded. More explicitly,

$$
\sup_{x\in\mathbb R}|f'(x)|=4\left(\frac34\right)^{3/4}e^{-3/4}=:M,
$$

obtained by differentiating $4t^3e^{-t^4}$ for $t\geq0$. The [mean value theorem](../../../calculus.md#mean-value-theorem) gives $|f(x)-f(y)|\leq M|x-y|$ for every $x,y$. Thus $f$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity), and choosing $\delta=\varepsilon/M$ proves **$e^{-x^4}$ is uniformly continuous on $\mathbb R$**.

## 4A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4a/a">a</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/a/solution">Solution</h4>

↑ **Parent:** [A](#4a/a)

Every point has arbitrarily small [path-connected](../../../geometry-and-topology.md#path-connected-space) open neighbourhoods. Indeed, in a [coordinate chart](../../../differential-geometry.md#manifold-chart) homeomorphic to $\mathbb R^n$, take the inverse image of a sufficiently small open [Euclidean ball](../../../functional-analysis.md#euclidean-ball). The ball is [convex](../../../real-analysis.md#convex-function), hence [path-connected](../../../geometry-and-topology.md#path-connected-space), and its inverse image is [path-connected](../../../geometry-and-topology.md#path-connected-space) by the [homeomorphism](../../../topology.md#homeomorphism). If the supplied neighbourhood is not itself open, first take an open neighbourhood within it and a ball contained in its chart image. This proves that $X$ is a [locally path-connected space](../../../geometry-and-topology.md#locally-path-connected-space).

Fix $x_0\in X$ and let $A$ consist of the points joined to $x_0$ by a [path](../../../geometry-and-topology.md#continuous-path). For $x\in A$, a [path-connected](../../../geometry-and-topology.md#path-connected-space) open neighbourhood $U_x$ is contained in $A$: concatenate a [path](../../../geometry-and-topology.md#continuous-path) from $x_0$ to $x$ with one from $x$ to any point of $U_x$. Hence $A$ is [open](../../../topology.md#open-set). For $x\notin A$, the same kind of neighbourhood cannot meet $A$, since a meeting point would provide a [path](../../../geometry-and-topology.md#continuous-path) to $x$. Hence $X\setminus A$ is also [open](../../../topology.md#open-set). Since $X$ is a [connected space](../../../geometry-and-topology.md#connected-space) and $A$ is nonempty, $A=X$. This proves **$X$ is path-connected**, including the general principle that [connected locally path-connected spaces are path-connected](../../../geometry-and-topology.md#connected-locally-path-connected-spaces-are-path-connected). The empty-space case, if allowed, is vacuous.

<h3 id="4a/b">b</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/b/solution">Solution</h4>

↑ **Parent:** [B](#4a/b)

Every nonempty [open set](../../../topology.md#open-set) in the given [topology](../../../topology.md) contains $1$. Suppose a [continuous map](../../../topology.md#continuous-map) $f$ took distinct values $f(m)$ and $f(n)$. Choose disjoint open intervals $U,V\subset\mathbb R$ containing these respective values. By [continuity](../../../calculus.md#continuous-function), $f^{-1}(U)$ and $f^{-1}(V)$ are nonempty [open sets](../../../topology.md#open-set) in $\mathbb N$, and therefore both contain $1$. This is impossible because the inverse images of disjoint sets are disjoint. Thus **every such continuous map is constant**. Conversely, constant maps are [continuous](../../../calculus.md#continuous-function). This is the [continuous real maps from the initial-segment topology](../../../topology.md#continuous-real-maps-from-the-initial-segment-topology) argument, using the [Hausdorff](../../../topology.md#hausdorff-space) separation of distinct real points.

## 5F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5f/solution">Solution</h3>

↑ **Parent:** [5F](#5f)

The principal real arctangent is defined here on $x\ne0$, so work on either of the two open half-planes. Put $r=\sqrt{x^2+y^2}$. Direct [differentiation](../../../calculus.md#differentiation) gives

$$
\phi_x=-\frac{y}{r^2},\qquad\phi_y=\frac{x}{r^2},\qquad\phi_{xx}=\frac{2xy}{r^4},\qquad\phi_{yy}=-\frac{2xy}{r^4}.
$$

Hence $\phi_{xx}+\phi_{yy}=0$: **$\phi$ is harmonic on its domain**. The [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) for $f=\phi+i\psi$ require

$$
\psi_x=-\phi_y=-\frac{x}{r^2},\qquad\psi_y=\phi_x=-\frac{y}{r^2}.
$$

Integrating these [partial derivatives](../../../calculus.md#partial-derivative) gives the [harmonic conjugate](../../../partial-differential-equation.md#harmonic-conjugate)

$$
\boxed{\psi(x,y)=-\log r+C_0=-\frac12\log(x^2+y^2)+C_0.}
$$

The constants may be chosen independently on the two components. The [harmonic angle and logarithmic radius](../../../partial-differential-equation.md#harmonic-angle-and-logarithmic-radius) representation supplies the [holomorphic function](../../../complex-analysis.md#holomorphic-function)

$$
\boxed{f(z)=\begin{cases}-i\operatorname{Log}z+iC_0,&\operatorname{Re}z>0,\\-i\operatorname{Log}(-z)+iC_0,&\operatorname{Re}z<0,\end{cases}}
$$

where $\operatorname{Log}$ is the [branch of the complex logarithm](../../../analysis.md#branch-of-the-complex-logarithm) on the right half-plane. On the left half-plane it is the angle of $-z$, rather than the principal angle of $z$, that equals $\arctan(y/x)$. This distinguishes the literal arctangent from a globally defined argument; no single-valued [complex logarithm](../../../analysis.md#complex-logarithm) exists on the whole punctured plane.

With $C_0=0$, the [level sets](../../../topology.md#level-set) $\phi=C$, for $-\pi/2<C<\pi/2$, are the two opposite rays of $y=x\tan C$ with the origin removed. On each half-plane only one ray remains. The [level sets](../../../topology.md#level-set) $\psi=K$ are circles $r=e^{-K}$, with their two points on $x=0$ excluded from the literal domain. The rays and circles meet at right angles, as expected for [harmonic conjugates](../../../partial-differential-equation.md#harmonic-conjugate).

<a id="5f/image-angle-contours-are-opposite-rays-logarithmic-radius-contours-are-circles-on-the-two-half-planes-x-ne0"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3-harmonic-contours.png)

**[Figure 1](#5f/image-angle-contours-are-opposite-rays-logarithmic-radius-contours-are-circles-on-the-two-half-planes-x-ne0). Angle contours are opposite rays; logarithmic-radius contours are circles, on the two half-planes $x\ne0$.**

## 6E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

For a differentiable equality constraint, the [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) method finds candidate [extrema](../../../mathematical-optimization.md#maximum-and-minimum) by solving

$$
\nabla f=\lambda\nabla g,\qquad g=c.
$$

The condition requires $\nabla g\ne0$ at the point: every tangent direction to the constraint is perpendicular to $\nabla g$, and at a [extremum](../../../mathematical-optimization.md#maximum-and-minimum) the directional [derivative](../../../calculus.md#derivative) of $f$ vanishes in every such direction. Thus $\nabla f$ is parallel to $\nabla g$. One must then classify candidates and check any singular or boundary cases.

For the [ellipsoid](../../../geometry-and-topology.md#ellipsoid), its constraint [gradient](../../../calculus.md#gradient) never vanishes on the surface, and its [compactness](../../../topology.md#compact-space) guarantees a maximum and a minimum. The [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equations become

$$
y=\frac{2\lambda x}{a^2},\qquad x=\frac{2\lambda y}{b^2},\qquad0=\frac{2\lambda z}{c^2}.
$$

If $\lambda=0$, then $x=y=0$ and $z=\pm c$, giving value $0$. If $\lambda\ne0$, then $z=0$; neither $x$ nor $y$ can vanish on this part of the surface. Combining the first two equations gives $4\lambda^2=a^2b^2$, and then $y=\pm(b/a)x$. The constraint yields $x^2=a^2/2$ and $y^2=b^2/2$. Therefore

$$
\boxed{\max xy=\frac{ab}{2},\qquad\min xy=-\frac{ab}{2}.}
$$

The maximum occurs at $(a/\sqrt2,b/\sqrt2,0)$ and its negative; the minimum at $(a/\sqrt2,-b/\sqrt2,0)$ and its negative. To verify these are the global [extrema](../../../mathematical-optimization.md#maximum-and-minimum), use

$$
\frac{2|xy|}{ab}\leq\frac{x^2}{a^2}+\frac{y^2}{b^2}\leq1.
$$

Equality is attained at exactly the points just found. The remaining two candidates have value $0$ between the extremal values.

## 7B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7b/solution">Solution</h3>

↑ **Parent:** [7B](#7b)

For the [quantum harmonic oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator), split the two [expectation values](../../../quantum-mechanics.md#expectation-value) into their [variances](../../../variance.md) and squared means:

$$
E=\frac{(\Delta p)^2}{2m}+\frac{m\omega^2(\Delta x)^2}{2}+\frac{\langle p\rangle^2}{2m}+\frac{m\omega^2\langle x\rangle^2}{2}.
$$

The last two terms are nonnegative, so

$$
\boxed{E\geq\frac{(\Delta p)^2}{2m}+\frac{m\omega^2(\Delta x)^2}{2}.}
$$

Apply the [arithmetic-geometric mean inequality](../../../mathematical-optimization.md#arithmetic-geometric-mean-inequality) to the two remaining nonnegative terms, then the [Heisenberg uncertainty principle](../../../quantum-theory.md#heisenberg-uncertainty-relation):

$$
E\geq2\sqrt{\frac{(\Delta p)^2}{2m}\frac{m\omega^2(\Delta x)^2}{2}}=\omega\Delta p\Delta x\geq\boxed{\frac{\hbar\omega}{2}}.
$$

The argument applies to any normalized state with finite oscillator energy; the stated [stationary state](../../../quantum-mechanics.md#stationary-state) is a particular case. Equality requires zero position and momentum means, minimum [quantum uncertainty](../../../quantum-mechanics.md#quantum-uncertainty), and balanced kinetic and potential contributions, as in the oscillator [ground state](../../../quantum-mechanics.md#ground-state).

## 8C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8c/solution">Solution</h3>

↑ **Parent:** [8C](#8c)

Under the null hypothesis, the defect count in each packet has a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $3,\theta$. The [likelihood](../../../statistical-modelling.md#likelihood-function), apart from factors independent of $\theta$, is

$$
L(\theta)\propto\theta^{94+2(40)+3(6)}(1-\theta)^{3(116)+2(94)+40}=\theta^{192}(1-\theta)^{576}.
$$

The [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) is therefore

$$
\boxed{\widehat\theta=\frac{192}{768}=\frac14.}
$$

The fitted [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) probabilities for counts $0,1,2,3$ are $27/64,27/64,9/64,1/64$, yielding expected packet counts $108,108,36,4$. The [Pearson chi-squared goodness-of-fit test](../../../statistical-modelling.md#pearson-chi-squared-goodness-of-fit-test) uses

$$
X^2=\frac{(116-108)^2}{108}+\frac{(94-108)^2}{108}+\frac{(40-36)^2}{36}+\frac{(6-4)^2}{4}=\boxed{\frac{104}{27}\simeq3.852}.
$$

For [binomial goodness-of-fit with an estimated parameter](../../../statistical-modelling.md#binomial-goodness-of-fit-with-an-estimated-parameter), there are $4-1-1=2$ [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom): the category counts have a fixed total, and one parameter was estimated. At the conventional $5\%$ level the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with two [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom) has upper critical value $5.99$, so **the data do not reject the independent common-defect-probability model**. The approximate [p-value](../../../statistical-modelling.md#p-value) is $e^{-X^2/2}\simeq0.146$; even at $10\%$, the critical value $4.61$ exceeds the observed statistic.

This is a goodness-of-fit conclusion rather than proof that individual bulbs are independent. The last expected count is only $4$, so the [chi-squared asymptotic approximation](../../../probability-theory.md#chi-squared-asymptotic-approximation) is somewhat marginal in that cell. The stated calibration is the usual asymptotic test with all four cells retained; if more accurate small-count inference is required, calibrate the fitted statistic under the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) model. Pooling cells would require a corresponding treatment of parameter fitting and test calibration.

## 9C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

Write $u_n=\mathbb P(X_n=0\mid X_0=0)$. The [Markov property](../../../markov-process.md#markov-property), conditioning on the state at time $n$, gives

$$
u_{n+1}=\alpha u_n+(1-\beta)(1-u_n)=(\alpha+\beta-1)u_n+1-\beta,\qquad u_0=1.
$$

Put $r=\alpha+\beta-1$ and $\pi_0=(1-\beta)/(2-\alpha-\beta)$. Then $\pi_0=r\pi_0+1-\beta$, so subtraction yields $u_{n+1}-\pi_0=r(u_n-\pi_0)$. Iterating this [linear recurrence](../../../algebra.md#linear-recurrence-relation) gives

$$
\boxed{u_n=\frac{1-\beta+(1-\alpha)(\alpha+\beta-1)^n}{2-\alpha-\beta},\qquad n\geq0.}
$$

For $r=0$, read the $n=0$ expression using $r^0=1$, or state $u_0=1$ separately; for $n\geq1$, $u_n=\pi_0$. Since $|r|<1$, the result also shows [convergence in a metric space](../../../topological-analysis.md#convergence-in-a-metric-space) to the [stationary distribution](../../../markov-process.md#stationary-distribution) probability $\pi_0$.

## 10G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10g/i">i</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/i/solution">Solution</h4>

↑ **Parent:** [I](#10g/i)

The [row rank](../../../vector-space.md#row-rank) of a [matrix](../../../vector-space.md#matrix) is the [dimension](../../../vector-space.md#dimension-vector-space) of the [linear span](../../../vector-space.md#linear-span) of its row vectors. Its [column rank](../../../vector-space.md#column-rank) is the [dimension](../../../vector-space.md#dimension-vector-space) of the [linear span](../../../vector-space.md#linear-span) of its column vectors, equivalently the [dimension](../../../vector-space.md#dimension-vector-space) of the [image](../../../set-theory.md#image-of-a-function) of the corresponding [linear map](../../../vector-space.md#linear-map). The [equality of row rank and column rank](../../../linear-algebra.md#equality-of-row-rank-and-column-rank) states that **these two numbers are equal for every matrix**. Their common value is the [rank of a matrix](../../../vector-space.md#matrix-rank).

<h3 id="10g/ii">ii</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10g/ii)

Regard $B$ as a [linear map](../../../vector-space.md#linear-map) $\mathbb R^n\to\mathbb R^p$ and $A$ as a [linear map](../../../vector-space.md#linear-map) $\mathbb R^p\to\mathbb R^m$ (the same argument holds over any [field](../../../algebra.md#field)). Then

$$
\operatorname{im}(AB)=A(\operatorname{im}B)\subseteq\operatorname{im}A.
$$

Its [dimension](../../../vector-space.md#dimension-vector-space) cannot exceed either $\dim\operatorname{im}A$ or $\dim\operatorname{im}B$, since applying a [linear map](../../../vector-space.md#linear-map) cannot increase [dimension](../../../vector-space.md#dimension-vector-space). The [rank bound for a matrix product](../../../vector-space.md#rank-bound-for-a-matrix-product) is therefore

$$
\boxed{\operatorname{rank}(AB)\leq\min\{\operatorname{rank}A,\operatorname{rank}B\}\leq p.}
$$

The bound $p$ is attained when

$$
A=\begin{pmatrix}I_p\\0_{(m-p)\times p}\end{pmatrix},\qquad B=\begin{pmatrix}I_p&0_{p\times(n-p)}\end{pmatrix}.
$$

Their product has an $I_p$ block and zeros elsewhere, so its [rank of a matrix](../../../vector-space.md#matrix-rank) is $p$. Thus the bound depending only on the given [matrix](../../../vector-space.md#matrix) sizes is **sharp**.

## 11G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11g/i">i</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/i/solution">Solution</h4>

↑ **Parent:** [I](#11g/i)

Write the [cardinality](../../../set-theory.md#cardinality) of the finite [group](../../../group.md) as $|G|=p^am$, where $p$ is [prime](../../../number-theory.md#prime-number) and $p\nmid m$. The [Sylow theorems](../../../finite-group-theory.md#sylow-theorems) say that a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of order $p^a$ exists; every [p-group](../../../finite-group-theory.md#p-group) is contained in a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup); and all [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) are [conjugate subgroups](../../../group-theory.md#conjugate-subgroup). If $n_p$ is their number, then

$$
\boxed{n_p\equiv1\pmod p,\qquad n_p\mid m.}
$$

Equivalently, for a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) $P$, conjugation and the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) give $n_p=[G:N_G(P)]$, where $N_G(P)$ is the [normalizer](../../../group-theory.md#normalizer). The containment statement is often included in the conjugacy form: every [p-group](../../../finite-group-theory.md#p-group) lies in a conjugate of any fixed [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup).

<h3 id="11g/ii">ii</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11g/ii)

The [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_5$ has [cardinality](../../../set-theory.md#cardinality) $5!=120=3\cdot40$, so its [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) for $p=3$ have [cardinality](../../../set-theory.md#cardinality) $3$. One example is

$$
\boxed{\langle(123)\rangle=\{e,(123),(132)\}.}
$$

Every nonidentity [permutation](../../../combinatorics.md#permutation) of [order of a group element](../../../group-theory.md#order-of-a-group-element) $3$ in $S_5$ is a single [permutation cycle](../../../finite-group-theory.md#permutation-cycle) of length $3$: two disjoint length-three [permutation cycles](../../../finite-group-theory.md#permutation-cycle) would require six letters. Choose the three moved letters in $\binom53$ ways, then one of their two length-three [permutation cycles](../../../finite-group-theory.md#permutation-cycle), giving $20$ such elements. Each subgroup of [cardinality](../../../set-theory.md#cardinality) $3$ has exactly two nonidentity elements, and distinct such subgroups have no nonidentity element in common. Consequently

$$
\boxed{n_3(S_5)=\frac{\binom53\,2}{2}=10.}
$$

This also satisfies the numerical [Sylow theorem](../../../finite-group-theory.md#sylow-theorems) restrictions $10\mid40$ and $10\equiv1\pmod3$.

## 12A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

For a regular [parametrized surface](../../../calculus.md#parametrized-surface) $\sigma(u,v)$, the [first fundamental form](../../../differential-geometry.md#first-fundamental-form) is the induced metric

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,\qquad E=\sigma_u\cdot\sigma_u,\quad F=\sigma_u\cdot\sigma_v,\quad G=\sigma_v\cdot\sigma_v.
$$

Choose the [unit normal](../../../differential-geometry.md#unit-normal) $N=(\sigma_u\times\sigma_v)/|\sigma_u\times\sigma_v|$. With the convention $II_{ij}=N\cdot\sigma_{ij}$, the [second fundamental form](../../../second-fundamental-form.md) is

$$
II=e\,du^2+2f\,du\,dv+g\,dv^2,\qquad e=N\cdot\sigma_{uu},\quad f=N\cdot\sigma_{uv},\quad g=N\cdot\sigma_{vv}.
$$

The [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature), the product of the [principal curvatures](../../../second-fundamental-form.md#principal-curvature), is

$$
\boxed{K=\frac{eg-f^2}{EG-F^2}.}
$$

For a compact [smooth embedded surface](../../../differential-geometry.md#smooth-embedded-surface) without boundary, the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) gives

$$
\boxed{\int_S K\,dA=2\pi e(S),}
$$

where $e(S)$ is the [Euler characteristic](../../../homology.md#euler-characteristic). The no-boundary condition is needed for this form; a [smooth embedded surface](../../../differential-geometry.md#smooth-embedded-surface) with boundary has the additional boundary [geodesic curvature](../../../differential-geometry.md#geodesic-curvature) integral.

For the [surface of revolution](../../../differential-geometry.md#surface-of-revolution), use

$$
\sigma(u,v)=\bigl((r+a\sin u)\cos v,(r+a\sin u)\sin v,b\cos u\bigr).
$$

The parameters are periodic, with local open parameter rectangles providing the [coordinate charts](../../../differential-geometry.md#manifold-chart). Put $R=r+a\sin u$ and $D=\sqrt{a^2\cos^2u+b^2\sin^2u}$. Since $r>a>0$ and $b>0$, both $R$ and $D$ are positive. The tangent vectors are

$$
\sigma_u=(a\cos u\cos v,a\cos u\sin v,-b\sin u),\qquad\sigma_v=(-R\sin v,R\cos v,0).
$$

Their [inner products](../../../linear-algebra.md#inner-product) are $E=D^2$, $F=0$, and $G=R^2$. Thus

$$
\boxed{I=(a^2\cos^2u+b^2\sin^2u)\,du^2+(r+a\sin u)^2\,dv^2.}
$$

Their [cross product](../../../vector-space.md#cross-product) is $R(b\sin u\cos v,b\sin u\sin v,a\cos u)$, so its normalization gives the outward [unit normal](../../../differential-geometry.md#unit-normal)

$$
N=\frac1D(b\sin u\cos v,b\sin u\sin v,a\cos u).
$$

Next,

$$
\begin{aligned}
\sigma_{uu}&=(-a\sin u\cos v,-a\sin u\sin v,-b\cos u),\\
\sigma_{uv}&=(-a\cos u\sin v,a\cos u\cos v,0),\\
\sigma_{vv}&=(-R\cos v,-R\sin v,0).
\end{aligned}
$$

Taking their [inner products](../../../linear-algebra.md#inner-product) with $N$ yields $e=-ab/D$, $f=0$, and $g=-bR\sin u/D$. Hence the [fundamental forms of an elliptic ring torus](../../../second-fundamental-form.md#fundamental-forms-of-an-elliptic-ring-torus) give

$$
\boxed{II=-\frac{ab}{\sqrt{a^2\cos^2u+b^2\sin^2u}}\,du^2-\frac{b(r+a\sin u)\sin u}{\sqrt{a^2\cos^2u+b^2\sin^2u}}\,dv^2.}
$$

Choosing the inward [unit normal](../../../differential-geometry.md#unit-normal) changes both displayed coefficients of $II$ to their negatives and leaves $I$ and $K$ unchanged. As a consistency check, $K=ab^2\sin u/(RD^4)$; its integral over the [torus](../../../topology.md#torus) is zero, since $K\,dA=ab^2\sin u\,du\,dv/D^3$ cancels under $u\mapsto u+\pi$. This agrees with $e(S)=0$ in the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem).

## 13H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="13h/solution">Solution</h3>

↑ **Parent:** [13H](#13h)

The proposed [norm](../../../functional-analysis.md#norm) is finite because every [continuous function](../../../calculus.md#continuous-function) on $[0,1]$ is bounded and integrable. It is nonnegative. If $\|f\|=0$ and $f(x_0)\ne0$ at some point, [continuity](../../../calculus.md#continuous-function) gives a nontrivial interval within $[0,1]$ on which $|f|$ is bounded below by a positive constant, contradicting the zero integral. Thus $\|f\|=0$ implies $f=0$. The converse is immediate. Absolute homogeneity follows from $|cf(x)|=|c||f(x)|$, and the pointwise inequality $|f(x)+g(x)|\leq|f(x)|+|g(x)|$ integrates to the [triangle inequality](../../../topological-analysis.md#triangle-inequality). These establish **all the norm axioms**, so $V$ is a [normed vector space](../../../functional-analysis.md#normed-vector-space).

To test the [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) condition, compare the terms with indices $n$ and $2n$. Put $d_n(x)=\sin(nx)-\sin(2nx)$. The identities $2\sin(nx)\sin(2nx)=\cos(nx)-\cos(3nx)$ and $2\sin^2(nx)=1-\cos(2nx)$ give

$$
\begin{aligned}
\int_0^1d_n(x)^2\,dx
&=\int_0^1\sin^2(nx)\,dx+\int_0^1\sin^2(2nx)\,dx-2\int_0^1\sin(nx)\sin(2nx)\,dx\\
&=1-\frac{\sin(2n)}{4n}-\frac{\sin(4n)}{8n}-\frac{\sin n}{n}+\frac{\sin(3n)}{3n}\longrightarrow1.
\end{aligned}
$$

Because $|d_n(x)|\leq2$, we have $d_n(x)^2\leq2|d_n(x)|$. Therefore

$$
\liminf_{n\to\infty}\|f_n-f_{2n}\|\geq\frac12.
$$

In particular, for all sufficiently large $n$, these arbitrarily late pairs have [norm](../../../functional-analysis.md#norm) distance greater than $1/4$. This proves the [sine sequence is not Cauchy in the integral norm](../../../measure-theory.md#sine-sequence-is-not-cauchy-in-the-integral-norm). Thus **the sequence is not Cauchy and does not converge to an element of $V$**, since every [norm convergent](../../../functional-analysis.md#norm-convergence) sequence is [Cauchy](../../../real-analysis.md#cauchy-sequence). This direct separation argument does not rely on [completeness](../../../topological-analysis.md#completeness) of $V$.

## 14H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="14h/solution">Solution</h3>

↑ **Parent:** [14H](#14h)

An [entire function](../../../complex-analysis.md#entire-function) that is doubly [periodic](../../../function.md#periodic-function) is bounded: its absolute value has a finite maximum on the compact square $[0,1]+i[0,1]$, and periodic translations carry every point of $\mathbb C$ into that square. The [Liouville theorem](../../../complex-analysis.md#liouville-theorem) therefore proves **every such analytic function is constant**.

For the zero-pole count, suppose the [meromorphic function](../../../isolated-singularity.md#meromorphic-function) is not identically zero; otherwise isolated zero multiplicities are not defined. It has only finitely many [zeros](../../../polynomial.md#zero-of-a-function) and [poles](../../../isolated-singularity.md#pole) modulo the lattice $\Lambda=\mathbb Z+i\mathbb Z$, because a compact square can be covered by finitely many local meromorphic neighbourhoods. Choose a translated unit square with no [zeros](../../../polynomial.md#zero-of-a-function) or [poles](../../../isolated-singularity.md#pole) on its boundary. The [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) $f'/f$ is doubly [periodic](../../../function.md#periodic-function), so integrals on opposite sides cancel, with their opposite orientations. The [argument principle](../../../complex-analysis.md#argument-principle) gives

$$
\boxed{N-P=\frac1{2\pi i}\oint\frac{f'(z)}{f(z)}\,dz=0.}
$$

Both counts include multiplicities. Each half-open [fundamental parallelogram](../../../complex-analysis.md#fundamental-parallelogram-of-a-period-lattice) contains exactly one representative of each lattice orbit, and translation by a lattice vector preserves the multiplicity of a [zero](../../../polynomial.md#zero-of-a-function) or [pole](../../../isolated-singularity.md#pole). Consequently the counts agree in the prescribed half-open square too, even if that particular square has boundary [zeros](../../../polynomial.md#zero-of-a-function) or [poles](../../../isolated-singularity.md#pole). Nonzero constants have both counts zero.

For the series, let $\Lambda=\mathbb Z+i\mathbb Z$ and write it as the [Weierstrass elliptic function](../../../complex-analysis.md#weierstrass-elliptic-function) $\wp(z)$. On a compact set avoiding $\Lambda$, choose $R$ with $|z|\leq R$. For $|w|>2R$,

$$
\frac1{(z-w)^2}-\frac1{w^2}=\frac{2wz-z^2}{w^2(z-w)^2},\qquad \left|\frac1{(z-w)^2}-\frac1{w^2}\right|\leq\frac{C_R}{|w|^3}.
$$

There are $O(j)$ lattice points with $j\leq|w|<j+1$, hence $\sum_{w\ne0}|w|^{-3}$ converges by comparison with $\sum_jj^{-2}$. The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) proves absolute [locally uniform convergence](../../../real-analysis.md#locally-uniform-convergence) of the tail, and the finite remaining terms define [holomorphic functions](../../../complex-analysis.md#holomorphic-function) off their [poles](../../../isolated-singularity.md#pole). It follows that $\wp$ is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) off $\Lambda$. Near each $w_0\in\Lambda$, separate the term $(z-w_0)^{-2}$; the remaining terms converge locally uniformly to a [holomorphic function](../../../complex-analysis.md#holomorphic-function). Thus $\wp$ is [meromorphic](../../../isolated-singularity.md#meromorphic-function) on $\mathbb C$, with a double [pole](../../../isolated-singularity.md#pole) at each lattice point and no other [poles](../../../isolated-singularity.md#pole).

It remains to prove the required [periods](../../../mathematics.md#period-of-a-function), rather than merely assert them from the lattice. Termwise [differentiation](../../../calculus.md#differentiation), justified by [locally uniform convergence](../../../real-analysis.md#locally-uniform-convergence) of these holomorphic series, gives

$$
\wp'(z)=-2\sum_{w\in\Lambda}\frac1{(z-w)^3}.
$$

This series is absolutely locally uniformly convergent off $\Lambda$. For either generator $\omega=1,i$, reindexing $w\mapsto w-\omega$ proves $\wp'(z+\omega)=\wp'(z)$. Therefore $\wp(z+\omega)-\wp(z)$ has zero [derivative](../../../calculus.md#derivative) off $\Lambda$. Its principal parts at lattice points cancel, so it extends to an entire constant $c_\omega$.

The original convergent series is even: reindexing $w\mapsto-w$ gives $\wp(-z)=\wp(z)$. At $z=-\omega/2$, which is not a lattice point for either generator, evenness gives

$$
c_\omega=\wp(\omega/2)-\wp(-\omega/2)=0.
$$

Hence **the series defines a meromorphic function with periods $1$ and $i$**. This [termwise derivative proof of Weierstrass periodicity](../../../complex-analysis.md#termwise-derivative-proof-of-weierstrass-periodicity) uses an absolutely convergent derivative sum; splitting the original series into two separate inverse-square sums would not be justified.

## 15E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="15e/solution">Solution</h3>

↑ **Parent:** [15E](#15e)

Seek a [power series](../../../real-analysis.md#power-series) $y(x)=\sum_{k\geq0}a_kx^k$ in the [Legendre differential equation](../../../differential-equation.md#legendre-differential-equation). Equating coefficients of $x^k$ gives

$$
(k+2)(k+1)a_{k+2}+\bigl(n(n+1)-k(k+1)\bigr)a_k=0,
$$

so

$$
\boxed{a_{k+2}=\frac{(k-n)(k+n+1)}{(k+2)(k+1)}a_k.}
$$

The even and odd coefficients form separate chains. Choose a nonzero seed of the same parity as $n$ and set the other seed to zero. In the chosen chain, none of the factors vanishes before $k=n$, and the factor $k-n$ vanishes at $k=n$. Therefore this chain terminates with a nonzero $a_n$: it gives a [polynomial](../../../polynomial.md) of degree exactly $n$.

To impose the normalization, its value at $x=1$ must be nonzero. Suppose a nonzero polynomial solution were $y=(x-1)^mq(x)$ with $m\geq1$ and $q(1)\ne0$. The lowest-order coefficient in $(1-x^2)y''-2xy'$ would be $-2m^2q(1)(x-1)^{m-1}$, whereas $n(n+1)y$ has order $m$. This cannot satisfy the equation. Thus divide by $y(1)$ to obtain the [Legendre polynomial](../../../differential-equation.md#legendre-polynomial) $P_n$ with $P_n(1)=1$. Substitution or the coefficient recurrence gives

$$
\boxed{P_0(x)=1,\qquad P_1(x)=x,\qquad P_2(x)=\frac12(3x^2-1).}
$$

For an axisymmetric solution of the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) regular at the two polar axes, the separated modes and their superposition in [spherical polar coordinates](../../../calculus.md#spherical-coordinate-system) are

$$
\phi_n(r,\theta)=\bigl(A_nr^n+B_nr^{-n-1}\bigr)P_n(\cos\theta),\qquad
\phi(r,\theta)=\sum_{n=0}^\infty\bigl(A_nr^n+B_nr^{-n-1}\bigr)P_n(\cos\theta).
$$

This is the usual [separation of variables](../../../partial-differential-equation.md#separation-of-variables) expansion; the singular angular solutions are excluded by regularity at the axes.

Here $\sin^2\theta=\frac23(P_0(\cos\theta)-P_2(\cos\theta))$, so only degrees $0$ and $2$ are required. The degree-zero radial function $A_0+B_0/r$ takes the same value $2/3$ at $r=a,b$; since $a<b$, this forces $B_0=0$, $A_0=2/3$. Write the degree-two coefficient as $-(2/3)T(r)$, where $T=Ar^2+Br^{-3}$ and $T(a)=T(b)=1$. Multiplying these boundary equations by $a^3,b^3$ and subtracting gives

$$
A=\frac{b^3-a^3}{b^5-a^5},\qquad B=\frac{a^3b^3(b^2-a^2)}{b^5-a^5}.
$$

Consequently

$$
\boxed{\phi(r,\theta)=\frac23\left[1-\frac{(b^3-a^3)r^2+a^3b^3(b^2-a^2)r^{-3}}{b^5-a^5}P_2(\cos\theta)\right].}
$$

Each term is [harmonic](../../../partial-differential-equation.md#harmonic-function) in the shell, and the radial factor is $1$ at both boundaries, so this satisfies both [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition). The [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions), applied to the difference of two solutions, proves uniqueness among solutions continuous on the closed shell.

## 16B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="16b/solution">Solution</h3>

↑ **Parent:** [16B](#16b)

Expand the initial [wavefunction](../../../quantum-mechanics.md#wave-function) in the complete orthonormal [energy eigenstates](../../../quantum-mechanics.md#energy-eigenstate), with $c_n=\langle\psi_n,\Psi(0)\rangle$. The [unitary time evolution](../../../quantum-mechanics.md#unitary-time-evolution) is

$$
\boxed{\Psi(x,t)=\sum_{n=1}^\infty c_ne^{-iE_nt/\hbar}\psi_n(x),\qquad\sum_{n=1}^\infty|c_n|^2=1.}
$$

On the two-dimensional subspace spanned by $\psi_1,\psi_2$, the [observable](../../../quantum-mechanics.md#observable) has [matrix](../../../vector-space.md#matrix) $\begin{pmatrix}2&-1\\-1&2\end{pmatrix}$. Its normalized [eigenvectors](../../../linear-operator-theory.md#eigenvector) are the symmetric and antisymmetric combinations. A complete orthonormal [eigenbasis](../../../linear-operator-theory.md#eigenbasis) is therefore

$$
\boxed{\phi_1=\frac{\psi_1+\psi_2}{\sqrt2},\quad A\phi_1=\phi_1;\qquad
\phi_2=\frac{\psi_1-\psi_2}{\sqrt2},\quad A\phi_2=3\phi_2;\qquad
\phi_n=\psi_n,\quad A\phi_n=0\ (n\geq3).}
$$

The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1,3,0$, with $0$ infinitely degenerate. The first two are nondegenerate, regardless of the distinct energies $E_n$.

The first [measurement in quantum mechanics](../../../quantum-measurement.md), with outcome $3$, leaves the state $\phi_2$ up to an irrelevant phase. At time $t$ it has become

$$
\Psi(t)=\frac{e^{-iE_1t/\hbar}\psi_1-e^{-iE_2t/\hbar}\psi_2}{\sqrt2}.
$$

Its [probability amplitude](../../../quantum-mechanics.md#probability-amplitude) for outcome $1$ is

$$
\langle\phi_1,\Psi(t)\rangle=\frac12\left(e^{-iE_1t/\hbar}-e^{-iE_2t/\hbar}\right).
$$

The [Born rule](../../../quantum-mechanics.md#born-rule) gives the [two-level observable transition probability](../../../quantum-mechanics.md#two-level-observable-transition-probability)

$$
\boxed{\mathbb P(A(t)=1\mid A(0)=3)=\sin^2\left(\frac{(E_2-E_1)t}{2\hbar}\right).}
$$

## 17E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="17e/solution">Solution</h3>

↑ **Parent:** [17E](#17e)

Neglect end effects, so the [electrostatic potential](../../../electromagnetism.md#electric-potential) depends only on the cylindrical radius $r$. The radial [Laplace equation](../../../partial-differential-equation.md#laplace-equation) is $(r\phi')'=0$, with general solution $A\log r+B$. Imposing the conductor [boundary conditions](../../../differential-equation.md#boundary-condition) gives

$$
\boxed{\phi(r)=\begin{cases}\displaystyle V\frac{\log(r/a)}{\log\lambda},&a<r<\lambda a,\\[6pt]\displaystyle V\frac{\log(2a/r)}{\log(2/\lambda)},&\lambda a<r<2a.\end{cases}}
$$

The radial [electric field](../../../electromagnetism.md#electric-field) is $E_r=-\phi'$. Just inside the middle cylinder it is $-V/[\lambda a\log\lambda]$, directed towards the inner cylinder; just outside it is $V/[\lambda a\log(2/\lambda)]$, directed towards the outer cylinder. By [Gauss's law](../../../electromagnetism.md#gauss-s-law), its [charge per unit length](../../../electromagnetism.md#linear-charge-density) is

$$
q'=2\pi\epsilon_0\lambda a\bigl(E_r(\lambda a+)-E_r(\lambda a-)\bigr)=2\pi\epsilon_0V\left(\frac1{\log\lambda}+\frac1{\log(2/\lambda)}\right).
$$

Hence the [capacitance per unit length](../../../electromagnetism.md#capacitance-per-unit-length) is

$$
\boxed{C(\lambda)=2\pi\epsilon_0\left(\frac1{\log\lambda}+\frac1{\log(2/\lambda)}\right).}
$$

The two [coaxial cylindrical capacitors](../../../electromagnetism.md#coaxial-cylindrical-capacitor) contribute in parallel because both connect the middle cylinder to the same grounded potential. This is the [coaxial capacitor with grounded inner and outer cylinders](../../../electromagnetism.md#coaxial-capacitor-with-grounded-inner-and-outer-cylinders) construction.

For $\lambda=1+\delta$ with $\delta\to0^+$, $\log\lambda=\delta+O(\delta^2)$ while $\log(2/\lambda)\to\log2$. Therefore

$$
\boxed{C(1+\delta)\sim\frac{2\pi\epsilon_0}{\delta}.}
$$

The inner gap has width $a\delta$ and area per unit length approximately $2\pi a$. Its [parallel-plate capacitor](../../../electromagnetism.md#parallel-plate-capacitor) approximation gives exactly the same leading result; the outer gap contributes only a bounded correction.

For the [extremum](../../../mathematical-optimization.md#maximum-and-minimum), set $u=\log\lambda$, $L=\log2$, so $0<u<L$. Then

$$
\frac{C}{2\pi\epsilon_0}=\frac1u+\frac1{L-u},\qquad
\frac{d}{du}\frac{C}{2\pi\epsilon_0}=-\frac1{u^2}+\frac1{(L-u)^2},\qquad
\frac{d^2}{du^2}\frac{C}{2\pi\epsilon_0}=\frac2{u^3}+\frac2{(L-u)^3}>0.
$$

Thus the unique stationary point is $u=L/2$. Strict [convexity](../../../real-analysis.md#convex-function) and divergence at both endpoints show it is a global minimum:

$$
\boxed{\lambda=\sqrt2,\qquad C_{\min}=\frac{8\pi\epsilon_0}{\log2}.}
$$

There is no maximum on $1<\lambda<2$.

## 18D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="18d/solution">Solution</h3>

↑ **Parent:** [18D](#18d)

At the initial instant the [circulation](../../../fluid-mechanics.md#circulation-physics) around every closed curve is zero because the fluid is at rest. A smooth material-flow map carries closed curves bijectively between times. Conservation of [circulation](../../../fluid-mechanics.md#circulation-physics) around every [material curve](../../../fluid-mechanics.md#material-curve) therefore makes the line integral of the velocity zero around every closed curve at the current time, not just small contractible loops. Fix a reference point in a connected fluid region and define

$$
\phi(x)=\int_{x_0}^{x}\mathbf u\cdot d\mathbf l.
$$

The vanishing closed-curve integrals make this independent of the path. Thus $\mathbf u=\nabla\phi$: the fluid has a globally defined [velocity potential](../../../fluid-mechanics.md#velocity-potential). Its [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) condition is $\nabla\cdot\mathbf u=0$, hence **$\nabla^2\phi=0$**. This argument establishes the global potential without silently assuming the fluid region is [simply connected](../../../algebraic-topology.md#simply-connected-space).

Use the laboratory frame, with the sphere instantaneously centred at the origin and moving in the $\theta=0$ direction. Impermeability equates fluid and sphere normal velocities, while the fluid is at rest at infinity:

$$
\phi_r(a,\theta)=U\cos\theta,\qquad\nabla\phi\longrightarrow0\quad(r\to\infty).
$$

Choose the additive constant so that $\phi\to0$ at infinity. Substitution of $\phi=f(r)\cos\theta$ into the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) in [spherical polar coordinates](../../../calculus.md#spherical-coordinate-system) gives

$$
(r^2f')'-2f=0,\qquad f(r)=Ar+Br^{-2}.
$$

The far-field condition gives $A=0$, and $f'(a)=U$ gives $B=-Ua^3/2$. Therefore

$$
\boxed{\phi(r,\theta)=-\frac{Ua^3\cos\theta}{2r^2}.}
$$

The radial and polar velocity components are

$$
u_r=\phi_r=\frac{Ua^3\cos\theta}{r^3},\qquad u_\theta=\frac1r\phi_\theta=\frac{Ua^3\sin\theta}{2r^3}.
$$

For fluid density $\rho$, its [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is

$$
\begin{aligned}
T_f&=\frac\rho2\int_a^\infty\int_0^{2\pi}\int_0^\pi\frac{U^2a^6}{r^6}\left(\cos^2\theta+\frac14\sin^2\theta\right)r^2\sin\theta\,d\theta\,d\varphi\,dr\\
&=\frac\rho2U^2a^6\cdot\frac1{3a^3}\cdot2\pi
=\boxed{\frac{\pi\rho a^3U^2}{3}}.
\end{aligned}
$$

Thus $T_f=\frac12m_aU^2$ with [added mass of a sphere](../../../physics.md#added-mass-of-a-sphere) $m_a=2\pi\rho a^3/3$, half the mass of displaced fluid.

For the initial acceleration after release, let $\dot U$ denote the upward acceleration, $\mathcal V=4\pi a^3/3$, and $m_b=\rho_b\mathcal V$. At the instant $U=0$, the velocity-squared term in the [Unsteady Bernoulli equation](../../../fluid-mechanics.md#unsteady-bernoulli-equation) vanishes. The time derivative of the potential at the sphere is $\phi_t(a,\theta)=-a\dot U\cos\theta/2$; centre-motion corrections also vanish at this instant. Relative to hydrostatic pressure, the additional pressure is consequently

$$
p_{\mathrm{acc}}=-\rho\phi_t=\frac12\rho a\dot U\cos\theta.
$$

Its upward force on the sphere is

$$
F_{\mathrm{acc}}=-\int_{r=a}p_{\mathrm{acc}}\cos\theta\,dS=-\frac12\rho a\dot U\cdot\frac{4\pi a^2}{3}=-m_a\dot U.
$$

Adding [buoyancy](../../../fluid-mechanics.md#buoyancy) and weight, [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) gives $(m_b+m_a)\dot U=(\rho-\rho_b)\mathcal Vg$. Therefore

$$
\boxed{\dot U=\frac{2(\rho-\rho_b)g}{\rho+2\rho_b}.}
$$

This is the [acceleration of a freely falling sphere with added mass](../../../physics.md#acceleration-of-a-freely-falling-sphere-with-added-mass), with upward chosen positive. If $\rho_b>\rho$, the negative value represents a downward acceleration.

## 19F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="19f/solution">Solution</h3>

↑ **Parent:** [19F](#19f)

Use the weighted [inner product](../../../linear-algebra.md#inner-product)

$$
\langle f,g\rangle=\int_a^bf(x)g(x)w(x)\,dx,\qquad h_n=\langle Q_n,Q_n\rangle>0.
$$

Here the interval is nondegenerate and the indicated integrals are finite, as required for the given [orthogonal polynomials](../../../numerical-analysis.md#orthogonal-polynomial). Strict positivity follows because $w>0$ and a nonzero polynomial cannot vanish on an interval. Since each $Q_j$ is [monic](../../../polynomial.md#monic-polynomial) of degree $j$, $Q_0,\ldots,Q_{n+1}$ form a [basis](../../../vector-space.md#basis) of the polynomials of degree at most $n+1$. Comparing leading coefficients, expand

$$
xQ_n=Q_{n+1}+\sum_{j=0}^nc_jQ_j.
$$

By [orthogonality](../../../linear-algebra.md#orthogonal-vectors), $c_j=\langle xQ_n,Q_j\rangle/h_j$. For $j\leq n-2$, symmetry of multiplication by $x$ gives

$$
\langle xQ_n,Q_j\rangle=\langle Q_n,xQ_j\rangle=0,
$$

because $xQ_j$ has degree at most $n-1$ and is a [linear combination](../../../vector-space.md#linear-combination) of $Q_0,\ldots,Q_{n-1}$. Only the last two terms remain. Their coefficients are

$$
\boxed{a_n=\frac{\int_a^bxQ_n(x)^2w(x)\,dx}{\int_a^bQ_n(x)^2w(x)\,dx},\qquad
b_n=\frac{\int_a^bQ_n(x)Q_{n-1}(x)xw(x)\,dx}{h_{n-1}}=\frac{h_n}{h_{n-1}}>0\quad(n\geq1).}
$$

For the second equality, $xQ_{n-1}-Q_n$ has degree at most $n-1$, so its [inner product](../../../linear-algebra.md#inner-product) with $Q_n$ vanishes. Rearranging proves the [three-term recurrence for monic orthogonal polynomials](../../../numerical-analysis.md#three-term-recurrence-for-monic-orthogonal-polynomials):

$$
\boxed{Q_{n+1}=(x-a_n)Q_n-b_nQ_{n-1}.}
$$

For $n=0$ this reads $Q_1=x-a_0$ because $Q_{-1}=0$ and $Q_0=1$. The coefficient $b_0$ is therefore immaterial and is not determined by the polynomials. The usual convention is $b_0=0$; if a positive $b_0$ is desired, any positive value gives the identical recurrence. The strictly positive norm-ratio formula is the assertion for **$n\geq1$**, not a division by the norm of $Q_{-1}$.

## 20C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="20c/solution">Solution</h3>

↑ **Parent:** [20C](#20c)

For the [Lagrangian sufficiency theorem](../../../mathematical-optimization.md#lagrange-sufficiency-theorem), write a maximization problem as $\max_{x\in D}f(x)$ subject to $g_i(x)\leq c_i$. Here $D$ may already incorporate simple constraints such as nonnegativity. Define the [Lagrangian in optimization](../../../mathematical-optimization.md#optimization-lagrangian)

$$
L(x,\lambda)=f(x)-\sum_i\lambda_i(g_i(x)-c_i),\qquad\lambda_i\geq0.
$$

The theorem states that a feasible point $x_*$ is a global maximizer if there are such multipliers for which $x_*$ globally maximizes $L(\cdot,\lambda)$ on $D$ and [complementary slackness](../../../mathematical-optimization.md#complementary-slackness) holds: $\lambda_i(g_i(x_*)-c_i)=0$ for every $i$. To prove it, for any feasible $x$ observe that

$$
f(x)\leq L(x,\lambda)\leq L(x_*,\lambda)=f(x_*).
$$

The first inequality uses feasibility and nonnegative multipliers, the second uses global maximization of the [Lagrangian in optimization](../../../mathematical-optimization.md#optimization-lagrangian), and the last uses [complementary slackness](../../../mathematical-optimization.md#complementary-slackness). Thus **$x_*$ is globally optimal**. No convexity hypothesis is needed for this implication; [concavity](../../../real-analysis.md#concave-function) is useful when establishing the required global maximization of $L$ from its [gradient](../../../calculus.md#gradient).

For the particular problem, put $d=e^{c_2}-1\geq0$ and $R=c_1-2d\geq0$. The logarithmic constraint is equivalent to $x_1\geq d$. The objective increases strictly with either variable, so at a maximum the resource constraint is tight: otherwise $x_1$ could be increased. Hence

$$
x_1=\frac{c_1-3x_2}{2},\qquad0\leq x_2\leq\frac R3.
$$

On this interval the objective becomes $F(x_2)=(c_1-3x_2)/2+3\log(1+x_2)$, with

$$
F'(x_2)=-\frac32+\frac3{1+x_2},\qquad F''(x_2)=-\frac3{(1+x_2)^2}<0.
$$

It increases up to $x_2=1$ and decreases thereafter, so the unique feasible maximizer is

$$
\boxed{x_2^*=\min\left\{1,\frac{c_1-2(e^{c_2}-1)}3\right\},\qquad x_1^*=\frac{c_1-3x_2^*}{2}.}
$$

The maximum value is

$$
\boxed{\begin{cases}
\displaystyle d+3\log(1+R/3),&0\leq R\leq3,\\[3pt]
\displaystyle\frac{c_1-3}{2}+3\log2,&R\geq3.
\end{cases}}
$$

The two expressions agree at $R=3$. This includes the degenerate feasible set $R=0$, where $x_1^*=d$ and $x_2^*=0$.

To certify the result using the [Lagrangian sufficiency theorem](../../../mathematical-optimization.md#lagrange-sufficiency-theorem), take $D=[0,\infty)^2$ and

$$
L=x_1+3\log(1+x_2)-\lambda(2x_1+3x_2-c_1)+\mu(\log(1+x_1)-c_2),
$$

where $\lambda,\mu\geq0$. Set

$$
\lambda=\frac1{1+x_2^*},\qquad\mu=(2\lambda-1)(1+x_1^*).
$$

Since $x_2^*\leq1$, $\lambda\geq1/2$ and $\mu\geq0$. These choices make both components of $\nabla_xL$ vanish at $x_*$: $1-2\lambda+\mu/(1+x_1^*)=0$ and $3/(1+x_2^*)-3\lambda=0$. The [Lagrangian in optimization](../../../mathematical-optimization.md#optimization-lagrangian) is [concave](../../../real-analysis.md#concave-function) on $D$, so the zero [gradient](../../../calculus.md#gradient) proves global maximization there. The resource constraint is tight. When $R<3$ the logarithmic constraint is tight; when $R\geq3$, $\mu=0$. Thus [complementary slackness](../../../mathematical-optimization.md#complementary-slackness) holds in every case, including both endpoints, and the theorem establishes the claimed optimum.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
