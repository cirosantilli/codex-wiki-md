<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At a locked state choose the rotating frame with $\theta_i'=0$. For small phase differences, [Taylor expansion](../../../../../taylor-expansion.md) gives $h(\theta_j-\theta_i)-h(0)=h'(0)(\theta_j-\theta_i)+O(|\theta_j-\theta_i|^2)$. Let the [graph Laplacian](../../../../../laplacian-matrix.md) have $L_{ii}=\sum_jd_{ij}$ and $L_{ij}=-d_{ij}$ for $i\ne j$. The leading locked equations are

$$
0=\xi-\Omega_1\mathbf1-h'(0)L\theta.
$$

If coupling is balanced, $\sum_jd_{ij}=\sum_jd_{ji}$ for every $i$, so $\mathbf1^{\mathsf T}L=0$. Summing over cells cancels all linear coupling terms and gives

$$
\boxed{\Omega_1=\frac1N\sum_{i=1}^N\xi_i+O(\max_{ij}|\theta_j-\theta_i|^2).}
$$

In particular symmetric reciprocal gap-junction conductances satisfy this condition. To leading order the collective physical [frequency](../../../../../frequency.md) is $1+\epsilon N^{-1}\sum_i\xi_i$.

**The arithmetic-mean conclusion requires this extra balance assumption.** The printed condition $d_{ii}=0$ alone is insufficient. For a connected directed coupling network let $\pi^{\mathsf T}L=0$, normalized by $\pi^{\mathsf T}\mathbf1=1$. The valid [weighted collective oscillator frequency](../../../../../weighted-collective-oscillator-frequency.md) result is

$$
\boxed{\Omega_1=\sum_i\pi_i\xi_i+O(\max|\theta_j-\theta_i|^2).}
$$

For two cells with $d_{12}=p>0$, $d_{21}=q>0$, one has $\pi=(q,p)/(p+q)$ and $\Omega_1=(q\xi_1+p\xi_2)/(p+q)$ at linear order. For example $p=1,q=2,\xi_1=0,\xi_2=\delta$ gives $\Omega_1=\delta/3$, rather than $\delta/2$, while the locked phase difference is $O(\delta)$ when $h'(0)\ne0$. This supplies a counterexample with arbitrarily small phase differences. It also identifies exactly why reciprocal coupling recovers the requested mean: the left [null space](../../../../../kernel-of-a-linear-map-split.md) is then spanned by the uniform [vector](../../../../../vector.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
