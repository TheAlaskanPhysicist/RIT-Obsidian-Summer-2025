Stanley Goodwin, 6/7/2025

# Supplemental Framework on Relative Motion and Curvature in Generalized Reference Frames
This document develops a geometric, observer-centric framework to describe motion and dynamical quantities in curved spacetime without relying on traditional 4-vector formalism. All physical measurements are made by an external observer (EXT) of a pointlike internal system (INT), enabling a consistent, covariant treatment of velocity, acceleration, and tidal effects, even in the absence of global symmetries. The framework is designed to be pedagogically clear while remaining mathematically precise and will later serve as the foundation for a more general information-theoretic formulation of dynamics.

---
## Assumptions and Conventions
In this document, we assume the following to simplify the mathematical framework while maintaining physical rigor:
 - The metric tensor satisfies $$g_{ij}(x^k,t)=\braket{e_i|e_j}\iff g_{ij}(x^k,t)=g^*_{ji}(x^k,t) \iff g^\dagger(x^k,t)=g(x^k,t)$$ ensuring the metric is Hermitian (this is for any potential for complex numbers)

 - The basis vectors $e_i(x^k,t)$ are smooth functions of space and time.

---
## Physical Quantities
### Position Vectors
We define the particle’s position vector relative to each observer’s frame as:
$$\begin{align}
\Aboxed{\vec{r}_\text{int}&=r^ie_i} & 
r^i&=r^i\left(\vec{x}(t),t\right) &
e_i&=e_i\left(\vec{x}(t),t\right)
&& \text{(Internal Position)}\\
\Aboxed{\vec{\mathrm{r}}_\text{ext}&=\mathrm{r}^i\mathrm{e}_i} & \mathrm{r}^i&=\mathrm{r}^i\left(\vec{\mathrm{x}}(\mathrm{t}), \mathrm{t}\right) & \mathrm{e}_i&=\mathrm{e}_i\left(\vec{\mathrm{x}}(\mathrm{t}), \mathrm{t}\right)
&& \text{(External Position)}\\
\end{align}$$
All quantities relating to measurements of the EXT body will always have their variable wrapped in `\mathrm{}`, while quantities relating to the INT body will be italicized.

Each observer defines their own metric tensor via the inner product of basis vectors:
$$\begin{align}
g_{ij}=g_{ij}\left(\vec{x}(t),t\right)&=e_i\cdot e_j && \text{(Internal Metric)}\\
\mathrm{g}_{ij}=\mathrm{g}_{ij}\left(\vec{\mathrm{x}}(\mathrm{t}),\mathrm{t}\right)&=\mathrm{e}_i\cdot\mathrm{e}_j && \text{(External Metric)}\\
\end{align}$$
Each frame also can measure infinitesimal changes position as:
$$\begin{align}
\Aboxed{d\vec{r}_\text{int}&=\dfrac{d\vec{r}_\text{int}}{dt}dt}\\
\Aboxed{d\vec{\mathrm{r}}_\text{ext}&=\dfrac{d\vec{\mathrm{r}}_\text{ext}}{d\mathrm{t}}d\mathrm{t}}\\
\end{align}$$
---
### Proper Time of INT
Proper time $dt_\text{int}$ measured along the worldline of the internal observer is invariant and can be calculated from external coordinates as:
$$\begin{align}
&&dt_\text{int} &= \sqrt{\mathrm{g}_{ij}\dfrac{d\mathrm{x}^i}{d\mathrm{t}}\dfrac{d\mathrm{x}^j}{d\mathrm{t}}}\ d\mathrm{t}\\
\implies && \Delta t_\text{int} &=
\int_{\mathrm{t}_1}^{\mathrm{t}_2}\sqrt{\mathrm{g}_{ij}\dfrac{d\mathrm{x}^i}{d\mathrm{t}}\dfrac{d\mathrm{x}^j}{d\mathrm{t}}}\ d\mathrm{t}
\end{align}$$
This is the elapsed proper time experienced by INT in their own frame.

---
#### Null Trajectories and the Speed of Light
Although this framework is grounded in geometric kinematics without presupposing special relativity, we may naturally derive constraints for massless particles by demanding that they traverse **null trajectories**; that is, their motion does not accumulate proper time.

