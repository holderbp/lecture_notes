DC Circuits
===========

AC/DC (and "RC")
--------------------------------------------

Today we will discuss **"direct-current" (DC) circuits**. These are circuits powered by EMF devices providing a constant potential difference, such as a battery.  Once the battery (or batteries) is connected to the circuit (today: a system of resistors), the current in each wire will have a constant value and direction.  (By "each wire" we mean each juntionless wire; upon reaching a junction, the currents will split/add.) 

![Simple DC Circuit](images/08_dc-circuit.png)

After studying magnetic fields, and magnetic induction in particular, we will see that it is often easier to produce an *alternating* source of EMF, where the value of the potential oscillates sinusoidally.  Attaching such a power source to a system of resistors (or other circuit elements) creates an **alternating-current (AC) circuit**.

![Simple AC Circuit](images/08_ac-circuit.png)

Next time we will consider a special case of DC circuits, those with resistors and capacitors: **RC Circuits**.  Since a capacitor is effectively a broken wire, current will be zero long after the battery is connected to such a circuit.  We will therefore be interested in the short-term behavior: charging (or dis-charging a capacitor).

![Simple RC Circuit](images/08_rc-circuit.png)

[RC circuits become more interesting when connected to an AC source, because then they are *constantly* charging and discharging.]

Potential and current in a DC circuit
--------------------------------------------

### Overview

To understand a circuit, one must determine:

1. The value of the potential at all points (relative to an arbitrary zero value, e.g., the "negative" terminal of the battery), and

2. The the value and directin of the current in each wire and/or circuit element.

**Potential**: The potential is *raised* when crossing a battery (from - to +), *remains the same* along wires (since $R_\text{wire} = 0$ and, by Ohm's Law, $\Delta V_\text{wire} = I R_\text{wire} = 0), and *drops* across a resistor or capacitor (recall: $\Delta V_R = I R$ and $\Delta V_C = Q/C$).

![Potential values shown as colors at all points on a circuit with a battery, two resistors, and a capacitor.  The potential difference across each element should be thought of as a "difference in color".  For example, the battery has a potential difference of "red to blue".](images/08_coloring-potential-simple-RC-circuit.png)

**Current**: The current is the flow of charge past a point in the circuit, so --- like a fluid --- the current is *constant* at all points on a junctionless wire (a fluid flow is constant through a pipe, until that pipe splits).  And current *splits* or *merges* at a junction of wires.

![Simple DC circuit showing current flow, with a different value for each of the three individual junctionless wires.](images/08_current-flow-three-resistor-circuit.png)

Note that, in the figure above:
- The current through the battery, $I_\text{batt}$, is the same as the current through $R_1$.
- At junction A, current splits such that $I_\text{batt} = I_1+ I_2$.
- The current through R_3 and R_4 is the same.
- At junction B, current merges.

### Kirchoff's Rules

Equivalent Resistance
--------------------------------------------

Application of Kirchoff's Rules
--------------------------------------------

### Overview

### Algorithm for solving any DC circuit

1. 

2. 