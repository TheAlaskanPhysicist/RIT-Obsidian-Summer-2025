Lecture: https://www.youtube.com/watch?v=4RX_lpoGRBg
https://www.youtube.com/watch?v=4RX_lpoGRBg&list=PLUl4u3cNGP60gl3fdUTKRrt5t_GPx2sRg


### What is Statistical Mechanics / Thermodynamics
Statistical Mechanics is a probabilistic approach to equilibrium properties of large numbers of degrees of freedom.

> Do non-equilibrium statistical mechanics require more degrees of freedom? If so, how much?
> Can we expand equilibrium to N-th order perturbations?
> Does the equilibrium drastically reduce the amount of information we need to encode the system? Hence why we usually look only at equilibrium statistical mechanics?

Thermodynamics is a phenomenological description (mathematical description of direct observation of reality) of equilibrium properties of microscopic systems.

We can look at a black box and, through observation, build a mathematical framework to describe its properties. Very useful for a lot of physics and science.

Newtonian mechanics lacks description of heat and other thermal properties.

### Preliminary Definitions
**System:** Isolate system thermally (by adiabatic laws).
- Isolated from the rest of the universe in a box that doesn't allow heat transfer.
**Diathermic:** Systems that allow heat flow in and out of the system.

**Equilibrium:** When "properties" don't change over observation time.

**Properties:** Mechanical properties
 - ($V$, $P$), volume and pressure of a gas
 - ($L$,$F$), length and force of a wire
 - ($\vec{M}$,$\vec{B}$), magnetization and magnetic field of a magnet.
But there are also thermal properties we don't know yet.

These are like the analogues of the coordinates and velocities of any Newtonian particle.
We want to find rules that these coordinates are coevolving, based off of observation.

**Phenomenology:** Observations $\rightarrow$ Laws


### 0th Law of Thermodynamics
**0th Law:** If two systems, $A$ and $B$ are both in equilibrium with system $C$, then $A$ must be in thermal equilibrium with $B$. Equilibrium is transitive.
$$\begin{align}
A\leftrightarrow C \ \land \ B\leftrightarrow C\ \implies A\leftrightarrow B
\end{align}$$
This adds one more coordinate to the description above, being the analogue of temperature.
Transitivity of equilibrium implies the existence of a "temperature."

> Given a set of physical systems and an operator $\leftrightarrow$, we can make a group of sorts that has transitivity? What other properties does equilibrium have? How do higher-order approximations change that?

Not necessarily mathematically rigorous, but physically correct.
If a system reaching equilibrium, it has a set of coordinates.
$$\begin{align}
A&:\{A_1,A_2,\dots\} & B&:\{B_1,B_2,\dots\} & C&:\{C_1,C_2,\dots\}\\
\end{align}$$
What it means to have an equilibrium of $A$ and $B$ is as follows:
$$\begin{align}
f_\text{AC}(A\cup C)&=f_\text{AC}(A_1,A_2,\dots,C_1,C_2,\dots)=0\\
f_\text{BC}(B\cup C)&=f_\text{BC}(B_1,B_2,\dots,C_1,C_2,\dots)=0\\
\end{align}$$
We can then suppose some new function $F$ such that:
$$\begin{align}
C_1&=F_\text{AC}(A_1,A_2,\dots,C_2,C_3,\dots)\\
C_1&=F_\text{BC}(B_1,B_2,\dots,C_2,C_3,\dots)\\
\end{align}$$
Given that $A\leftrightarrow C \ \land \ B\leftrightarrow C$, then:
$$\begin{align}
F_\text{AC}(A_1,A_2,\dots,C_2,C_3,\dots)&=F_\text{BC}(B_1,B_2,\dots,C_2,C_3,\dots)\\
\end{align}$$
Equilibrium of $A$ and $B$ then implies:
$$\begin{align}
f_\text{AB}(A\cup B)&=f_\text{AB}(A_1,A_2,\dots,B_1,B_2,\dots)=0\\
\end{align}$$
Thus concludes the 0th law of thermodynamics.
The equilibrium between 2 objects can be mathematically represented as:
$$\begin{align}
\theta_A(A_1,A_2,\dots)=\theta_B(B_1,B_2,\dots)
\end{align}$$
Where $\theta_A$ and $\theta_B$ are functions that depend only on their respective system.
System C is no longer need to describe the equilibrium of $A$ and $B$.
These are isotherms since the temperature doesn't change along the surface this spans.

> Temperature arises from the transitivity, but why just 1 parameter?
> How do we know it's just 1 temperature analogue and not a set of independent values that all follow that constraint? Can we prove that or is it taken by empirical observation?

This function is a property of the system, akin to a 3-way measurement of mass on a scale.
We would like to relate Temperature to the other coordinates of the system.


