# Two-state ion-channel gating

↑ **Parent:** [Voltage-gated ion channel](voltage-gated-ion-channel.md)

[Two-state ion-channel gating](two-state-ion-channel-gating.md) models an individual gate as a random switch between closed and open states. Write $p(t)$ for its open [probability](probability.md); this is the $X$ in the header equation. An individual gate's state is always closed or open, rather than partly open. A population of identical gates can have a fraction open near $p(t)$, and averaging repeated identically prepared trials estimates the same [probability](probability.md). A finite population's observed fraction fluctuates. See [Purves and colleagues, Neuroscience, 2nd edition (2001): Ion Channels Underlying Action Potentials](https://www.ncbi.nlm.nih.gov/books/NBK10841/) for single-channel steps and their population averages.

At fixed [membrane potential](membrane-potential-split.md) $V$, let constant rates $\alpha,\beta>0$ govern closed-to-open and open-to-closed transitions respectively, in $\mathrm{s}^{-1}$. This is a two-state [continuous-time Markov chain](continuous-time-markov-chain-split.md). Over a short interval $\Delta t$, an initially closed gate opens with [probability](probability.md) $\alpha\Delta t+o(\Delta t)$, and an initially open gate closes with [probability](probability.md) $\beta\Delta t+o(\Delta t)$. Gain minus loss gives the deterministic [ordinary differential equation](ordinary-differential-equation.md) for the [probability](probability.md):

$$
\frac{dp}{dt}=\alpha(1-p)-\beta p=\frac{p_\infty-p}{\tau},\qquad
p_\infty=\frac{\alpha}{\alpha+\beta},\qquad \tau=\frac{1}{\alpha+\beta}.
$$

Here $p_\infty$ is the fixed-voltage limiting open [probability](probability.md), and $\tau$ is a [time constant](time-constant.md). The ratio of the rates fixes the limit, while their sum fixes the speed. With initial [probability](probability.md) $p(0)=p_0\in[0,1]$,

$$
p(t)=p_\infty+(p_0-p_\infty)e^{-t/\tau}.
$$

For a short derivation, subtract $p_\infty$: the deviation obeys $d(p-p_\infty)/dt=-(p-p_\infty)/\tau$, yielding the [exponential function](exponential-function.md). After one [time constant](time-constant.md), $1/e$ of the initial deviation remains. The solution stays between $p_0$ and $p_\infty$, so it remains a valid [probability](probability.md). The rate and [time constant](time-constant.md) formulations are described in [Gerstner and colleagues, Neuronal Dynamics, §2.2.2: transition rates and channel kinetics](https://neuronaldynamics.epfl.ch/online/Ch2.S2.html).

For a worked toy condition A, choose $\alpha=\beta=50\,\mathrm{s}^{-1}$ and $p_0=0.1$. Then $p_\infty=0.5$, $\tau=0.01\,\mathrm{s}=10\,\mathrm{ms}$, and

$$
p(10\,\mathrm{ms})=0.5-0.4e^{-1}\approx0.352848.
$$

In a separately prepared condition B, choose $\alpha=200\,\mathrm{s}^{-1}$, $\beta=50\,\mathrm{s}^{-1}$ and the same $p_0=0.1$. Now $p_\infty=0.8$, $\tau=4\,\mathrm{ms}$, and $p(10\,\mathrm{ms})=0.8-0.7e^{-2.5}\approx0.742540$. Condition B approaches a higher limit more quickly. These are two stipulated constant-rate conditions with $V$ held fixed in each experiment, not an empirical function relating rates to voltage or a sequential switch between conditions. The initial $p_0=0.1$ need not be the limiting [probability](probability.md) at the newly imposed voltage.

<a id="image-two-state-ion-channel-gating-two-constant-rate-relaxation-conditions"></a>
![](ion-channel-gating-relaxation.png)

**[Figure 4](#image-two-state-ion-channel-gating-two-constant-rate-relaxation-conditions). Two-state ion-channel gating: two constant-rate relaxation conditions**. Original computed [probability](probability.md) curves, both starting at $p_0=0.1$. Dashed lines show the limiting open [probabilities](probability.md) $0.5$ and $0.8$; dotted lines mark [time constants](time-constant.md) $10$ and $4\,\mathrm{ms}$. The dot marks condition A at $10\,\mathrm{ms}$, where $p\approx0.352848$. Smooth curves represent open [probability](probability.md) or population averages, not an individual gate's random state trace or an ionic [electric current](electric-current.md).

In the [Hodgkin-Huxley model](hodgkin-huxley-model.md), the rates depend on [membrane potential](membrane-potential-split.md): $\alpha_X(V)$ and $\beta_X(V)$. Its $X_\infty(V)=\alpha_X(V)/(\alpha_X(V)+\beta_X(V))$ is the limit for voltage held at that $V$. During an [action potential](action-potential.md), changing $V$ changes the rates and gates feed back onto $V$ through ionic [electric currents](electric-current.md); substituting the present voltage into the constant-rate solution does not solve that coupled system. Gating describes availability of a conducting pathway. Even an open [ion channel](ion-channel.md) carries zero net ionic [electric current](electric-current.md) at its [reversal potential](reversal-potential.md).

The useful bridge is from abrupt random molecular events to a smooth population prediction. A channel requiring several [independent permissive gates in an ion channel](independent-permissive-gates-in-an-ion-channel.md) has an open [probability](probability.md) equal to their product; this can make channel availability much smaller than each gate's availability. The [Hodgkin-Huxley model](hodgkin-huxley-model.md) uses $\bar g_{\mathrm{Na}}m^3h$ and $\bar g_{\mathrm K}n^4$ for [sodium](sodium.md) and [potassium](potassium.md) [electrical conductances](electrical-conductance.md), respectively.

**Table of contents**

- [Independent permissive gates in an ion channel](independent-permissive-gates-in-an-ion-channel.md)

## ↑ Ancestors (5)

1. [Voltage-gated ion channel](voltage-gated-ion-channel.md)
2. [Membrane potential](membrane-potential-split.md)
3. [Biological cell](biological-cell-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Biology](biology-split.md)
- [Hodgkin-Huxley model](hodgkin-huxley-model.md)
- [Ion channel](ion-channel.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/3/a/solution.md)
- [Two-state ion-channel gating](two-state-ion-channel-gating.md)
