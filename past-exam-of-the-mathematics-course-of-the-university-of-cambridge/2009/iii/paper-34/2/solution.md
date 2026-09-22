<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $Q_n(\theta)=n^{-1}\sum_{i=1}^n\log f(Y_i;\theta)$ and $Q(\theta)=\mathbb E_{\theta_0}\log f(Y_1;\theta)$. The integrable absolute-log envelope makes these expectations finite. Compactness and continuity of the likelihood ensure that a maximum exists, and maximizing it is equivalent almost surely to maximizing $Q_n$.

First identify the unique maximizer of $Q$. Let $r(y)=f(y;\theta)/f(y;\theta_0)$ on the support of the true density. Since $\log r\leq r-1$,

$$
Q(\theta)-Q(\theta_0)=\mathbb E_{\theta_0}\log r(Y_1)\leq\mathbb E_{\theta_0}r(Y_1)-1=\int_{\{f(y;\theta_0)>0\}}f(y;\theta)dy-1\leq0.
$$

Equality requires $r=1$ almost surely under the true distribution and no mass outside its support, so the two probability distributions coincide. By [identifiability](../../../../../identifiability.md), this happens only for $\theta=\theta_0$. Equivalently $Q(\theta_0)-Q(\theta)$ is the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) from the true distribution to the candidate.

Fix $\varepsilon>0$ and let $K_\varepsilon=\{\theta\in\Theta:\|\theta-\theta_0\|\geq\varepsilon\}$. If this set is empty there is nothing to prove. Otherwise it is compact, so continuity and the strict maximum imply

$$
\delta_\varepsilon=Q(\theta_0)-\max_{\theta\in K_\varepsilon}Q(\theta)>0.
$$

On the event $\sup_{\Theta}|Q_n-Q|<\delta_\varepsilon/3$, every point of $K_\varepsilon$ has $Q_n(\theta)<Q(\theta_0)-2\delta_\varepsilon/3$, whereas $Q_n(\theta_0)>Q(\theta_0)-\delta_\varepsilon/3$. Hence no maximizer can belong to $K_\varepsilon$. The supplied [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md) therefore proves [compact-parameter consistency of maximum likelihood](../../../../../compact-parameter-consistency-of-maximum-likelihood.md):

$$
\mathbb P_{\theta_0}(\|\widehat\theta_n-\theta_0\|\geq\varepsilon)\leq\mathbb P_{\theta_0}\!\left(\sup_\Theta|Q_n-Q|\geq\frac{\delta_\varepsilon}{3}\right)\longrightarrow0,
\qquad\boxed{\widehat\theta_n\xrightarrow{p}\theta_0.}
$$

Under the usual regularity conditions, with nonsingular one-observation [Fisher information matrix](../../../../../fisher-information-matrix.md) $I(\theta_0)$, the [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) is

$$
\boxed{\sqrt n(\widehat\theta_n-\theta_0)\xrightarrow{d}N_d\bigl(0,I(\theta_0)^{-1}\bigr),}
$$

where $I(\theta_0)=\mathbb E_{\theta_0}[S_{\theta_0}(Y_1)S_{\theta_0}(Y_1)^T]$ and $S_\theta=\nabla_\theta\log f(\cdot;\theta)$ is the [score function](../../../../../informant-function.md).

For the uniform model, let $M_n=\max_iY_i$. For a sample in its support, the likelihood is $\theta^{-n}\mathbf1_{\{\theta\geq M_n\}}$, decreasing on its nonzero region. Thus the [uniform endpoint maximum-likelihood estimator](../../../../../uniform-endpoint-maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\theta_n=M_n.}
$$

The all-zero sample is a probability-zero exception and may be assigned an arbitrary positive estimate. Independence gives $\mathbb P_\theta(M_n\leq y)=(y/\theta)^n$ on $[0,\theta]$. For $0<\varepsilon<\theta$,

$$
\mathbb P_\theta(|M_n-\theta|>\varepsilon)=\left(1-\frac\varepsilon\theta\right)^n\longrightarrow0;
$$

for $\varepsilon\geq\theta$ this probability is zero. This proves consistency directly.

Let $T_n=n(\theta-M_n)/\theta$. Its exact [cumulative distribution function](../../../../../cumulative-distribution-function.md) is

$$
\mathbb P_\theta(T_n\leq t)=\begin{cases}0&t<0,\\1-(1-t/n)^n&0\leq t\leq n,\\1&t>n.\end{cases}
$$

For fixed $t\geq0$, this converges to $1-e^{-t}$, so $T_n\xrightarrow{d}\operatorname{Exp}(1)$. In particular the errors are of order $1/n$. Explicitly, for every fixed $\eta>0$ and sufficiently large $n$,

$$
\mathbb P_\theta\bigl(\sqrt n|M_n-\theta|>\eta\bigr)=\left(1-\frac\eta{\theta\sqrt n}\right)^n\leq e^{-\eta\sqrt n/\theta}\longrightarrow0.
$$

Consequently

$$
\boxed{\frac{n(\theta-\widehat\theta_n)}\theta\xrightarrow{d}\operatorname{Exp}(1),\qquad\widehat\theta_n=\theta+o_p(n^{-1/2}).}
$$

One violated regularity condition is parameter-independent support: the density is supported on $[0,\theta]$. Differentiation under the density integral is not valid in the usual regular-model form. Indeed the interior score equals $-1/\theta$, whose expectation is not zero; the changing endpoint contributes the omitted boundary term. Thus the uniform model is handled by its exact maximum distribution, rather than by the regular asymptotic normality theorem.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
