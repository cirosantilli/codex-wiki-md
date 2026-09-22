# Symmetric rational mixture sampler

↑ **Parent:** [Mixture distribution](mixture-distribution.md)

The displayed [mixture distribution](mixture-distribution.md) combines a [Standard Cauchy distribution](standard-cauchy-distribution.md) and a symmetric law whose magnitude has [cumulative distribution function](cumulative-distribution-function.md) $r^2/(1+r^2)$ for $r\geq0$. Use independent uniforms $U,V,H$: if $U\leq p$, return $\tan(\pi(V-1/2))$; otherwise return a fair independent sign times $\sqrt{V/(1-V)}$. The magnitude density is $2r/(1+r^2)^2$ and splitting its mass equally between signs gives $|x|/(1+x^2)^2$. An alternative [rejection sampling](rejection-sampling.md) proposal is standard Cauchy, with envelope constant $M=p+\pi(1-p)/2$, because $|x|/(1+x^2)\leq1/2$.

## ↑ Ancestors (7)

1. [Mixture distribution](mixture-distribution.md)
2. [Probability distribution](probability-distribution.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/3/ii/solution.md)
