<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Identify a line with its unique parameter pair in $E=(0,\infty)\times[0,2\pi)$, using

$$
L(p,\theta)=\{z\in\mathbb R^2:z\cdot n_\theta=p\},\qquad n_\theta=(\cos\theta,\sin\theta).
$$

A [Poisson line process](../../../../../poisson-line-process.md) means a [Poisson point process](../../../../../poisson-point-process.md) on the Borel parameter space $E$: for each [measurable](../../../../../measurability.md) $B$ of finite [mean](../../../../../expected-value.md) [measure](../../../../../measure.md), the number of its parameter points is [Poisson](../../../../../poisson-distribution.md) with [mean](../../../../../expected-value.md) $\mu(B)$, and counts in finitely many disjoint sets are [independent](../../../../../independent-random-variables.md). Infinite-measure sets are handled by a [countable](../../../../../countable-set.md) finite-measure exhaustion. Here $\mu(dp,d\theta)=dp\,d\theta$ is sigma-finite and nonatomic, so there are countably many distinct lines [almost surely](../../../../../almost-sure-convergence.md). It is not an assertion that line counts are [Poisson](../../../../../poisson-distribution.md) with respect to planar area.

Fix $r>0$ and let $D_r=\{z:|z|<r\}$. Exactly the lines with $0<p<r$ hit this disk, apart from the zero-probability tangent case. Thus the count of disk-hitting lines is

$$
M_r\sim\operatorname{Poisson}(2\pi r).
$$

Every intersection in $D_r$ uses two of these lines. Writing $N_r=\#(\Phi\cap D_r)$, we have

$$
\{N_r\geq1\}\subseteq\{M_r\geq2\},\qquad N_r\leq\binom{M_r}{2}.
$$

This also proves local finiteness of the intersection [point process](../../../../../point-process.md). Initially it gives a non-strict bound $\mathbb P(N_r\geq1)\leq1-(1+2\pi r)e^{-2\pi r}$.

To establish strictness, choose the two parameter boxes

$$
B_1=(r/8,r/4)\times(0,1/16),\qquad B_2=(r/2,5r/8)\times(0,1/16).
$$

Each has positive [measure](../../../../../measure.md), and both lie among the disk-hitting lines. If one line from each box intersected at $z\in D_r$, then

$$
|p_2-p_1|=|z\cdot(n_{\theta_2}-n_{\theta_1})|\leq r|n_{\theta_2}-n_{\theta_1}|\leq r|\theta_2-\theta_1|<r/16.
$$

But their distance parameters differ by more than $r/4$, a contradiction. The event of exactly one line in each box and no other disk-hitting lines has [probability](../../../../../probability.md)

$$
\delta_r=e^{-2\pi r}\mu(B_1)\mu(B_2)=e^{-2\pi r}\left(\frac{r}{128}\right)^2>0.
$$

On this event $M_r=2$ but $N_r=0$. Therefore

$$
\boxed{\mathbb P(N_r\geq1)\leq1-(1+2\pi r)e^{-2\pi r}-\delta_r<1-(1+2\pi r)e^{-2\pi r}.}
$$

The following original diagram illustrates why two disk-hitting lines need not produce an intersection inside the disk.

<a id="3/image-two-lines-meeting-a-disk-can-have-their-intersection-outside-it"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-31-chords.png)

**[Figure 1](#3/image-two-lines-meeting-a-disk-can-have-their-intersection-outside-it). Two lines meeting a disk can have their intersection outside it**.

To decide whether $\Phi$ is [Poisson](../../../../../poisson-distribution.md), compute its [intensity measure](../../../../../intensity-measure-of-a-point-process.md) and compare its void [probability](../../../../../probability.md). Use the equivalent signed line coordinates $L(t,\theta)$ with $t\in\mathbb R$ and $0\leq\theta<\pi$. If $t>0$ this is the original pair $(t,\theta)$; if $t<0$ it is $(-t,\theta+\pi)$. The [measure](../../../../../measure.md) is $dt\,d\theta$, with no extra factor of two. Translation by $a$ sends $t$ to $t+a\cdot n_\theta$, preserving this [measure](../../../../../measure.md). Thus both the line and intersection processes are stationary.

[Almost surely](../../../../../almost-sure-convergence.md) no two lines are parallel and no three are concurrent. In each finite-intensity parameter region, conditional line parameters have continuous joint densities. Parallel pairs and concurrent triples satisfy lower-dimensional equations and have [probability](../../../../../probability.md) zero; a [countable](../../../../../countable-set.md) exhaustion proves the assertion for all lines. Hence different unordered pairs have distinct intersections [almost surely](../../../../../almost-sure-convergence.md). For a bounded [Borel set](../../../../../borel-set.md) $A$, the second [Poisson factorial moment measure](../../../../../poisson-factorial-moment-measure.md) identity gives

$$
\mathbb EN(A)=\frac12\int_0^\pi\int_0^\pi\int_{\mathbb R}\int_{\mathbb R}\mathbf1_{\{L(t,\theta)\cap L(s,\phi)\in A\}}\,dt\,ds\,d\theta\,d\phi.
$$

For nonparallel normals, their intersection $z$ satisfies $t=z\cdot n_\theta$, $s=z\cdot n_\phi$. The absolute [Jacobian determinant](../../../../../jacobian-determinant.md) of this transformation is $|\sin(\phi-\theta)|$. Consequently

$$
\begin{aligned}
\mathbb EN(A)&=\frac{|A|}{2}\int_0^\pi\int_0^\pi|\sin(\phi-\theta)|\,d\phi\,d\theta\\
&=\pi|A|,
\end{aligned}
$$

since the inner [integral](../../../../../integral.md) is $2$ for every $\theta$. In particular **$\mathbb EN_r=\pi^2r^2$**.

If $\Phi$ were a [Poisson point process](../../../../../poisson-point-process.md), the count $N_r$ would therefore be [Poisson](../../../../../poisson-distribution.md) with that [mean](../../../../../expected-value.md), giving $\mathbb P(N_r=0)=e^{-\pi^2r^2}$. But the earlier necessary-two-lines argument gives

$$
\mathbb P(N_r=0)\geq(1+2\pi r)e^{-2\pi r}.
$$

At $r=2/\pi$ this lower bound is $5e^{-4}$, whereas the supposed [Poisson](../../../../../poisson-distribution.md) void [probability](../../../../../probability.md) is $e^{-4}$. This contradiction proves **$\Phi$ is not a [Poisson point process](../../../../../poisson-point-process.md)**. Its points share parent lines, and the explicit void/[mean](../../../../../expected-value.md) comparison demonstrates the resulting dependence rather than merely asserting it.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
