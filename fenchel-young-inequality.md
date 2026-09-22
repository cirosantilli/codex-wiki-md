<h1 id="fenchel-young-inequality">Fenchel–Young inequality</h1>

↑ **Parent:** [Convex conjugate](convex-conjugate.md)

The [Fenchel–Young inequality](fenchel-young-inequality.md) says that every input and every slope obey

$$
f(x)+f^*(p)\geq p\cdot x,\qquad x,p\in\mathbb R^n,
$$

where $f$ is any [proper extended-real function](proper-extended-real-function.md) and $f^*$ is its [convex conjugate](convex-conjugate.md). No [convexity](convex-function.md) assumption on $f$ is needed for this inequality: the defining [supremum](supremum.md) is at least the particular value $p\cdot x-f(x)$. If either term on the left is $+\infty$, the inequality still holds, but cannot be an equality because the [dot product](dot-product.md) on the right is finite.

For a [proper convex function](proper-convex-function.md), equality is equivalent to the [subgradient](subgradient.md) condition

$$
f(x)+f^*(p)=p\cdot x\quad\Longleftrightarrow\quad p\in\partial f(x).
$$

To see this, with $f(x)$ finite, equality says that $x$ attains the [supremum](supremum.md) defining $f^*(p)$, so $p\cdot z-f(z)\leq p\cdot x-f(x)$ for every $z$. Rearranging gives the [subgradient inequality](subgradient-inequality.md) $f(z)\geq f(x)+p\cdot(z-x)$. Geometrically, the [affine minorant](affine-minorant.md) $\ell_p(z)=p\cdot z-f^*(p)$ touches $f$ at $x$.

If the [proper convex function](proper-convex-function.md) is also closed, meaning its [epigraph](epigraph.md) is a [closed set](closed-set.md), or equivalently it is [lower semicontinuous](lower-semicontinuity.md), then

$$
p\in\partial f(x)\quad\Longleftrightarrow\quad x\in\partial f^*(p).
$$

The forward implication holds without closedness; the reverse one requires the additional hypothesis in general. Applying the equality criterion to $f^*$ relates $x\in\partial f^*(p)$ to $f^{**}(x)+f^*(p)=p\cdot x$, and the [Fenchel-Moreau theorem](fenchel-moreau-theorem.md) supplies $f^{**}=f$ when $f$ is closed. See [Bertsekas, Convex Optimization Theory: A Summary, §5.4.1, Proposition 5.4.3](https://ocw.mit.edu/courses/6-253-convex-analysis-and-optimization-spring-2012/db7bde2cd43e8dbaba11f6911311b87c_MIT6_253S12_summary.pdf#page=46) for precisely this distinction.

A concrete failure of the reverse implication occurs for the [indicator functional of a constraint set](indicator-functional-of-a-constraint-set.md) $f$ of the open interval $(-1,1)$. Its [convex conjugate](convex-conjugate.md) is $f^*(p)=|p|$: the endpoint gives the [supremum](supremum.md), even though it is excluded from the interval. At $(x,p)=(1,1)$, $x\in\partial f^*(p)=\{1\}$, but $f(1)=+\infty$, so equality fails and $\partial f(1)$ is empty. Closing the interval changes the endpoint value and restores equality there.

For the [convex quadratic function](convex-quadratic-function.md) $f(x)=x^2/2$, the [Fenchel–Young inequality](fenchel-young-inequality.md) is $x^2/2+p^2/2\geq px$, and equality holds exactly when $x=p$. For the [absolute value](absolute-value.md) $f(x)=|x|$, finite equality requires $p=\operatorname{sgn}(x)$ at $x\ne0$, where $\operatorname{sgn}$ is the [sign function](sign-function.md); at $x=0$ every $p\in[-1,1]$ gives equality. These are exactly the [subgradients](subgradient.md) of the [absolute value](absolute-value.md), including its entire interval of slopes at the corner.

**Table of contents**

- [Fenchel–Young gap](fenchel-young-gap.md)

## ↑ Ancestors (6)

1. [Convex conjugate](convex-conjugate.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Cramér-Lundberg workload exponent](cramer-lundberg-workload-exponent.md)
- [Fenchel-Moreau theorem](fenchel-moreau-theorem.md)
- [Fenchel–Young inequality](fenchel-young-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-26/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-348/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-211/5/c/solution.md)
- [Subgradient inversion under convex conjugacy](subgradient-inversion-under-convex-conjugacy.md)
- [Support-function subgradients as exposed faces](support-function-subgradients-as-exposed-faces.md)