### Ideal Gas Scale
Since we want to give a number to Temperature, we can use the Ideal Gas Scale.
This is very common in physics, so we'll use it as an example.
$$\begin{align}
PV=Nk_BT
\end{align}$$
Ideal gases have the property that:
$$\begin{align}
\lim_{V\rightarrow\infty} PV=\lim_{P\rightarrow0} PV=\text{Constant}
\end{align}$$
For real life cases, we use the following:
$$\begin{align}
T^\circ(K)&=273.16\dfrac{\lim_{V\rightarrow\infty} (PV)_\text{system}}{\lim_{V\rightarrow\infty} (PV)_{\text{Triple Point of }H_2O}}
\end{align}$$
### 1st Law of Thermodynamics
If the state of an otherwise adiabatic isolated system is changed by work, the amount of work is only a function of initial and final points.
The system is conservative, meaning it is path-dependent through coordinate space.
$$\begin{align}
\Delta W\equiv E(\vec{x}_f)-E(\vec{x}_i)
\end{align}$$
Where $W$ is work, $E$ is energy, and $\vec{x}_i,\vec{x}_f$ are abstract coordinates of the system.
With diathermic walls (allow heat exchange), this is not conserved:
$$\begin{align}
\Delta W\not\equiv E(\vec{x}_f)-E(\vec{x}_i)
\end{align}$$
To account for the energy, we create a new parameter Heat:
$$\begin{align}
\Delta Q\equiv (E_f-E_i) - \Delta W
\end{align}$$
Systems that are adiabatic are like laws of motion from Newtonian mechanics, where they are idealizations of our system (like $F=ma$ of a point particle).

In differential form:
$$\begin{align}
dE(\vec{x})&=\text{d}W+\text{d}Q
\end{align}$$
Since $E$ is a function of state, it depends on where you are in parameter space, we write $d$.
Since $W$ and $Q$ are dependent on path, we write $\text{d}$.
Both versions are derivatives, but talk about two different senses of the word.

**Quasistatic:** Slow (enough) to maintain equilibrium under dynamical transforms.
When done in this way, we can be very certain where we are in coordinate space, and so we can calculate the path-dependent work correctly.
$$\begin{align}
\text{d}W&=\sum_iJ_i \ dx_i
\end{align}$$
Where $J_i$ is a generalized force and $x_i$ is a generalized displacement in coordinate space.

| System | $x_i$                     | $J_i$                      |
| ------ | ------------------------- | -------------------------- |
| Wire   | $L$ (length)              | $F$ (force)                |
| Film   | $A$ (area)                | $\sigma$ (surface tension) |
| Gas    | $V$ (volume)              | $-P$ (pressure)            |
| Magnet | $\vec{M}$ (magnetization) | $\vec{B}$ (magnetic field) |
If you make the size of your system twice as big, $x_i$ get proportionally bigger:
 - Extensive (covariant)
Likewise, $J_i$ will be inversely proportional to the change:
 - Intensive (contravariant)

If we only focus on Quasistatic cases, we can always find an expression for $\text{d}W=\sum_iJ_i \ dx_i$.
We also need to include $\text{d}Q$ for the heat, so is there an analogue for $\text{d}Q$ like $\text{d}W$?

In mechanical equilibrium, force-analogues are all constant (force, pressure, etc).
In thermal equilibrium, temperature (analogues) should also be the same.

We can then conjecture that we can write $\text{d}Q$ in the form:
$$\begin{align}
\text{d}Q&=T\text{d}S
\end{align}$$
Where $S$ is something unknown as of now, but later revealed to be entropy.

### Heat Capacity
**Heat Capacity:** How much heat energy is stored per temperature?
$$\begin{align}
C_\text{path}&=\left.\dfrac{\text{d}Q}{dT}\right|_\text{path}
\end{align}$$
Since $Q$ is path-dependent, so is the heat capacity.

If I do this in a gas, there are two ways I can add heat energy.

**Constant Volume:**
$$\begin{align}
C_v&=\left(\dfrac{\text{d}Q}{dT}\right)_{V}=\left(\dfrac{\text{d}E}{dT}\right)_{V}+\left(P\dfrac{\text{d}V}{dT}\right)_{V}=\left(\dfrac{\text{d}E}{dT}\right)_{V}+0\\
\Aboxed{C_v&=\left(\dfrac{\text{d}E}{dT}\right)_{V}}
\end{align}$$
**Constant Pressure:**
$$\begin{align}
C_p&=\left(\dfrac{\text{d}Q}{dT}\right)_{P}=\left(\dfrac{\text{d}E}{dT}\right)_{P}+\left(P\dfrac{\text{d}V}{dT}\right)_{P}\\
\Aboxed{C_p&=\left(\dfrac{\text{d}E}{dT}\right)_{P}+P\left(\dfrac{\text{d}V}{dT}\right)_{P}}
\end{align}$$

### Ideal Gas Law
Suppose I have an adiabatic system with a gas that expands from a volume $V$ to a new volume $V'$.
In experiment, we see the system's temperature does not change over the process ($T_f=T_i=T$).
Since it is adiabatically isolated, and no mechanical work was done on the system:
$$\begin{align}
dE&=\text{d}W+\text{d}Q=0+0=0\implies\boxed{dE=0}
\end{align}$$
As a matter of principle, we know that $E$ is a function of pressure and volume.
Since we know, for the ideal gas, that the product of pressure and volume is proportional to temperature, we can exchange one of the variables for temperature.
$$\begin{align}
E(P,V)\equiv E(T,V)
\end{align}$$
From the heat capacities above, we can see that:
$$\begin{align}
C_p-C_v=\dfrac{PV}{T}=Nk_B
\end{align}$$
This quantity is a constant that is proportional to the number of particles.
Here, $k_B$ is also unknown as of now, but later determined to be the Boltzmann Constant.




### Post-Lecture
Is there an extensions of the carnot engine for any generalized, reverisble path in parameter space?
If so, it might offer insight like Berry Phase does in Quantum Mechanics.

work can be non-conservative, right?


Reversible Process = Conservative Potential = All poings in config space have a single potential number