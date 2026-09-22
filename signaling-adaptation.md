# Signaling adaptation

↑ **Parent:** [Signal transduction](signal-transduction.md)

[Signaling adaptation](signaling-adaptation.md) is a decline of a response toward its earlier level while the initiating [signal](signal.md) remains present. Specify which response is measured and its baseline: complete [signaling adaptation](signaling-adaptation.md) means eventual return to that baseline; partial [signaling adaptation](signaling-adaptation.md) leaves a lasting displacement. The continuing [signal](signal.md) distinguishes [signaling adaptation](signaling-adaptation.md) from simply switching off the stimulus. [Signaling adaptation](signaling-adaptation.md) describes behavior, while [signaling feedback](signaling-feedback.md) describes a causal arrangement, so neither implies the other.

By reducing a persistent response to background [ligand](ligand-biochemistry.md) [concentration](concentration.md), [signaling adaptation](signaling-adaptation.md) can make a [biological cell](biological-cell.md) sensitive to changes rather than only to absolute levels. Resetting the response helps leave room for another change over a useful range of [ligand](ligand-biochemistry.md) [concentrations](concentration.md). This is valuable in [chemotaxis](chemotaxis.md): swimming [bacteria](bacteria.md) encounter changing chemical conditions, and their [signal transduction](signal-transduction.md) influences whether a run continues or a tumble occurs. [Signaling adaptation](signaling-adaptation.md) helps separate a change encountered during motion from a lasting background. This usefulness does not imply exact return or equal sensitivity at every possible [concentration](concentration.md). [General Principles of Cell Communication](molecular-biology-of-the-cell-4th-edition-by-bruce-alberts-and-others/general-principles-of-cell-communication.md) [Yi, Huang, Simon and Doyle, PNAS 97 (2000), pp. 4649–4653: chemotaxis and adaptation](https://groups.csail.mit.edu/mac/projects/amorphous/6.978/papers/doyle-PNAS-2000.pdf)

Here is a solvable [incoherent feedforward loop](incoherent-feedforward-loop.md) toy that exhibits complete [signaling adaptation](signaling-adaptation.md) without [signaling feedback](signaling-feedback.md). The input $s(t)$ jumps from $0$ to $1$ at $t=0$ and remains $1$, a [Heaviside step function](heaviside-step-function.md). Let $x$ be a fast activating branch, $a$ a slower inhibitory branch, and $r=x-a$ a readout. The activities $s,x,a,r$ are [dimensionless variables](dimensionless-variable.md); physical time is in seconds. Choose [time constants](time-constant.md) $\tau_x=1$ second and $\tau_a=5$ seconds, with [initial conditions](initial-condition.md) $x(0)=a(0)=0$:

$$
\tau_x\frac{dx}{dt}=s-x,\qquad \tau_a\frac{da}{dt}=s-a,\qquad r=x-a.
$$

Both branches read $s$ directly. Neither branch depends on $r$, and $a$ does not change $x$: the subtraction only defines the readout. Thus the slow opposing influence is feedforward, with no closed [feedback control](closed-loop-control.md) loop.

For $t\geq0$, solving the two [ordinary differential equations](ordinary-differential-equation.md) gives

$$
x(t)=1-e^{-t/\tau_x},\qquad a(t)=1-e^{-t/\tau_a},\qquad r(t)=e^{-t/\tau_a}-e^{-t/\tau_x}.
$$

Writing $t$ for the numerical time in seconds, these are $x=1-e^{-t}$, $a=1-e^{-t/5}$ and $r=e^{-t/5}-e^{-t}$. Initially $r=0$, then $x$ rises faster than $a$, producing a pulse. At long times $x$ and $a$ both approach $1$, so $r$ returns to $0$ despite sustained $s=1$. For this upward step $e^{-t/5}\geq e^{-t}$, hence $r(t)\geq0$. The striking feature of this [signaling adaptation](signaling-adaptation.md) toy is that both branches remain active while the readout becomes quiet: the continuing background and the response to its arrival are separable.

<a id="image-a-sustained-unit-input-and-a-transient-readout-in-an-incoherent-feedforward-loop-toy"></a>
![](signaling-adaptation-step-response.png)

**[Figure 7](#image-a-sustained-unit-input-and-a-transient-readout-in-an-incoherent-feedforward-loop-toy). A sustained unit input and a transient readout in an incoherent feedforward loop toy**. Original computed curves for [time constants](time-constant.md) of $1$ and $5$ seconds, zero [initial conditions](initial-condition.md), and normalized [dimensionless variables](dimensionless-variable.md). The upper panel shows the sustained input and the two branches; the lower panel shows the readout $r=x-a$, its maximum near $2.0118$ seconds, and its approach to the zero baseline. Values and time scales are chosen for illustration, not fitted to a measured [signal transduction](signal-transduction.md) pathway.

Find the pulse maximum by differentiating the [exponential functions](exponential-function.md). With numerical time in seconds, the [derivative](derivative.md) is

$$
r'(t)=-\frac15e^{-t/5}+e^{-t}.
$$

The stationary condition is $e^{-4t/5}=1/5$, so the [natural logarithm](natural-logarithm.md) gives

$$
t_{\mathrm{peak}}=\frac54\ln5\simeq2.0118\ \text{seconds},\qquad r_{\mathrm{peak}}=\frac45\,5^{-1/4}\simeq0.53499.
$$

Before this time the [derivative](derivative.md) is positive; afterwards it is negative. Together with $r(0)=0$ and $\lim_{t\to\infty}r(t)=0$, this proves that it is the unique pulse maximum. As another numerical check, at $t=10$ seconds $x\simeq0.999955$, $a\simeq0.864665$ and $r\simeq0.135290$: the slow branch is still catching up.

The subtraction $r=x-a$ is a mathematical readout, not a claim that an actual chemical [concentration](concentration.md) equals this difference for arbitrary inputs. Nonnegativity was established only for the specified upward step; other input histories can give a negative signed readout. Complete [signaling adaptation](signaling-adaptation.md) here also relies on equal eventual branch gains: changing the readout to $r=x-0.9a$ leaves $r_*=0.1$ for $s=1$. This toy illustrates cancellation and different [time constants](time-constant.md); it does not establish molecular implementation or robustness to arbitrary parameter changes. Ma and colleagues' 2009 study separately analyzed biochemical [mathematical models](mathematical-model.md) with [negative feedback](negative-feedback.md) and [incoherent feedforward loops](incoherent-feedforward-loop.md), identifying additional conditions for [signaling adaptation](signaling-adaptation.md) in those models. [Ma et al., Cell 138 (2009): adaptive architectures and their kinetic conditions](https://cqb.pku.edu.cn/tanglab/pdf/78.pdf)

A historical connection to [feedback control](closed-loop-control.md) comes from Yi, Huang, Simon and Doyle's 2000 analysis of a bacterial [chemotaxis](chemotaxis.md) model. They identified [integral action](integral-action.md) in its regulation of [receptor](receptor-biochemistry.md) activity: accumulated deviations alter a slower adjustment, which in turn changes the measured activity. At a stationary state, an adjustment that integrates a nonzero error cannot remain constant, explaining how zero error can follow. Their conclusion depended on stated biochemical assumptions and stable behavior; it was not a claim that every [biological cell](biological-cell.md) uses that mechanism. A transient pulse alone, as the [incoherent feedforward loop](incoherent-feedforward-loop.md) toy shows, cannot identify the underlying [signaling feedback](signaling-feedback.md) architecture. [Yi et al., Robust perfect adaptation in bacterial chemotaxis through integral feedback control, PNAS 97 (2000): Results and Discussion](https://groups.csail.mit.edu/mac/projects/amorphous/6.978/papers/doyle-PNAS-2000.pdf)

## ↑ Ancestors (3)

1. [Signal transduction](signal-transduction.md)
2. [Biology](biology-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Chemotaxis feedback regulation](chemotaxis-feedback-regulation.md)
- [CheR](cher.md)
- [Incoherent feedforward loop](incoherent-feedforward-loop.md)
- [Morphogen response threshold](morphogen-response-threshold.md)
- [Negative feedback](negative-feedback.md)
- [Signal transduction](signal-transduction.md)
- [Signaling adaptation](signaling-adaptation.md)
- [Signaling feedback](signaling-feedback.md)
