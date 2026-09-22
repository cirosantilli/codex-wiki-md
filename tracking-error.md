# Tracking error

↑ **Parent:** [Closed-loop control](closed-loop-control.md)

The [tracking error](tracking-error.md) used by the [controller](controller-control-theory.md) is the signed difference

$$
e(t)=r(t)-y_m(t),
$$

between the [reference signal](reference-signal.md) and the [measured output](measured-output.md). A positive [tracking error](tracking-error.md) means the readout is below the desired value; a negative [tracking error](tracking-error.md) means it is above. With exact measurement $y_m=y$, $r=1$ and $y=1.1$ give $e=-0.1$. For a positive-response [controlled plant](plant-control-theory.md), positive [feedback gain](feedback-gain.md) in [proportional control](proportional-control.md) $u=k_p e$ then reduces the [plant output](output-control-theory.md). The sign of the [controller](controller-control-theory.md) must also account for the sign of the [controlled plant](plant-control-theory.md)'s response: a positive command that reduces the [plant output](output-control-theory.md) requires a different sign choice. Kantor uses the opposite [tracking error](tracking-error.md) convention, $PV-SP$, together with a minus sign in his [controller](controller-control-theory.md); translating both signs gives the convention here. [Jeffrey Kantor, negative feedback and proportional-control equations](https://jckantor.github.io/cbe30338-book/notebooks/03.06-Proportional-Integral-Control.html)

Distinguish the [controller](controller-control-theory.md)'s [tracking error](tracking-error.md) from the physical [plant output](output-control-theory.md) discrepancy $\varepsilon=r-y$. If the readout has constant [sensor bias](sensor-bias.md) $b$, then

$$
y_m=y+b,\qquad e=\varepsilon-b,\qquad \varepsilon=e+b.
$$

All four quantities $r,y,y_m,e$ have the same units under [dimensional analysis](dimensional-analysis.md); a [sensor bias](sensor-bias.md) is expressed in those units too. A readout that is too high by $0.2\,{}^\circ\mathrm C$ can make $e=0$ when the physical [temperature](temperature.md) is $0.2\,{}^\circ\mathrm C$ below the goal. [Integral action](integral-action.md) integrates the [tracking error](tracking-error.md) it receives; it cannot infer this missing calibration information from that [tracking error](tracking-error.md) alone. [Thermometer calibration](thermometer-calibration.md) against an independent reference addresses a different problem from tuning a [feedback gain](feedback-gain.md).

<a id="image-reference-signal-tracking-error-and-a-biased-measured-output"></a>
![](tracking-reference-errors-signals.png)

**[Figure 4](#image-reference-signal-tracking-error-and-a-biased-measured-output). Reference signal, tracking error, and a biased measured output**. Original signal diagram with a synthetic [equilibrium point](equilibrium-point-of-a-dynamical-system.md) for [proportional-integral control](proportional-integral-control.md). All output coordinates are [temperature](temperature.md) rises above one fixed baseline; the [control input](control-input.md) is in heater-command percentage points. With $r=1$ and [sensor bias](sensor-bias.md) $b=0.2$, zero measured [tracking error](tracking-error.md) means $y_m=1$, while the physical [plant output](output-control-theory.md) is $y=0.8$ and its discrepancy is $\varepsilon=0.2$. No plotted laboratory measurements are implied.

A motivating apparatus/model comparison is Park, Martin, Kelly and Hedengren's temperature-control laboratory: two TIP31C heaters with attached TMP36GZ sensors and heat sinks, an Arduino, a power supply, and a USB-connected computer. The readout converts sensor [voltage](voltage.md) to [temperature](temperature.md); software records that [measured output](measured-output.md) while specifying heater commands from $0$ to $100\%$. For the single-heater test, one command changes in steps and the other heater stays off. Parameters are fitted to one run, then a different command sequence tests predictions without feeding measured [temperatures](temperature.md) into the simulation. The authors observe that their richer thermal model predicts the response better than the approximation with a single [time constant](time-constant.md) and a delayed [control input](control-input.md), especially after command changes. The real sensor has its own thermal lag. They also repeat the same command profile at different ambient [temperatures](temperature.md) and find changes in the response, motivating ambient-condition reporting. This experiment measures a command-to-readout response, not independently the exact heater [temperature](temperature.md) or delivered power. [Park, Martin, Kelly and Hedengren, Benchmark Temperature Microcontroller for Process Dynamics and Control, sections 2 and 3, Figures 3, 6 and 7: author-uploaded full text](https://www.researchgate.net/publication/338614896_Benchmark_Temperature_Microcontroller_for_Process_Dynamics_and_Control)

The lesson for [tracking error](tracking-error.md) is to record three traces during a tracking test: the [reference signal](reference-signal.md), the [measured output](measured-output.md), and the applied [control input](control-input.md). Their first difference is the [tracking error](tracking-error.md); a model prediction minus a readout is instead a model discrepancy. In a proposed comparison of [proportional control](proportional-control.md) and [proportional-integral control](proportional-integral-control.md), keep the initial [temperature](temperature.md), ambient conditions, heater limits, and target changes fixed; run the second heater separately as a known [control disturbance](control-disturbance.md). Independent [thermometer calibration](thermometer-calibration.md) is needed to assess physical accuracy. These are suggested controls, not additional experiments claimed for the paper. A sensor's lag, [measurement noise](measurement-noise.md), [actuator saturation](actuator-saturation.md), and changed ambient conditions can all invalidate conclusions drawn from the ideal first-order model.

**Table of contents**

- [Steady-state tracking error](steady-state-tracking-error.md)

## ↑ Ancestors (5)

1. [Closed-loop control](closed-loop-control.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Actuator saturation](actuator-saturation.md)
- [Closed-loop control](closed-loop-control.md)
- [Control theory](control-theory-split.md)
- [Feedback gain](feedback-gain.md)
- [Integral action](integral-action.md)
- [PID controller](pid-controller.md)
- [Proportional control](proportional-control.md)
- [Proportional-integral control](proportional-integral-control.md)
- [Reference signal](reference-signal.md)
- [Sensor bias](sensor-bias.md)
- [Steady-state tracking error](steady-state-tracking-error.md)
- [Tracking error](tracking-error.md)
