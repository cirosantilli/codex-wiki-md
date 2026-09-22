# Average memory access time

↑ **Parent:** [Memory access latency](memory-access-latency.md)

The [arithmetic mean](arithmetic-mean.md) of [memory access latencies](memory-access-latency.md). Suppose each read completes before the next begins, every [cache hit](cache-hit.md) costs $t_h$, and every [cache miss](cache-miss.md) costs $t_h+p$, with the same additional [cache miss penalty](cache-miss-penalty.md) $p$. If $h$ is [cache hit rate](cache-hit-rate.md) and $m=1-h$ is [cache miss rate](cache-miss-rate.md), the [weighted arithmetic mean](weighted-arithmetic-mean.md) is

$$
\operatorname{AMAT}=h\,t_h+m(t_h+p)=t_h+mp.
$$

The common lookup cost is paid on both outcomes. This additive assumption matches the simple model in [Beyond Physical Memory: Policies](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md) (§22.1, equation 22.1, pp. 1–2), where main [computer memory](computer-memory.md) acts as a [memory cache](cache-computing.md) for [memory pages](memory-page.md) backed by disk; here the same accounting is applied to a toy data [memory cache](cache-computing.md).

Assign synthetic values $t_h=2\,\mathrm{ns}$ and $p=30\,\mathrm{ns}$. The twelve-read, two-slot [fully associative cache](fully-associative-cache.md) example has five [cache hits](cache-hit.md) and seven [cache misses](cache-miss.md), giving

$$
\operatorname{AMAT}=2+\frac{7}{12}\,30=19.5\,\mathrm{ns},\qquad T=5\cdot2+7\cdot32=234\,\mathrm{ns}.
$$

With four [cache slots](cache-slot.md), its four [compulsory misses](compulsory-miss.md) instead give $\operatorname{AMAT}=12\,\mathrm{ns}$. This comparison holds the timing costs fixed as capacity changes, which is a model assumption rather than a hardware promise.

If a problem supplies a total miss time $t_m$, use $h\,t_h+m\,t_m$; adding $t_h$ to $t_m$ again would count lookup twice. Variable [cache miss penalties](cache-miss-penalty.md), multiple consulted levels, or overlapping requests require a richer timing model. Real [CPU](central-processing-unit.md) work can overlap a pending read, so this [arithmetic mean](arithmetic-mean.md) cannot by itself predict program speed or stall time. [Memory part 2: CPU caches by Ulrich Drepper](memory-part-2-cpu-caches-by-ulrich-drepper.md)

## ↑ Ancestors (5)

1. [Memory access latency](memory-access-latency.md)
2. [Cache (computing)](cache-computing.md)
3. [Computer memory](computer-memory.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cache (computing)](cache-computing.md)
- [Cache miss penalty](cache-miss-penalty.md)
- [Memory access latency](memory-access-latency.md)
