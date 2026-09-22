<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the same normalized [spherical cap](../../../../../../spherical-cap.md) area $q$, constant $c_n$ and function $F=\sin^n\rho-q$ as above. Put $\rho_0=\arcsin(1/\sqrt n)$. The supplied ratio estimate gives

$$
c_n<\frac1n\sqrt{\frac{n+1}{2\pi}}\leq\frac{\sqrt{n-1}}n=\sin\rho_0\cos\rho_0.
$$

The middle inequality holds for every $n\geq2$, since $n+1\leq2\pi(n-1)$. Applying the upper projection bound for the [spherical cap](../../../../../../spherical-cap.md) at $\rho_0$ yields

$$
q(\rho_0)\leq c_n\frac{\sin^{n-1}\rho_0}{\cos\rho_0}\leq\sin^n\rho_0,
$$

so $F(\rho_0)\geq0$.

Recall

$$
F'(\rho)=\sin^{n-2}\rho\bigl(n\sin\rho\cos\rho-(n-1)c_n\bigr).
$$

At $\rho_0$ the expression in parentheses is positive, because $n\sin\rho_0\cos\rho_0=\sqrt{n-1}$ and $(n-1)c_n<\sqrt{n-1}$. It increases up to $\pi/4$ and then decreases strictly to a negative value at $\pi/2$. Hence it crosses zero exactly once on $[\rho_0,\pi/2]$, from positive to negative. The minimum of $F$ is again an endpoint value; $F(\rho_0)\geq0$ and $F(\pi/2)=1/2$. **This proves the stronger range of the [spherical cap area upper bound](../../../../../../spherical-cap-area-upper-bound.md):**

$$
\boxed{\operatorname{Vol}_{n-1}(D_\rho)\leq\sin^n\rho\,s_{n-1}\qquad(\sin\rho\geq n^{-1/2}).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
