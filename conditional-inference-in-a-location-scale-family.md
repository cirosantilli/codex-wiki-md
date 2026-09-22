# Conditional inference in a location-scale family

↑ **Parent:** [Location-scale family](location-scale-family.md)

For normalized residuals $A_i=(Y_i-\bar Y)/s$, [Fisherian conditional inference](fisherian-conditional-inference.md) uses the [conditional distribution](conditional-distribution.md) of $(\bar Y,s)$ given the observed $A=a$. For almost every attainable ancillary value, the joint conditional density of $\bar Y=m$ and $s=t>0$ is proportional to

$$
t^{n-2}\sigma^{-n}\prod_{i=1}^nf_0\!\left(\frac{m+ta_i-\mu}{\sigma}\right).
$$

The factor $t^{n-2}$ is the radial Jacobian on the $(n-1)$-dimensional centered residual space. After setting $u=(m-\mu)/\sigma$ and $v=t/\sigma$, the conditional density is proportional to $v^{n-2}\prod_i f_0(u+va_i)$, which is parameter-free. Conditioning on a continuous ancillary uses a [regular conditional distribution](regular-conditional-distribution.md), rather than division by the probability of a singleton ancillary value.

## ↑ Ancestors (6)

1. [Location-scale family](location-scale-family.md)
2. [Statistical model](statistical-model-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/1/solution.md)