Let us consider the proper time differential experienced by the internal frame (INT), as previously defined:
$$\begin{align}
dt_\text{int} &= \sqrt{\mathrm{g}_{ij}\dfrac{d\mathrm{x}^i}{d\mathrm{t}}\dfrac{d\mathrm{x}^j}{d\mathrm{t}}}\ d\mathrm{t}
\end{align}$$
For a **massless particle**, proper time is not accumulated:
$$\begin{align}
dt_\text{int} &= 0 &\iff && \mathrm{g}_{ij}\dfrac{d\mathrm{x}^i}{d\mathrm{t}}\dfrac{d\mathrm{x}^j}{d\mathrm{t}}=0
\end{align}$$
This relation defines a **null trajectory**, meaning the worldline lies on the light cone of the external metric $\mathrm{g}_{ij}$​. Equivalently, EXT measures the squared speed of a massless particle to satisfy:
$$\begin{align}
\mathrm{v}^2&=\mathrm{g}_{ij}\dfrac{d\mathrm{x}^i}{d\mathrm{t}}\dfrac{d\mathrm{x}^j}{d\mathrm{t}}=0
\end{align}$$
Thus, we interpret the "speed of light" not as a constant scalar $c$, but as a **geometric condition**; motion along a null path with respect to the external observer’s metric. The measured speed is always constrained to be "on the light cone," regardless of curvature or coordinate representation.

This provides a geometric definition of **relativistic causality**: no influence can propagate faster than the null limit imposed by the geometry. The formalism thereby recovers the classical invariant light speed as a natural consequence of how internal time vanishes along null worldlines.

In contrast, **massive particles** obey:
$$\begin{align}
\mathrm{g}_{ij}\dfrac{d\mathrm{x}^i}{d\mathrm{t}}\dfrac{d\mathrm{x}^j}{d\mathrm{t}}>0
\end{align}$$
ensuring they remain within the light cone and experience nonzero proper time. This distinction will later guide our formulation of energy and momentum for both types of particles.

---
### Relative Motion of INT as Measured by EXT
The external observer measures the following kinematic quantities of the internal particle.
#### Linear velocity
$$\begin{align}
\mathrm{v}^i&=\dfrac{d\mathrm{x}^i}{d\mathrm{t}}
\end{align}$$
#### Angular velocity
$$\begin{align}
\omega^k=\dfrac{1}{4}\epsilon^{kij}\left(\mathrm{e}_i\cdot\dfrac{d\mathrm{e}_j}{d\mathrm{t}}-\dfrac{d\mathrm{e}_i}{d\mathrm{t}}\cdot\mathrm{e}_j\right)
\end{align}$$
#### Linear acceleration
$$\begin{align}
\mathrm{a}^i&=\dfrac{d\mathrm{v}^i}{d\mathrm{t}}+\Gamma_{jk}^i\left(\vec{\mathrm{x}}(\mathrm{t}),\mathrm{t}\right)\mathrm{v}^j\mathrm{v}^k
\end{align}$$
#### Angular acceleration
$$\begin{align}
\alpha^k=\dfrac{1}{4}\epsilon^{kij}\left(\mathrm{e}_i\cdot\dfrac{d^2\mathrm{e}_j}{d\mathrm{t}^2}-\dfrac{d^2\mathrm{e}_i}{d\mathrm{t}^2}\cdot\mathrm{e}_j\right)
\end{align}$$
---
### Tidal Forces of INT
Tidal effects are described by the Riemann curvature tensor, a geometric invariant calculated by EXT at the location of INT:
$$\begin{align}
R^i_{jkl}&=\dfrac{d\Gamma_{jl}^i}{d\mathrm{x}^k}-\dfrac{d\Gamma_{jk}^i}{d\mathrm{x}^l}+\Gamma_{km}^i\Gamma_{jl}^m-\Gamma_{lm}^i\Gamma_{jk}^m
\end{align}$$
Here, $\Gamma_{jk}^i$ are Christoffel symbols evaluated in EXT’s coordinate system.

---
### Massive Particle Dynamics
For particles with nonzero mass, we may further refine our kinematic description into one that supports dynamical quantities, such as momentum, inertia, and forces. Unlike the null case, a massive particle satisfies:
$$\begin{align}
\mathrm{g}_{ij}\dfrac{d\mathrm{x}^i}{d\mathrm{t}}\dfrac{d\mathrm{x}^j}{d\mathrm{t}}>0
\end{align}$$
which implies the particle moves strictly within the local light cone of EXT's metric.

---
#### Momentum
Let us define the **kinematic momentum** of the particle in EXT's frame as:
$$\begin{align}
\mathrm{p}^i&=m\mathrm{v}^i
\end{align}$$
where $m$ is an observer-independent scalar mass parameter, and $\mathrm{v}^i$ is the particle's velocity as measured in EXT's coordinates. This definition reflects how momentum is a projection of mass onto local velocity, **not** assumed from Newtonian axioms but emerging as a conserved quantity under geodesic motion.

