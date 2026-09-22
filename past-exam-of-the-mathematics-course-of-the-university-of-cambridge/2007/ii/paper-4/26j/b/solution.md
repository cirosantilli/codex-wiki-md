<h1 id="26j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\rho=\lambda/\mu$. The proposed stationary probability is the product

$$
\boxed{\pi(c,r,b)=e^{-3\rho}\frac{\rho^c}{c!}\frac{\rho^r}{r!}\frac{\rho^b}{b!}.}
$$

It sums to one. Divide the balance equation at $(c,r,b)$ by this probability. Incoming immigration from $(c-1,r,b)$ contributes $\lambda c/\rho=\mu c$; incoming first metamorphosis from $(c+1,r-1,b)$ contributes $\mu(c+1)r/(c+1)=\mu r$; the next metamorphosis contributes $\mu b$; incoming death from $(c,r,b+1)$ contributes $\mu(b+1)\rho/(b+1)=\lambda$. Their sum is precisely the outgoing rate. Missing boundary terms contribute zero, as the corresponding coordinate is zero. Thus $\pi Q=0$.

For $\lambda,\mu>0$ the chain is irreducible: with positive probability all current insects progress and die before another arrival, and from the empty state specified finite arrivals and stage transitions can reach any state. It is nonexplosive, since only finitely many Poisson arrivals occur in a finite interval and each individual makes at most three stage/death transitions. The existence of this normalized stationary law for an irreducible nonexplosive chain implies positive recurrence and uniqueness of the stationary probability law. “Only solution” here means only probability solution; the homogeneous equation itself also admits zero and scalar multiples.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
