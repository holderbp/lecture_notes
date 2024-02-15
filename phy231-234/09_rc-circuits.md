# RC Circuits

## Introduction and Overview

In the past few lectures we have studied circuits, in particular *circuits in equilibrium*. We looked at charged capacitors, which had been attached to an EMF (e.g., a battery) for a long time, leaving a charge $Q_\text{tot} = C \Delta V_C$.  We then looked at DC circuits with resistors, and we assumed that the currents in every wire was constant, unchanging in time.

Today we consider the first case of a circuit with *changing* current (we will see another example when we look at alternating current (AC) circuits, in which the power source is a sinusoidally oscillating EMF). Specifically, we will look at circuits with one capacitor and one resistor, and consider:

1. The discharge ($Q_\text{tot} \rightarrow 0$) of a charged capacitor, and
2. The charging of an unchanged capacitor ($0 \rightarrow Q_\text{tot}$) when connected to an EMF.

In each case, we will derive the time dependence of charge accumulation/loss, $Q(t)$, and thus also the dependence of $I(t)$ and $\Delta V_c(t)$.

To determine $Q(t)$ in each case above, we will write down a loop rule equation, $\sum \Delta V = 0$, show that it is actually a differential equation, and then solve the differential equation.

## Introduction to Differential Equations

Given a quantity, \( X \), that depends on time, a differential equation describes that time dependence through the derivatives of the quantity. For example:

\[
\frac{d^2X}{dt^2} + a \frac{dX}{dt} + b = 0 \quad \text{or} \quad \frac{dX}{dt} = aX^2
\]

The first example is called a linear differential equation because each term contains, at most, one power of \( X \); the right example is called a nonlinear differential equation because it contains an \( X^2 \) term. Generally, a linear equation can be solved, i.e., we can write down exactly how the quantity depends on time, \( X(t) = f(t) \), where \( f(t) \) is the solution and \( X_0 = f(0) \) is an initial condition. A nonlinear differential equation generally needs to be solved "numerically", using a computer. The left example is called a second-order differential equation because it contains a second derivative. The right example is a first-order diff. eqn.

The solution to a first-order differential equation will have one unknown constant. The value of the constant must be set by your choice of the \( X_0 \) initial condition. A second-order diff. eqn solution contains two constants, set by \( X_0 \) and \( \frac{dX}{dt}(t=0) \).

We encountered one example of a linear differential equation in PHY230, while studying oscillatory motion. Newton's second law applied to a mass on a spring was:

\[
\vec{F} = m\vec{a} \quad \Rightarrow \quad F_{\text{spring}} = -kx = m\frac{d^2x}{dt^2} \quad \Rightarrow \quad -kx = m\frac{d^2x}{dt^2}
\]

We found that this second-order differential equation has the following solution:

\[
\frac{d^2x}{dt^2} = -kx \quad \Rightarrow \quad x(t) = A \cos(\omega t + \phi) \quad \text{with} \quad \omega^2 = \frac{k}{m}
\]

Because if you take two derivatives of \( x(t) \), you obtain \( -\omega^2 x(t) \). The arbitrary constants in this solution, \( A \) and \( \phi \), were set by our choice of initial conditions, the initial position, \( x(0) \), and velocity, \( v(0) \).


![A mass on a spring, the classic harmonic oscillator.](images/09_mass-on-spring.png)

## Discharging a Capacitor

![Charging and then discharging a capacitor.](images/09_charging-and-discharging-capacitor.png)

![Graphs of charge (Q), current (I), and potential difference when discharging a capacitor.](images/09_QIV-graphs-discharging.png)

## Charging a Capacitor

![Graphs of charge (Q), current (I), and potential difference when charging a capacitor.](images/09_QIV-graphs-charging.png)