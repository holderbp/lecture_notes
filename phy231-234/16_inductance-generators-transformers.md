# Applications of Induction: Generators & Transformers

## Inductors and Inductance in Circuits

We will not spend much time on inductors, or the AC (alternating current) circuits where they are important, but you should know that there is a circuit element called an inductor which is simply a coil of wire.

![Circuit diagram with a battery/emf, a resistor, and an inductor/coil (L)](images/16_inductor-circuit.png)

Qualitatively, we can understand that there will be a potential difference across the inductor
```math
\Delta V_L = \Delta V_{ab}
```
Whenever the current through the coil is *changing*. The potential difference will be due to the induced EMF (caused by the changing $\vec{B}$ field in the coil, caused by the changing current).

Closing the switch in the circuit above causes an increasing current, which cases an increasing $\vec{B}_\text{coil}$ which causes an oppositely-pointed $\vec{B}_\text{ind}$.

![An inductor with current flow has its own magnetic field but when that field increases in strength (as current increases) it will generate an induced magnetic field in the opposite direction, which causes an opposing current.](images/16_inductors-with-current.png)

Opening the switch causes the current to decrease, and a  decreasing current causes decreasing $\vec{B}_\text{coil}$ which causes $\vec{B}_\text{ind}$ in the same direction as the original field:

![An inductor with current flow has its own magnetic field but when that field decreases in strength (as current decreases) it will generate an induced magnetic field in the same direction, which causes more  current in the same direction.](images/16_inductors-with-current-two.png)

We define the *inductance* (or "self-inductance"), $L$, of an inductor as the constant of proportionality between magnetic flux through the coil and the current passing through the coil:
```math
\Phi_B = L I
```
From here we can determine the potential difference across an inductor. Find the "rate" of the above definition (change wrt time):
```math
\begin{align}
\frac{\Delta \Phi_B}{\Delta t} &= L \frac{\Delta I}{\Delta t} \\
\varepsilon_{\text{ind}} &= L \frac{\Delta I}{\Delta t}\\
\Delta V &= L \frac{\Delta I}{\Delta t}
```
Note that $L$ doesn't change in time; it is a constant.

So we see that the potential difference depends on the rate of change of the current in time.

Although we define $L$ in terms of $\Phi_B$ and $I$, the value actually depends only on the physical properties of the coil itself (e.g., $N_{\text{loops}}$, diameter, ...). This is similar to how, recall, the capacitance, $C$, and resistance, $R$, also depend only on the physical characteristics of the circuit element.



