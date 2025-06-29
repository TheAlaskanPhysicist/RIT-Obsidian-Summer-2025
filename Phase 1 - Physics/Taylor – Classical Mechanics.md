
Pg. 312



### Compendium
Time is absolute (in classical mechanics).


Newton's first law: $\vec{F}^\text{net}=0\implies\dfrac{d\vec{p}}{dt}=0$.
> Conservation of linear momentum
> Definition of *inertial reference frame*

Newton's second law: $\vec{F}^\text{net}=\dfrac{d\vec{p}}{dt}$. 
> Force-Momentum relation
> Valid in inertial reference frames

Newton's third law: $\vec{F}_\text{int}^\text{net}=0\implies \vec{F}^\text{net}=\vec{F}_\text{ext}^\text{net}=\dfrac{d\vec{p}}{dt}$.
> Internally, momentum is conserved.
> All reciprocal forces are equal and opposite.

Angular first law: $\vec{\tau}^\text{net}=0\implies\dfrac{d\vec{l}}{dt}=0$
> Conservation of angular momentum
> Valid in inertial reference frames

Angular second law: $\vec{\tau}^\text{net}=\dfrac{d\vec{l}}{dt}$. 
> Torque-Angular Momentum relation

Angular third law: $\vec{\tau}_\text{int}^\text{net}=0\implies \vec{\tau}^\text{net}=\vec{\tau}_\text{ext}^\text{net}=\dfrac{d\vec{l}}{dt}$.
> Internally, momentum is conserved.
> All reciprocal torques are equal and opposite (in rigid-body systems).

Conservation of Energy: $\oint\vec{F}\cdot d\vec{r}=0 \iff \vec\nabla\times\vec{F}=0$
 > In all systems that are conservative (path-independent).
 > $\vec{F}=-\vec\nabla U$.

Principle of Stationary Action:
For a conservative field $L$, the path that extremizes action takes the form:
$$\begin{align}
L(q_1,\dot{q}_1,q_2,\dot{q}_2,\dots,q_n,\dot{q}_n)&=L\\
\dfrac{\partial L}{\partial q_i}-\dfrac{d}{dt}\dfrac{\partial L}{\partial\dot{q}_i}&=0
\end{align}$$
> Are there extensions to further derivatives? What happens in non-cartesian space?
> Does this work with Fourier Duals, or just with the derivatives.



