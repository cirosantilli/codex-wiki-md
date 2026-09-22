# Effective-bandwidth admission region with a voice delay gate

↑ **Parent:** [Priority queue with a shared buffer](priority-queue-with-a-shared-buffer.md)

Assume [independent](independent-random-variables.md) stationary [Compound Poisson process](compound-poisson-process.md) inputs, preemptive-resume priority for voice, [first come first served](first-come-first-served.md) within each class, capacity $C$, a shared buffer of $B$ units of work, packet sizes bounded by $s_{\max}<B$, and voice delay gate $D>0$. Write $B_0=B-s_{\max}$ and $K=CD$. For $n_v,n_d$ flows with per-flow [effective bandwidths](effective-bandwidth.md) $a_v,a_d$, the [continuous-time exponential workload bound](continuous-time-exponential-workload-bound.md) gives

$$
p_d\leq e^{-\theta_TB_0},\qquad
p_v\leq e^{-\theta_TB_0}+e^{-\theta_VK},
$$

provided $n_va_v(\theta_T)+n_da_d(\theta_T)\leq C$ and $n_va_v(\theta_V)\leq C$. To prove this, couple with the unthinned infinite-buffer aggregate and voice queues driven by the same offered packets. Dropping work reduces both the total and voice workloads under this [service discipline](service-discipline.md). A buffer-fit failure implies total workload greater than $B_0$, and a voice-gate failure implies voice workload at least $K$. Apply the two bounds and a union bound; [Poisson arrivals see time averages](poisson-arrivals-see-time-averages.md) converts stationary prearrival probabilities to offered-packet loss fractions. For target losses $\ell_d,\ell_v$, choose $0<\eta_B<\min(\ell_d,\ell_v)$ and $\eta_V=\ell_v-\eta_B$, then set

$$
\theta_T=B_0^{-1}\log(1/\eta_B),\qquad
\theta_V=K^{-1}\log(1/\eta_V).
$$

The two [effective bandwidth](effective-bandwidth.md) constraints, together with strict aggregate mean-load stability, define a sufficient integer admission region. Voice loss includes the shared-buffer term, even though data packets have lower service priority.

## ↑ Ancestors (8)

1. [Priority queue with a shared buffer](priority-queue-with-a-shared-buffer.md)
2. [Multiclass single-server queue](multiclass-single-server-queue.md)
3. [Queueing theory](queueing-theory-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/4/b/solution.md)