To explore **momentum transport**, we differentiate:
$$\begin{align}
\dfrac{d\mathrm{p}^i}{d\mathrm{t}}&=m\left(\mathrm{a}^i-\Gamma_{jk}^i\left(\vec{\mathrm{x}}(\mathrm{t}),\mathrm{t}\right)\mathrm{v}^j\mathrm{v}^k\right)
\end{align}$$
This separates the **coordinate acceleration** from the connection-induced acceleration due to spacetime curvature. If the particle follows a geodesic, its **covariant acceleration vanishes**, i.e.:
$$\begin{align}
\dfrac{d\mathrm{p}^i}{d\mathrm{t}}&=-\Gamma_{jk}^i\left(\vec{\mathrm{x}}(\mathrm{t}),\mathrm{t}\right)\mathrm{v}^j\mathrm{v}^k
\end{align}$$
suggesting no external force acts on the particle. This equation provides a foundation for defining **forces as deviations from geodesic transport**, allowing us to later incorporate interaction models (e.g., electromagnetic or fictitious forces in non-inertial frames).

---
#### Kinetic Energy (Preliminary)
While energy has not yet been defined formally, a kinetic term naturally arises from the square of the velocity under the metric:
$$\begin{align}
T&=\dfrac{1}{2}m\mathrm{g}_{ij}\mathrm{v}^i\mathrm{v}^j
\end{align}$$
This scalar captures the “effort” associated with the particle's motion and will later serve as the basis for defining a full Lagrangian or Hamiltonian structure.

---
## Extensions and Methodological Remarks
### Extension to Particles with Mass (related to curvature)
While the formalism above applies to structureless point particles, nothing in its construction prohibits associating a scalar mass $m$ to the particle. This mass may later be used to relate the particle to gravitational effects; particularly if one seeks to calculate how the particle perturbs the ambient geometry via Einstein’s field equations.

Such an extension, however, likely falls outside the scope of conventional Quantum Field Theory unless one posits how spacetime curvature emerges from a probabilistic field description. I leave this open-ended—not to prescribe *how* such a mechanism might work, but to assert that it **must**, and the challenge is understanding *why* it does.

No assumption of momentum or energy has been made in this document, as these require additional physical structures, such as a stress-energy tensor, which are not yet introduced. The present work is restricted entirely to **geometric and kinematic quantities**.

---
### Extension to Extended Bodies (Finite Volume)
The current framework assumes the particle is point-like and without internal structure. However, the formalism generalizes naturally to continuous distributions of matter (I.e. INT with internal structure), such as fluids, elastic bodies, or fields, where the object occupies a finite volume.

In such cases, the object can be thought of as a **locally static volume with internal structure**, described by a continuum of worldlines. While spacetime remains locally smooth and approximately flat over small regions, spatial derivatives of curvature (i.e., **tidal effects**) become essential for describing how different parts of the object accelerate relative to one another.

Future work will involve defining concepts such as **rigidity, deformation, strain**, and **internal stresses** using geometric quantities. These will likely require additional field variables and evolution equations.

---
### Why This Is Not a 4-Vector Formulation
Although 4-vectors and coordinate-free tensor notation are standard in relativistic physics, this document deliberately avoids them in favor of a **frame-dependent, observer-centric formulation**.

Each observer measures:
- Their own local proper time $t$,
- Their own (potentially time-varying) spatial basis vectors $e_i(x^j,t)$,
- And particle motion **relative to their own coordinate region**.

This reflects a **physically operational perspective**: it is more natural for observers to measure rates of change with local instruments with respect to their own basis than to commit to global Lorentz-invariant objects. The mathematics remains covariant, but explicitly constructed from quantities that are meaningful _locally_ rather than from shared convention.

Additionally, I have limited formal experience with 4-vector notation as commonly used in General Relativity. My undergraduate curriculum at RIT did not include a dedicated course in GR, nor a graduate level course at RPI, so much of my exposure to relativistic physics has been self-directed. As a result, I chose to work within a more familiar and intuitive geometric language in order to articulate my ideas clearly. This choice allowed me to focus on the conceptual structure of the framework rather than on formal conventions, and I believe it provides a transparent foundation for potential advisors to engage with the physical intuition driving the project. 

This choice is aligned with the long-term objective of replacing fixed geometric structures (like 4-vectors and Lorentz transformations) with an **entirely relational and information-theoretic formulation of mechanics**: where motion is described not relative to absolute spacetime, but in terms of statistically measurable changes between observers.