The Lagrangian takes $L=T-V$ for unconstrained motion (any path through parameter space).
$$\begin{align}
S=\int_{t_1}^{t_2}L\ dt
\end{align}$$
Particles travel the path of stationary action (Hamilton's principle)
$$\begin{align}
q_i&:\text{(Generalized Coordinate)}\\
\dfrac{\partial L}{\partial q_i}&:\text{(Generalized Force)}\\
\dfrac{\partial L}{\partial\dot{q}_i}&:\text{(Generalized Momentum)}
\end{align}$$
If a system has the same number of DOF as generalized coordinates, it's said to be *holonomic*.
Constraint forces do not have to be conservative, only non-constraint forces do.

If the Lagrangian is independent of a coordinate $q_i$, the corresponding generalized momentum is conserved. This is called Noether's Theorem.

Why? Suppose we have the Euler-Lagrange Equations:
$$\begin{align}
\dfrac{\partial L}{\partial q_i}-\dfrac{d}{dt}\dfrac{\partial L}{\partial\dot{q}_i}&=0
\end{align}$$
If the generalized force is 0 in the $q_i$ coordinate direction, then:
$$\begin{align}
\dfrac{d}{dt}\dfrac{\partial L}{\partial\dot{q}_i}&=0&&\implies&\dfrac{\partial L}{\partial\dot{q}_i}&=\text{Constant}
\end{align}$$
So we see the generalized momentum is conserved.

Translational Invariance $\implies$ Conservation of Momentum
Time Independence $\implies$ Conservation of Energy/Hamiltonian


#### Lagrangian Non-Uniqueness
Suppose I have a Lagrangian $L$ that satisfies the Euler-Lagrange equations:
$$\begin{align}
\dfrac{\partial L}{\partial q_i}-\dfrac{d}{dt}\dfrac{\partial L}{\partial\dot{q}_i}&=0
\end{align}$$
Let there be a function $f(x,\dot{x})$ that also satisfies the Euler-Lagrange equations:
$$\begin{align}
\dfrac{\partial f}{\partial q_i}-\dfrac{d}{dt}\dfrac{\partial f}{\partial\dot{q}_i}&\equiv0
\end{align}$$
Then $L'=L+f$ must also satisfy the Euler-Lagrange equations.
This is similar to gauge freedom in electromagnetism.


#### Lagrangian with constraints
Let $f$ be a constraint function of dependent variables. Then:
$$\begin{align}
\dfrac{\partial L}{\partial q_i}+\lambda(t)\dfrac{\partial f}{\partial q_i}-\dfrac{d}{dt}\dfrac{\partial L}{\partial\dot{q}_i}&\equiv0
\end{align}$$
Where $f$ is:
$$\begin{align}
f(q_1,q_2,\dots,q_n)&=\text{const}
\end{align}$$
This applies for any constraints, including multiple functions with multiple constraints.
Therefore, the generalized version would take the following form:
$$\begin{align}
\dfrac{\partial L}{\partial q_i}+\sum_k\lambda_k(t)\dfrac{\partial f_k}{\partial q_i}-\dfrac{d}{dt}\dfrac{\partial L}{\partial\dot{q}_i}&\equiv0
\end{align}$$
I think this looks very similar to the idea of the sum of internal forces (Langrangian forces) and external forces (Constraint forces) is equal to the rate change of momentum.



Centrifugal potential... (is there a Coriolis potential?)











### Calculus of Variations
Let $f$ be a function that extremizes the functional equation:
$$\begin{align}
S[f]=\int_{a}^{b}L(x,f(x),f'(x))\ dx
\end{align}$$
Consider a perturbation $f\rightarrow f+\epsilon\eta$. where $\eta(a)=\eta(b)=0$ Then we have:
$$\begin{align}
S[f+\epsilon\eta]&=\int_{a}^{b}L(x,f(x)+\epsilon\eta(x),f'(x)+\epsilon\eta'(x))\ dx\\
\dfrac{d}{d\epsilon}S[f+\epsilon\eta]
&=\dfrac{d}{d\epsilon}\int_{a}^{b}L(x,f(x)+\epsilon\eta(x),f'(x)+\epsilon\eta'(x))\ dx\\
&=\int_{a}^{b}\left(\eta(x)\dfrac{\partial L}{\partial f}+\eta'(x)\dfrac{\partial L}{\partial f'}\right)\ dx\\
&=\int_{a}^{b}\eta(x)\left(\dfrac{\partial L}{\partial f}-\dfrac{d}{dx}\dfrac{\partial L}{\partial f'}\right)\ dx+\left.\eta(x)\dfrac{\partial L}{\partial f'}\right|_a^b\\
\Aboxed{0&=\dfrac{\partial L}{\partial f}-\dfrac{d}{dx}\dfrac{\partial L}{\partial f'}}
\end{align}$$

The reason why we talk about "stationary action" instead of minima, is because if you have a finite system that wraps around on itself, the shortest path between 2 points actually becomes 2 different lines. Both are "minima" but one of them isn't truly a minimum, just a local minimum. Extend that to a box becoming infinitely big, the line directly away from point B from point A is technically satisfied in the equation for stationary action.








6.2
6.3
6.4
(pg.230)

All chapter 7





Moments of mass:
$$\begin{align}
\vec{R}\int dm&=\int \vec{r}\ dm && \text{(Center of Mass)}\\
\end{align}$$













### Quantities
We assume no changing of basis vectors (for undergraduate)
$$\begin{align}
\vec{r}&=r^ie_i && \text{(Position)}\\
\vec{v}&=\dfrac{dr^i}{dt}e_i && \text{(Velocity)}\\
\vec{a}&=\dfrac{d^2r^i}{dt^2}e_i && \text{(Accleration)}\\
\vec{p}&=m\vec{v} && \text{(Momentum)}\\
\vec{F}&=m\vec{a} && \text{(Force)}\\
\vec{l}&=\vec{r}\times\vec{p} && \text{(Angular Momentum)}\\
\vec{\tau}&=\vec{r}\times\vec{F} && \text{(Torque)}\\
T&=\dfrac{1}{2}m\vec{v}^2 && \text{(Kinetic Energy)}\\
\end{align}$$

### Newton's First Law
In the absence of forces, a point particle moves with constant velocity $\vec{v}$.
> This only applies in Inertial Reference Frames
### Newton's Second Law
For any point particle of mass $m$, the net force $\vec{F}$ on the particle is always equal to the mass time acceleration of the particle's acceleration.
> This only applies in Inertial Reference Frames
### Newton's Third Law
The generation of forces must always come in pairs of equal and opposite value.
> This leads directly to the conservation of momentum.


No external forces $\implies$ Conserved momentum (over time).

Forces are "real," Potentials are not.
This is similar to $\vec{E}$ and $\vec{B}$ being "real," but $\phi$ and $\vec{A}$ are not.


Moments of mass:
$$\begin{align}
M\vec{R}&=\int \vec{r}\ dm && \text{(Center of Mass)}\\
\end{align}$$

Linear Momentum is conserved (in inertial frames)
Angular Momentum is conserved (in inertial frames)
Is there a true total momentum conserved (in inertial frames)?

Path Independence <-> Conserved
There will a unique "potential" for it if it's conserved.

$$\begin{align}
\vec{F}&=-\vec\nabla U
\end{align}$$
Central forces = Spherically-symmetric forces


For non-conservative systems: Use sums of forces in a differential equation.
For conservative systems: Use Euler-Lagrange equations.



pg 236

