# Flux of a vector field with an integrable tangential singularity

↑ **Parent:** [Divergence theorem](divergence-theorem.md)

Consider the [vector field](vector-field.md) $\mathbf F=(p(x),q(x),r(z))$ in the open unit [cube](cube.md), where $p$ and $r$ extend to continuously differentiable functions on $[0,1]$, and $q$ is continuous on $(0,1]$ with $\int_0^1|q(x)|\,dx<\infty$. Even if $q$ is unbounded as $x\downarrow0$, the [normal component](normal-component.md) on an $x$-face has the finite trace $\pm p(x)$. The two $y$-faces have finite [improper integral](improper-integral.md) fluxes $\pm\int_0^1q(x)\,dx$ and therefore cancel. The remaining face contributions give

$$
\boxed{\text{outward flux}=p(1)-p(0)+r(1)-r(0)}.
$$

To justify this use of the [divergence theorem](divergence-theorem.md), first apply it to $[\varepsilon,1]\times[0,1]^2$, on which the field is regular. Its [divergence](divergence.md) is $p'(x)+r'(z)$, independent of $q$. Its outward flux is $p(1)-p(\varepsilon)+(1-\varepsilon)[r(1)-r(0)]$. Taking $\varepsilon\downarrow0$ yields the displayed answer, and [absolute convergence](absolute-convergence.md) makes the two $y$-face limits finite separately. For example, $q(x)=1/[x(1+(\ln x)^2)]$ diverges at zero but

$$
\int_0^1q(x)\,dx=\left[\arctan(\ln x)\right]_{0^+}^{1}=\frac{\pi}{2}.
$$

This argument defines the normal traces and the face integrals explicitly; it does not assert that the whole [vector field](vector-field.md) has a finite value on the singular face.

## ↑ Ancestors (9)

1. [Divergence theorem](divergence-theorem.md)
2. [Vector calculus](vector-calculus.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/16/b/solution.md)
