<h1 id="11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

**Local errors of the Euler schemes.** Let $h=\Delta t>0$, and evaluate $f$ and its partial [derivatives](../../../../derivative.md) at an exact starting point $(y(t),t)$. Define

$$
A=f_t+f_yf=y''(t).
$$

The exact [Taylor expansion](../../../../taylor-expansion.md) is $y(t+h)=y+hf+\tfrac12h^2A+O(h^3)$. The [forward Euler method](../../../../euler-method.md) retains only $y+hf$, so its one-step defect, exact minus computed value, is

$$
\boxed{\delta_E=\frac{h^2}2A+O(h^3)=O(h^2).}
$$

For the [Backward Euler method](../../../../backward-euler-method.md), substitution of the exact solution into the scheme gives the residual

$$
y(t+h)-y(t)-h f(y(t+h),t+h)=-\frac{h^2}2A+O(h^3),
$$

because $f(y(t+h),t+h)=f+hA+O(h^2)$. Under local smoothness, solving the implicit step changes this residual by a factor $1+O(h)$, so the one-step defect has the same leading term:

$$
\boxed{\delta_{BE}=-\frac{h^2}2A+O(h^3)=O(h^2).}
$$

These are unnormalized [local truncation errors](../../../../local-truncation-error.md), as in the question. A convention dividing by $h$ instead gives $O(h)$. Both schemes have first-order [global error](../../../../global-discretization-error.md) under the usual smoothness and stability hypotheses.

**Euler stability.** For the [Dahlquist test equation](../../../../dahlquist-test-equation.md) $y'=-\Lambda y$, put $z=h\Lambda$, with $\operatorname{Re}z>0$. The numerical [amplification factors](../../../../amplification-factor.md) are

$$
\boxed{R_E(z)=1-z,\qquad R_{BE}(z)=\frac1{1+z}.}
$$

Strict decay requires $|R|<1$; the boundary $|R|=1$ gives bounded but generally nondecaying values. For [Forward Euler method](../../../../euler-method.md),

$$
|1-h\Lambda|<1\quad\Longleftrightarrow\quad0<h<\frac{2\operatorname{Re}\Lambda}{|\Lambda|^2}.
$$

For positive real $\Lambda$, this reduces to $0<h\Lambda<2$. The [absolute stability](../../../../linear-stability-domain.md) region in the $z$ plane is the disk $|z-1|\leq1$. For [Backward Euler method](../../../../backward-euler-method.md), $|1+z|>1$ whenever $\operatorname{Re}z>0$, so it decays for every step size. It is [A-stable](../../../../a-stability.md) and also [L-stable](../../../../l-stability.md), since $R_{BE}(z)\to0$ for large $z$ in this half-plane. Here $z$ has the opposite sign from the alternative convention $z=h\lambda$ for $y'=\lambda y$.

**Predictor-corrector accuracy.** The printed two-stage construction is [Heun's method](../../../../heun-s-method.md), equivalently

$$
y_{n+1}=y_n+\frac h2\left[f(y_n,t_n)+f(y_n+hf(y_n,t_n),t_n+h)\right].
$$

Although the second stage resembles a [Backward Euler method](../../../../backward-euler-method.md) evaluation, it uses the predicted value, so the combined method is explicit. Expand that stage around the exact starting point, putting

$$
B=f_{tt}+2f f_{ty}+f^2f_{yy}.
$$

Then

$$
f(y+hf,t+h)=f+hA+\frac{h^2}2B+O(h^3),
$$

and the numerical step is $y+hf+\tfrac12h^2A+\tfrac14h^3B+O(h^4)$. Along the exact solution, $y'''=B+f_yA$, so comparison with the exact [Taylor expansion](../../../../taylor-expansion.md) gives

$$
\boxed{\delta_H=h^3\left(\frac{f_yA}6-\frac B{12}\right)+O(h^4)=O(h^3).}
$$

Thus the local defect improves by one power of $h$, giving second-order [global error](../../../../global-discretization-error.md) under the usual hypotheses. For the linear test equation the defect reduces to $-h^3\Lambda^3y/6+O(h^4)$.

**Predictor-corrector stability.** Applied to the test equation, the predictor is $y^{(1)}=(1-z)y_n$ and the second value is $y^{(2)}=(1-z+z^2)y_n$. Their average gives

$$
\boxed{R_H(z)=1-z+\frac{z^2}2,\qquad\text{stability region: }\left|1-z+\frac{z^2}2\right|\leq1.}
$$

For real positive $z$, $R_H(z)=\tfrac12[(z-1)^2+1]$, so strict decay holds exactly for $0<z<2$, the same real-axis step bound as [Forward Euler method](../../../../euler-method.md). For complex $z=x+iy$ the precise condition is

$$
\left[1-x+\frac{x^2-y^2}2\right]^2+y^2(x-1)^2\leq1.
$$

The region is bounded and does not contain the full right half-plane: for example $z=3$ gives $R_H=5/2$. It is therefore not [A-stable](../../../../a-stability.md). Its imaginary-axis values satisfy $|R_H(iy)|^2=1+y^4/4>1$ for $y\ne0$. Better accuracy has not inherited the unconditional stability of an actual implicit [Backward Euler method](../../../../backward-euler-method.md) step.

<a id="11/image-absolute-stability-regions-of-the-three-time-stepping-methods-in-the-exam"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1-time-stepping-stability.png)

**[Figure 2](#11/image-absolute-stability-regions-of-the-three-time-stepping-methods-in-the-exam). Absolute stability regions of the three time-stepping methods in the exam**. Shading shows amplification factor of modulus at most one, using z equal to step size times Lambda for y prime equal to minus Lambda y. Positive real z therefore represents physical decay; Heun improves accuracy but retains a bounded stability region.

## ↑ Ancestors (12)

1. [11](../11.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
