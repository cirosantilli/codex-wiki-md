<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use half-open intervals and set

$$
\varphi(x)=\mathbf1_{[0,1)}(x),\qquad\psi(x)=\mathbf1_{[0,1/2)}(x)-\mathbf1_{[1/2,1)}(x).
$$

The [Haar scaling functions](../../../../../haar-scaling-function.md) and [Haar wavelets](../../../../../haar-wavelet.md) are

$$
\boxed{\varphi_{j,k}(x)=2^{j/2}\varphi(2^jx-k),\qquad\psi_{l,k}(x)=2^{l/2}\psi(2^lx-k).}
$$

For fixed $j$, each scaling function has squared integral $2^j2^{-j}=1$, and different $k$ have disjoint supports, proving that this family is [orthonormal](../../../../../orthonormal-set.md). Each wavelet also has norm one and integral zero. At a fixed level, distinct wavelets have disjoint supports. At different levels, their dyadic supports are either disjoint or the finer support lies in a half on which the coarser wavelet is constant. The finer wavelet has integral zero, so their inner product vanishes. Finally, a wavelet with $l\ge0$ is supported inside a unit interval; it is orthogonal to its containing $\varphi_{0,k}$ because its integral is zero, and to all other unit scaling functions because their supports are disjoint. Thus **both the scaling family at each fixed level and the complete stated Haar family are orthonormal sets**.

The [Haar refinement identity](../../../../../haar-refinement-identity.md) is

$$
\varphi_{j,k}=\frac{\varphi_{j+1,2k}+\varphi_{j+1,2k+1}}{\sqrt2},\qquad
\psi_{j,k}=\frac{\varphi_{j+1,2k}-\varphi_{j+1,2k+1}}{\sqrt2}.
$$

It shows that the closed scaling spaces $V_j$ satisfy $V_{j+1}=V_j\oplus W_j$, where $W_j$ is the closed span of the level-$j$ wavelets. The union of the $V_j$ is dense in $L^2(\mathbb R)$: continuous compactly supported functions can be approximated in $L^2$ by their dyadic cell averages, and such continuous functions are dense in $L^2$. Hence the orthonormal Haar family is also a complete [orthonormal basis](../../../../../orthonormal-basis.md).

For a [locally integrable function](../../../../../locally-integrable-function.md), define the compact-support coefficient integrals

$$
a_{j,k}=\int_{\mathbb R}f(x)\varphi_{j,k}(x)\,dx,\qquad b_{l,k}=\int_{\mathbb R}f(x)\psi_{l,k}(x)\,dx.
$$

These exist without requiring $f\in L^2$. The two formulas for the [Haar approximation](../../../../../haar-projection.md) are

$$
\boxed{H_j(f)=\sum_{k\in\mathbb Z}a_{j,k}\varphi_{j,k}=\sum_{k\in\mathbb Z}a_{0,k}\varphi_{0,k}+\sum_{l=0}^{j-1}\sum_{k\in\mathbb Z}b_{l,k}\psi_{l,k}.}
$$

For $j=0$ the wavelet sum is empty. For every fixed $j$, these sums are locally finite, so they make sense pointwise and locally in $L^1$. The refinement identities and their orthogonal two-by-two coefficient transformation establish equality by induction, even for merely locally integrable $f$. If $f\in L^2$, this is also the [orthogonal projection](../../../../../orthogonal-projection.md) onto $V_j$.

In particular, for $\delta=2^{-j}$ and $x\in I_k=[k\delta,(k+1)\delta)$,

$$
H_j(f)(x)=\frac1\delta\int_{I_k}f(u)\,du.
$$

Now impose the symmetry and monotonicity conditions. The limit zero and decrease on $[0,\infty)$ imply $0\le f(x)\le f(0)$ for $x\ge0$. For $k\ge0$, the cell average and every value inside $I_k$ lie between $f((k+1)\delta)$ and $f(k\delta)$. Therefore

$$
\int_{I_k}|H_j(f)-f|\le\delta\big(f(k\delta)-f((k+1)\delta)\big).
$$

Summing over the positive half-line telescopes and gives a bound $\delta f(0)$. Reflection maps each dyadic cell to another dyadic cell up to endpoints. Since $f$ is even, its [Haar approximation](../../../../../haar-projection.md) is even almost everywhere as well, so the negative half-line has the same error. Consequently

$$
\boxed{\|H_j(f)-f\|_1\le2\delta f(0)=f(0)2^{1-j}.}
$$

The argument proves integrability of the difference, even if $f$ itself is not integrable on the whole line. It is the symmetric monotone case of the [Haar approximation error for a function of bounded variation](../../../../../haar-approximation-error-for-a-function-of-bounded-variation.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
