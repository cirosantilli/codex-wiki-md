<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose a nonconstant element $t$ of the [function field](../../../../../function-field-of-an-algebraic-variety.md) $k(C)$. By Question 1 it gives a [finite morphism](../../../../../finite-morphism.md) $\pi:C\to\mathbb P^1$. The inverse images $U_0=\pi^{-1}(\mathbb A^1_t)$ and $U_1=\pi^{-1}(\mathbb A^1_{t^{-1}})$ are affine, because the inverse image of an affine under a [finite morphism](../../../../../finite-morphism.md) is the spectrum of a finite algebra over its coordinate ring. They cover $C$. This proves the [two-affine cover of a smooth projective curve](../../../../../two-affine-cover-of-a-smooth-projective-curve.md) assertion.

Their intersection is affine by Question 2. Thus the [Čech cochain complex](../../../../../cech-cochain-complex.md) for any [coherent sheaf](../../../../../coherent-sheaf.md) $\mathcal F$ has just two nonzero terms,

$$
\Gamma(U_0,\mathcal F)\oplus\Gamma(U_1,\mathcal F)
\longrightarrow\Gamma(U_0\cap U_1,\mathcal F).
$$

It follows that

$$
\boxed{H^i(C,\mathcal F)=0\quad(i\ge2).}
$$

On the [projective line](../../../../../projective-line.md), put $t=X_1/X_0$ on the first chart. The [twisting sheaf on projective space](../../../../../twisting-sheaf-on-projective-space.md) $\mathcal O(n)$ has frames $e_0=X_0^n$ and $e_1=X_1^n$, with $e_1=t^ne_0$ on the intersection; these are frame symbols also for negative $n$. In the $e_0$ frame the differential of the [Čech cochain complex](../../../../../cech-cochain-complex.md) is

$$
 k[t]\oplus k[t^{-1}]\longrightarrow k[t,t^{-1}],\qquad
 (a,b)\longmapsto t^nb-a.
$$

A [global section](../../../../../global-section.md) is therefore a Laurent polynomial in both $k[t]$ and $t^nk[t^{-1}]$. Its monomials have exponents $0\le j\le n$. For $n\ge0$ the sections have basis $e_0,te_0,\ldots,t^ne_0$; for $n<0$ there are none. The first [sheaf cohomology](../../../../../sheaf-cohomology.md) is

$$
H^1(\mathbb P^1,\mathcal O(n))=
\frac{k[t,t^{-1}]}{k[t]+t^nk[t^{-1}]}.
$$

Its basis consists of the monomials $t^je_0$ with $n<j<0$. These are precisely the exponents missed by the two chart spaces. Thus for every integer $n$,

$$
\boxed{h^0(\mathbb P^1,\mathcal O(n))=\max(n+1,0),\qquad
h^1(\mathbb P^1,\mathcal O(n))=\max(-n-1,0).}
$$

Both groups vanish at $n=-1$; all higher groups vanish for every $n$. This is also an explicit calculation of the [Čech cohomology of twists on the projective line](../../../../../cech-cohomology-of-twists-on-the-projective-line.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
