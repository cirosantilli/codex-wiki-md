<h1 id="duration-of-gambler-s-ruin-conditioned-on-a-chosen-boundary">Duration of gambler's ruin conditioned on a chosen boundary</h1>

↑ **Parent:** [Gambler's ruin](gambler-s-ruin.md)

For a simple symmetric random walk absorbed at $0,r$, the probability of absorption at $0$ is $h_i=(r-i)/r$. Conditioning on that absorption gives the [Doob h-transform](doob-h-transform.md) with transition probabilities $(r-i+1)/[2(r-i)]$ downwards and $(r-i-1)/[2(r-i)]$ upwards. If $g_i=\mathbb E_i[\tau\mathbf1_{\{\tau_0<\tau_r\}}]$, first-step analysis gives $g_i=h_i+(g_{i-1}+g_{i+1})/2$, $g_0=g_r=0$. Its solution is $g_i=i(r-i)(2r-i)/(3r)$, and dividing by $h_i$ gives the conditional duration.

## ↑ Ancestors (8)

1. [Gambler's ruin](gambler-s-ruin.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/19c/solution.md)
