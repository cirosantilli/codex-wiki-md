# Huber score

↑ **Parent:** [Huber location estimator](huber-location-estimator.md)

The Huber score clips a residual at a fixed threshold:

$$
\psi_k(u)=\max(-k,\min(u,k)).
$$

For $k>0$, the [Huber score](huber-score.md) is the [derivative](derivative.md) of the [Huber loss](huber-loss.md):

$$
\psi_k(u)=\rho_k'(u)=\begin{cases}-k,&u<-k,\\u,&-k\leq u\leq k,\\k,&u>k.\end{cases}
$$

It is a continuous [odd function](odd-function.md) and a [monotone function](monotonic-function.md), with [Lipschitz continuity](lipschitz-continuity.md) and $|\psi_k(u)|\leq k$. In a [Huber location estimator](huber-location-estimator.md), its argument is the standardized difference $u=(x-\theta)/s$. Its [derivative](derivative.md) is $1$ inside the clipping interval and $0$ outside; that [derivative](derivative.md) is undefined at the two endpoints. The score itself remains continuous there. This estimating score need not be the [score function](informant-function.md) of a separately specified [statistical model](statistical-model-split.md), nor is it already a normalized [influence function](influence-function.md).

**Table of contents**

- [Optimal bounded influence function for normal location](optimal-bounded-influence-function-for-normal-location.md)

## ↑ Ancestors (7)

1. [Huber location estimator](huber-location-estimator.md)
2. [Robust statistics](robust-statistics-split.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Huber location estimator](huber-location-estimator.md)
- [Huber location response to one outlier](huber-location-response-to-one-outlier.md)
- [Huber loss](huber-loss.md)
- [Huber score](huber-score.md)
- [Influence function of a Huber location estimator](influence-function-of-a-huber-location-estimator.md)
- [Local influence versus replacement breakdown](local-influence-versus-replacement-breakdown.md)
- [Optimal bounded influence function for normal location](optimal-bounded-influence-function-for-normal-location.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-41/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-223/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-223/2/a/solution.md)
