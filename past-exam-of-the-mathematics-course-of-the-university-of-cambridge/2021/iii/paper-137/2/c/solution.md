<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $g=f|_k[\alpha_N]$. Termwise [Mellin transform](../../../../../../mellin-transform.md) in the initial half-plane gives

$$
I(f,s):=\int_0^\infty f(iy)y^{s-1}\,dy
=(2\pi)^{-s}\Gamma(s)L(f,s),
$$

so $\Lambda(f,s)=N^{s/2}I(f,s)$.

From the definition of the slash action,

$$
g(iy)=N^{-1}(iy)^{-k}f\left(\frac{i}{Ny}\right),
$$

or equivalently

$$
f\left(\frac{i}{Ny}\right)=Ni^ky^kg(iy).
$$

Substituting $y=1/(Nt)$ in the Mellin integral therefore gives

$$
I(f,s)=i^kN^{1-s}I(g,k-s).
$$

Multiplying by $N^{s/2}$ and recognizing the completed function on the right yields

$$
\boxed{\Lambda(f,s)=i^kN^{1-k/2}
\Lambda(f|_k[\alpha_N],k-s)}.
$$

At infinity, both $f(iy)$ and $g(iy)$ decay exponentially because they are [cusp forms](../../../../../../cusp-form.md). The transformation just used converts the behavior of $f(iy)$ near zero into the exponential decay of $g(i/(Ny))$ at infinity. Consequently $I(f,s)$ converges absolutely for every $s\in\mathbb C$ after splitting the integral at one and applying that substitution to the part near zero. It is locally uniformly convergent in $s$, hence entire, and agrees with the original Dirichlet series in its initial domain. This proves the analytic continuation and the stated functional equation, as summarized by the [Mellin transform of a cusp-form L-function](../../../../../../mellin-transform-of-a-cusp-form-l-function.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
