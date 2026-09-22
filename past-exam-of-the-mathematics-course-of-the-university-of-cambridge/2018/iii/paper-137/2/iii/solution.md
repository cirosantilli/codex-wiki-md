<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The original PDF has the summation condition $\gcd(n,N)=1$; the TeX's $\gcd(n,n)=1$ is a transcription error. There is also an actual missing hypothesis in the PDF's coefficient formula: that simplified formula requires a [primitive Dirichlet character](../../../../../../primitive-dirichlet-character.md). We first derive a formula valid for every character, and then show both the primitive specialization and a counterexample to the unrestricted version.

For $k>2$, the [character-twisted Eisenstein series](../../../../../../character-twisted-eisenstein-series.md) converges absolutely and locally uniformly on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). On a compact subset, $|mz+n|$ is bounded below by a positive constant times $(m^2+n^2)^{1/2}$, and the corresponding two-dimensional lattice sum converges. Changing $n$ to $n+mN$ proves

$$
\boxed{G_k(\chi,z+N)=G_k(\chi,z).}
$$

The condition $\chi(-1)=(-1)^k$ makes the terms for $(m,n)$ and $(-m,-n)$ equal. The terms with $m=0$ contribute $2L(\chi,k)$, and all other terms are twice the sum over $m\geq1$.

For $\operatorname{Im}w>0$, the cotangent identity and

$$
\pi\cot\pi w=-\pi i-2\pi i\sum_{r\geq1}e^{2\pi irw}
$$

give, after $k-1$ differentiations,

$$
\sum_{t\in\mathbb Z}(w+t)^{-k}
=A_k\sum_{r\geq1}r^{k-1}e^{2\pi irw},
\qquad A_k=\frac{(-2\pi i)^k}{(k-1)!}.
$$

Differentiation is justified by locally uniform convergence. This is the [cotangent partial-fraction Fourier kernel](../../../../../../cotangent-partial-fraction-fourier-kernel.md).

Write $n=a+Nt$, with $a$ running through the unit classes modulo $N$, and define the finite Fourier transform

$$
S_\chi(r)=\sum_{a\bmod N\atop(a,N)=1}\chi(a)e^{2\pi ira/N},
\qquad g(\chi)=S_\chi(1).
$$

Here $g(\chi)$ is the [Gauss sum of a Dirichlet character](../../../../../../gauss-sum-of-a-dirichlet-character.md).  
Applying the kernel with $w=(mz+a)/N$ yields

$$
G_k(\chi,z)=2L(\chi,k)+\frac{2A_k}{N^k}
\sum_{m,r\geq1}r^{k-1}S_\chi(r)e^{2\pi imrz/N}.
$$

The double series converges absolutely: $|S_\chi(r)|\leq\varphi(N)$ and the exponential decay controls $\sum_{m,r}r^{k-1}e^{-2\pi mr\operatorname{Im}z/N}$. Grouping the terms with $mr=n$ proves the general [Fourier expansion of a character-twisted Eisenstein series](../../../../../../fourier-expansion-of-a-character-twisted-eisenstein-series.md):

$$
\boxed{c_0=2L(\chi,k),\qquad
c_n=\frac{2A_k}{N^k}\sum_{r\mid n}r^{k-1}S_\chi(r)\quad(n\geq1).}
$$

If $r$ is a unit modulo $N$, substitution $a\mapsto r^{-1}a$ gives $S_\chi(r)=\chi(r)^{-1}g(\chi)$. Suppose now that $\chi$ is primitive and $r$ is a nonunit. Choose a prime $p\mid\gcd(r,N)$. Reduction of units modulo $N$ onto units modulo $N/p$ is surjective. Primitivity means that $\chi$ is nontrivial on its kernel, so there is a unit $u\equiv1\pmod{N/p}$ with $\chi(u)\ne1$. Since $ru\equiv r\pmod N$, substitution by $u$ forces $S_\chi(r)=\chi(u)^{-1}S_\chi(r)$ and thus $S_\chi(r)=0$. This proves the [finite Fourier transform of a primitive Dirichlet character](../../../../../../finite-fourier-transform-of-a-primitive-dirichlet-character.md) identity, and consequently

$$
\boxed{c_n=\frac{2(-2\pi i)^k}{(k-1)!N^k}g(\chi)
\sum_{r\mid n}\overline\chi(r)r^{k-1}
\quad\text{when }\chi\text{ is primitive}.}
$$

The inverse-character notation in the question is understood to mean $\overline\chi(r)$, extended by zero on nonunits; literal inversion of $\chi(r)=0$ would be undefined.

For a counterexample without primitivity, take $N=2$, the principal character, and $k=4$. Then $S_\chi(r)=(-1)^r$, so $g(\chi)=-1$ but $S_\chi(2)=1$. At $n=2$, the general formula gives $c_2=7A_4/8$, whereas the printed simplified formula, interpreted as zero on nonunits, gives $-A_4/8$. Hence **the printed coefficient formula is false for arbitrary imprimitive characters**; the general boxed formula above supplies the correction.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
