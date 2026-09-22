<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

On the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), $g(y)=\lambda^2y$, so the [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md) becomes

$$
\left[1-(1-\alpha)z+\frac{1-3\alpha}{2}z^2\right]\xi^2
-(1+\alpha)\xi+\alpha=0,\qquad z=h\lambda.
$$

Both [roots of a polynomial](../../../../../../root-of-a-polynomial.md), including the parasitic one, must satisfy the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md).

For $\alpha=1/7$, multiply by seven and set $a=7-6z+2z^2$. The [polynomial](../../../../../../polynomial-split.md) is $a\xi^2-8\xi+1$. The [complex quadratic Schur criterion](../../../../../../complex-quadratic-schur-criterion.md) says that its [roots of a polynomial](../../../../../../root-of-a-polynomial.md) are strictly in the [unit disk](../../../../../../unit-disk.md) if

$$
|a|>1,\qquad |a|^2-1>8|a-1|.
$$

Here is a direct verification on the entire left half-plane. Put $z=-r+iy$, $r\geq0$, $t=y^2$, and $a_0=7+6r+2r^2$. Then

$$
q=|a|^2=a_0^2+8(r^2+3r+1)t+4t^2\geq49,
$$

and expansion of the squared inequality gives

$$
\begin{aligned}
(q-1)^2-64|a-1|^2={}&16t^4+64(r^2+3r+1)t^3\\
&+32(r^2+3r+3)(3r^2+9r+2)t^2\\
&+64r(r+3)(r^4+6r^3+17r^2+24r+11)t\\
&+16r(r+3)(r^2+3r+3)^2(r^2+3r+8).
\end{aligned}
$$

Every term is nonnegative, and at least one is positive unless $z=0$. Since $q-1>0$, taking square roots proves the strict [complex quadratic Schur criterion](../../../../../../complex-quadratic-schur-criterion.md) for $z\ne0$. At $z=0$, the [roots of a polynomial](../../../../../../root-of-a-polynomial.md) are the simple values $1$ and $1/7$. The leading coefficient cannot vanish because $|a|^2\geq49$. Thus **the method at $\alpha=1/7$ is [A-stable](../../../../../../a-stability.md)**. Its order three is compatible with the [Second Dahlquist barrier](../../../../../../second-dahlquist-barrier.md): that barrier concerns first-[derivative](../../../../../../derivative.md) [linear multistep methods](../../../../../../linear-multistep-method.md), whereas this method uses a second [derivative](../../../../../../derivative.md).

For $\alpha=1/2$, choose $z=-4$, strictly in the left half-plane. The [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md) reduces to

$$
-\xi^2-\frac32\xi+\frac12=0,\qquad
\xi=\frac{-3\pm\sqrt{17}}4.
$$

One [root of a polynomial](../../../../../../root-of-a-polynomial.md) has [modulus](../../../../../../modulus.md) $(3+\sqrt{17})/4>1$. Thus **the method at $\alpha=1/2$ is not [A-stable](../../../../../../a-stability.md)**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
