
# Inductors, RL and RLC Circuits

## Introduction and Overview

Last time, we introduced the idea of induction; so-called "Mutual Induction" of two coils, and "Self-Induction" of a single coil. We showed how the former led to devices called transformers which are workhorses of our AC power network. Today we will focus on the latter, in particular the use and function of inductors in a circuit.

In particular we will consider the dynamics of current flow in circuits with both inductors and resistors (RL circuits) and those with capacitors as well (RLC circuits). This will provide necessary background for the next lecture where we attach an AC voltage source to such circuits and study AC circuits in their full glory.

![A simple resistor-inductor (RL) circuit](images/17_simple-RL-circuit.png)

In addition to the dynamics (i.e., current flow over time) of these circuits, we will also focus on their purpose: energy storage devices. Just as a charged capacitor stores energy in its electric field (which could be released and utilized by discharging it), an inductor stores energy in its magnetic field.

## Review of Inductors

An inductor is simply a coil of wire used as an element in a circuit. If current in the coil is constant, then there is a constant magnetic field in the coil. But if the current is changing, then its own magnetic field strength is changing, and, by Faraday's Law, there is an additional induced current, driven by the induced EMF, which acts to oppose the change in magnetic flux in the coil.

Because the magnitude $|\mathbf{E}|$, and therefore magnetic flux $\Phi_B$, is proportional to current, we expect the induced EMF in the coil to be proportional to the change of the current, i.e., from Faraday's Law (treating the coil's own magnetic field as the "external field" ) we find the **defining equation of inductance**:
```math
\mathcal{E}_{\text{ind}} = - \frac{d\Phi_B}{dt} \propto \frac{dI}{dt} \quad \rightarrow \quad \mathcal{E}_{\text{ind}} = - L \frac{dI}{dt}
```
where the constant of proportionality, $L$, is called the inductance of the coil. We see that it has units of:
```math
[\mathcal{E}] = [L] \left[\frac{dI}{dt}\right] \quad V = \left[\frac{Vs}{A}\right] \quad \text{hence}, \quad [L] = \frac{Vs}{A} = H, \text{"Henry"}
```

In the following, we will show that inductance, just like capacitance, depends only on the physical properties of the coil (its geometry and windings), and not, e.g., on the current flowing through it.

### How to calculate inductance of an inductor

We can write the defining equation of inductance in terms of magnetic flux using Faraday's Law:
```math
\begin{align}
\mathcal{E}_{ind} &= L \frac{dI}{dt}\\
\frac{d}{dt} (N\Phi_B) &= L \frac{dI}{dt}
\end{align}
```
We can then integrate this equation with respect to time (dropping abs. values):
```math
\begin{align}
\int \frac{d}{dt} (N\Phi_B) dt & = L \int \frac{dI}{dt} dt \\
N\Phi_B &= LI + C \\
N\Phi_B &= LI 
\end{align}
```
where, in the last step, we can assume that when $I(t) = 0$, the flux is also $\Phi_B(0) = 0$, so the integration constant becomes $C = 0$.

Therefore we can express inductance as a ratio of flux to current at any moment of time:
```math
L = \frac{N\Phi_B}{I}
```
(Note that this does not mean that the inductance depends on current; we know that \( \Phi_B \) is proportional to \( I \), so it cancels in this equation.) This equation allows us to find \( L \) for some common coil types.

### Inductance of a long solenoid

![Solenoid with N loops and loop density per length n](images/17_coil-n-N.png)

To use the above equation, we recall the expression (derived using Ampère's Law) for the magnetic field of a solenoid with \( n \) windings per unit length:
```math
B_{solenoid} = \mu_0 n I = \frac{\mu_0 n I}{l}
```
Therefore
```math
\Phi_B = BA = \mu_0 n I A \Rightarrow L = \frac{N\Phi_B}{I} = \frac{\mu_0 N^2 A}{l}
```
And we see that the inductance per unit length is:
```math
\frac{L_{solenoid}}{l} = \mu_0 n^2 A
```

### Inductance of a (rectangular cross-section) toroidal solenoid

![A toroidal solenoid with rectangular cross-section. We can break up that cross section into chunks to integrate the field flux.](images/17_toroidal-solenoid-chunks.png)

Recall that the magnetic field of a toroidal solenoid depends only on \( r \), the distance from its center, \( B_T \propto \frac{1}{r} \). To calculate the flux here, we must do an integral (choosing a rectangular cross-section simplifies this):
```math
\Phi_B = \sum_{i=1}^{N} B_{A_n} = \sum_{i=1}^{N} \frac{\mu_0 n I}{2\pi r} A \Rightarrow \Phi_B = \int_a^b \frac{\mu_0 n I}{2\pi r} dr
```
So we find that
```math
\Phi_B = \frac{\mu_0 n I}{2\pi} \ln \left(\frac{b}{a}\right) \Rightarrow L = \frac{N\Phi_B}{I} = \frac{\mu_0 N^2}{2\pi} \ln \left(\frac{b}{a}\right)
```

