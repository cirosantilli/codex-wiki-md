<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [strongly continuous semigroup](../../../../../c0-semigroup.md) on the complex [Banach space](../../../../../banach-space-split.md) $E$ is a family $T_t\in\mathcal L(E)$ with $T_0=I$, $T_{s+t}=T_sT_t$ and $\|T_tf-f\|\to0$ as $t\downarrow0$ for every $f\in E$. Its [semigroup generator](../../../../../infinitesimal-generator-of-a-semigroup.md) is the [linear operator](../../../../../linear-operator.md)

$$
D(Z)=\left\{f\in E:\lim_{h\downarrow0}\frac{T_hf-f}{h}\text{ exists in }E\right\},\qquad
Zf=\lim_{h\downarrow0}\frac{T_hf-f}{h}.
$$

For $f\in D(Z)$, boundedness of $T_t$ and the semigroup identity give

$$
\frac{T_hT_tf-T_tf}{h}=T_t\frac{T_hf-f}{h}\longrightarrow T_tZf.
$$

Thus [semigroup commutation with its unbounded generator](../../../../../semigroup-commutation-with-its-unbounded-generator.md) means

$$
\boxed{T_tD(Z)\subseteq D(Z),\qquad ZT_tf=T_tZf\quad(f\in D(Z)).}
$$

There is no assertion that $Z$ is defined on every vector. The orbit is differentiable on this domain, with $\frac d{dt}T_tf=T_tZf$.

A [contraction semigroup](../../../../../contraction-semigroup.md) additionally satisfies $\|T_t\|\leq1$ for every $t\geq0$. For $\operatorname{Re}\lambda>0$, define the [Bochner integral](../../../../../bochner-integral.md)

$$
L_\lambda f=\int_0^\infty e^{-\lambda t}T_tf\,dt.
$$

[Strong continuity](../../../../../strong-continuity.md) gives a continuous integrand, and its [norm](../../../../../norm.md) is bounded by $e^{-t\operatorname{Re}\lambda}\|f\|$, so the integral exists and

$$
\|L_\lambda\|\leq\frac1{\operatorname{Re}\lambda}.
$$

Changing variables in $T_hL_\lambda f$ yields

$$
T_hL_\lambda f=e^{\lambda h}
\left(L_\lambda f-\int_0^h e^{-\lambda s}T_sf\,ds\right).
$$

After subtracting $L_\lambda f$ and dividing by $h$, the limit is $\lambda L_\lambda f-f$. Consequently

$$
\boxed{L_\lambda(E)\subseteq D(Z),\qquad
(\lambda I-Z)L_\lambda f=f.}
$$

For $f\in D(Z)$, integrate the [derivative](../../../../../derivative.md) of $e^{-\lambda t}T_tf$ over $[0,\infty)$. Its limit at infinity is zero by the contraction bound, and its value at zero is $f$. Therefore

$$
L_\lambda(\lambda I-Z)f
=-\int_0^\infty\frac d{dt}(e^{-\lambda t}T_tf)\,dt=f.
$$

Thus this is also the [Laplace-transform formula for a semigroup resolvent](../../../../../laplace-transform-formula-for-a-semigroup-resolvent.md), with $L_\lambda=(\lambda I-Z)^{-1}$.

To prove that $Z$ is a [closed operator](../../../../../closed-linear-operator.md), suppose $f_n\in D(Z)$, $f_n\to f$ and $Zf_n\to g$. Fix one $\lambda$ with positive real part. The identity just proved and boundedness of $L_\lambda$ give

$$
f=\lim_nL_\lambda(\lambda f_n-Zf_n)=L_\lambda(\lambda f-g).
$$

Its range lies in $D(Z)$, and applying $\lambda I-Z$ shows $Zf=g$. Thus the graph is closed. Linearity follows directly from linearity of the defining difference quotient, so **$Z$ is a closed [linear operator](../../../../../linear-operator.md)**.

The closedness conclusion also holds without the contraction assumption. For a general [strongly continuous semigroup](../../../../../c0-semigroup.md), the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) gives a uniform operator bound on each compact time interval. Integrating the generator-orbit identity gives $T_tf_n-f_n=\int_0^tT_sZf_n\,ds$. Under $f_n\to f$ and $Zf_n\to g$, pass to the limit to obtain $T_tf-f=\int_0^tT_sg\,ds$. Divide by $t$ and let $t\downarrow0$; [strong continuity](../../../../../strong-continuity.md) makes the right side converge to $g$, so $f\in D(Z)$ and $Zf=g$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
