<h1 id="o5/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The final cell is a grouped tail. Thus use twelve probabilities

$$
p_i(\theta)=e^{-\theta}\frac{\theta^i}{i!}\quad(0\leq i\leq10),\qquad
p_{11}(\theta)=\mathbb P_\theta(X\geq11)=1-\sum_{i=0}^{10}p_i(\theta).
$$

Maximize the grouped [Grouped Poisson likelihood](../../../../../grouped-poisson-likelihood.md)

$$
\ell(\theta)=\sum_{i=0}^{10}n_i\log p_i(\theta)+n_{11}\log p_{11}(\theta),
$$

then take $\boxed{\widehat\pi_i=p_i(\widehat\theta)}$ for all twelve cells. For example, the interior likelihood equation is

$$
\sum_{i=0}^{10}n_i\left(\frac i\theta-1\right)
+n_{11}\frac{p_{10}(\theta)}{p_{11}(\theta)}=0,
$$

because $p_{11}'(\theta)=p_{10}(\theta)$. It can be solved numerically, with no numerical work required here.

It would be incorrect to treat the last six observations as exactly eleven. If the underlying ungrouped particle counts were available, their sample mean would be the usual Poisson maximum likelihood estimate. For the data as supplied, the grouped likelihood handles the unknown tail counts directly.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [O5](../../../o5.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
