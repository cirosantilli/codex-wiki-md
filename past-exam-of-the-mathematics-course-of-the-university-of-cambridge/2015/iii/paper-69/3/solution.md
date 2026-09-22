<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Define the [second modulus of smoothness](../../../../../second-modulus-of-smoothness.md) by $\omega_2(f,h)=\sup_{|u|\leq h}\|f(\cdot+u)-2f+f(\cdot-u)\|_\infty$. The [Jackson kernel](../../../../../jackson-kernel.md) is even, nonnegative and has integral one. Symmetrizing its [convolution](../../../../../convolution.md) therefore gives

$$
j_n(f,x)-f(x)=\frac12\int_{-\pi}^{\pi}[f(x+t)-2f(x)+f(x-t)]J_n(t)\,dt.
$$

We first establish the needed scaling rule. For the translation operator $T_u$, $(T_u^m-I)=(I+T_u+\cdots+T_u^{m-1})(T_u-I)$. Squaring gives $\|(T_u^m-I)^2f\|\leq m^2\|(T_u-I)^2f\|$. Central and forward second differences have the same norm. For every $|v|\leq|t|$, take $m=\lceil |v|/h\rceil$ and $u=v/m$. Taking the supremum over these $v$ proves

$$
\omega_2(f,|t|)\leq(1+|t|/h)^2\omega_2(f,h).
$$

The zero-step case is immediate.

For $|t|\leq\pi$, the inequalities $|\sin(nt/2)|\leq n|\sin(t/2)|$, $|\sin(nt/2)|\leq1$, and $|\sin(t/2)|\geq |t|/\pi$ imply

$$
0\leq J_n(t)\leq C\min\left(n,\frac1{n^3t^4}\right).
$$

Use the first estimate on $|t|\leq1/n$ and the second outside it. Then

$$
\int_{-\pi}^{\pi}(1+n|t|)^2J_n(t)\,dt
\leq C\left[n\int_0^{1/n}1\,dt+\frac1n\int_{1/n}^{\pi}\frac{dt}{t^2}\right]\leq C'.
$$

All constants are independent of $n$ and $f$. Combining these estimates proves **the [Jackson operator estimate](../../../../../jackson-operator-estimate.md)**

$$
\boxed{\|j_n(f)-f\|_\infty\leq C\,\omega_2(f,1/n).}
$$

For $f\in C^2(\mathbb T)$, two applications of the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) give the [second-difference integral formula](../../../../../second-difference-integral-formula.md)

$$
f(x+h)-2f(x)+f(x-h)=\int_{-h}^{h}(h-|u|)f''(x+u)\,du
$$

for $h\geq0$. Its absolute value is at most $h^2\|f''\|_\infty$, so $\omega_2(f,h)\leq h^2\|f''\|_\infty$.

Finally, $J_m$ is a [trigonometric polynomial](../../../../../trigonometric-polynomial.md) of degree $2(m-1)$: its sine ratio squared is a Fejér [polynomial](../../../../../polynomial-split.md) of degree $m-1$, and squaring doubles that degree. Thus $j_m(f)$ has degree at most $2(m-1)$. To bound degree-$n$ best approximation, choose $m=\lfloor n/2\rfloor+1$, rather than using $j_n$ directly. Since $m\geq n/2$ for $n\geq1$, **the smooth-function approximation rate is**

$$
\boxed{E_n(f)\leq\|j_m(f)-f\|_\infty\leq\frac{C_1}{n^2}\|f''\|_\infty.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
