



> I've always wondered if there's a reason why there are 3 types of leptons (and in a way quarks too) and happen to have 3 dimensions of space As if Leptons and Quarks are geometric objects in Space, instead of just random particles. Obvy this would be disproved if we found Gen IV particles but we've yet to find them




### Particle Types as Geometric Quantities
There seems to be 2 kinds of transforms:
 - Duality (Leptons & Quarks, Particles & Antiparticles, etc.)
 - Ternality (particle basis being any 3 linearly-independent vectors)

### Guiding Idea
Typical particle physics distinguishes Ternality of particles by *flavor*, however I seek deeper meaning, and postulate that the 3 flavors arise from the geometric 3D space.


### Ternality: Particle Basis
If the bases of particles is formed in a geometric way as cartesian space tends to be, we can represent these particles as *tensors*, where our typical notion of the Standard Model particles are the "cartesian" equivalent of the basis.

Let's define an arbitrary particle of the following types:
$$\begin{align}
\ket{\tilde e_i}&=a_{i1}\ket{e^-}+a_{i2}\ket{\mu^-}+a_{i3}\ket{\tau^-} && \text{(Charged Leptons)}\\
\ket{\tilde \nu_i}&=a_{i1}\ket{\bar\nu_e}+a_{i2}\ket{\bar\nu_\mu}+a_{i3}\ket{\bar\nu_\tau} && \text{(Neutrinos)}\\
\ket{\tilde u_i}&=a_{i1}\ket{q_u}+a_{i2}\ket{q_c}+a_{i3}\ket{q_t} && \text{(Upper Quarks)}\\
\ket{\tilde d_i}&=b_{i1}\ket{q_d}+b_{i2}\ket{q_s}+b_{i3}\ket{q_b} && \text{(Lower Quarks)}
\end{align}$$





### Operators
We define the *generation* operator to be the following:
$$\begin{align}
G^\dagger\ket{\tilde{e}_i}&=\dfrac{a_{i1}}{\sqrt{a_{i1}^2+a_{i2}^2}}\ket{\mu^-}+\dfrac{a_{i2}}{\sqrt{a_{i1}^2+a_{i2}^2}}\ket{\tau^-}\\
G\ket{\tilde{e}_i}&=\dfrac{a_{i2}}{\sqrt{a_{i2}^2+a_{i3}^2}}\ket{e^-}+\dfrac{a_{i3}}{\sqrt{a_{i2}^2+a_{i3}^2}}\ket{\mu^-}\\
\end{align}$$







### Observations
For Left-chiral, fermions, we can see that:

| Particle               | Charge | Weak Isospin | Hypercharge |
| ---------------------- | ------ | ------------ | ----------- |
| Left Lepton            | -1     | -1/2         | -1          |
| Left Anti-Lepton       | +1     | +1/2         | +1          |
| Left Neutrino          | 0      | +1/2         | -1          |
| Left Anti-Neutrino     | 0      | -1/2         | +1          |
| Right Lepton           | -1     | 0            | -2          |
| Right Anti-Lepton      | +1     | 0            | +2          |
| Right Neutrino         | 0      | 0            | 0           |
| Right Anti-Neutrino    | 0      | 0            | 0           |
| ---                    |        |              |             |
| Left Upper Quark       | +2/3   | +1/2         | +1/3        |
| Left Upper Anti-Quark  | -2/3   | -1/2         | -1/3        |
| Left Lower Quark       | -1/3   | -1/2         | +1/3        |
| Left Lower Anti-Quark  | +1/3   | +1/2         | -1/3        |
| Right Upper Quark      | +2/3   | 0            | +4/3        |
| Right Upper Anti-Quark | -2/3   | 0            | -4/3        |
| Right Lower Quark      | -1/3   | 0            | +2/3        |
| Right Lower Anti-Quark | +1/3   | 0            | -2/3        |























### Duality Operators
Suppose we want to convert between the different kind of duals of the particles.

The first and most trivial is the Hermitian conjugate for Anti-Particle (charge):
$$\begin{align}
\ket{\tilde e_i}^\dagger&=\bra{\tilde e_i}
\end{align}$$
We can define the Lepton Duality operator as:
$$\begin{align}
D_L\ket{\tilde e_i}=\ket{\tilde \nu_i}\iff D_L^{-1}\ket{\tilde \nu_i}=\ket{\tilde e_i}
\end{align}$$
We can define the Quark Duality operator as:
$$\begin{align}
D_Q\ket{\tilde u_i}=\ket{\tilde d_i}\iff D_Q^{-1}\ket{\tilde d_i}=\ket{\tilde u_i}
\end{align}$$
And finally, we can define the Particle Duality operator as:
$$\begin{align}
D_P\ket{\tilde u_i}=\ket{\tilde e_i}\iff D_P^{-1}\ket{\tilde e_i} = \ket{\tilde u_i}\\
D_P\ket{\tilde d_i}=\ket{\tilde \nu_i}\iff D_P^{-1}\ket{\tilde \nu_i} = \ket{\tilde d_i}
\end{align}$$
#### Properties
We want these properties to apply in such a way that they physically realistic.
$$\begin{align}
D_Q^{-1}D_P^{-1}D_LD_P&=\mathbb{I}
\end{align}$$



### Tensor Products?
Lets define Hadrons as:
$$\begin{align}
H_{uuu}&=\ket{\tilde u_i}\otimes\ket{\tilde u_j}\otimes\ket{\tilde u_k}\\
H_{uud}&=\ket{\tilde u_i}\otimes\ket{\tilde u_j}\otimes\ket{\tilde d_k}\\
H_{udd}&=\ket{\tilde u_i}\otimes\ket{\tilde d_j}\otimes\ket{\tilde d_k}\\
H_{ddd}&=\ket{\tilde d_i}\otimes\ket{\tilde d_j}\otimes\ket{\tilde d_k}\\
\end{align}$$
We can then see that the Neutron Decay is a process such that:
$$\begin{align}
D: H_{udd}\rightarrow H_{uud}
\end{align}$$
Because reactions can always be reversed through time, we see that:
$$\begin{align}
D^{-1}D&=1
\end{align}$$

Such a decay can be modeled as:
$$\begin{align}
D(H_{udd})=H_{uud}+W^-
\end{align}$$
Which is general for any kind of Hadron of that form. Others also exist.






### Types of Duality
Electric Charge
Quark Upness or Downness
Lepton Chargeness
Spin














### Utilizing Equations
New operators:
$$\begin{align}
R\ket{\tilde{u}_i}&=\ket{\tilde{d}_i}\\
R\ket{\tilde{e}_i}&=\bra{\tilde{e}_i}\\
\end{align}$$


Maybe Neutron Decay?
$$\begin{align}
\left(\ket{\tilde u_j}+\ket{\tilde d_k}\right)+\ket{\tilde d_i}&=\left(\ket{\tilde u_j}+\ket{\tilde d_k}\right)+\ket{\tilde u_i}+\ket{\tilde e_i}+\ket{\tilde\nu_i}
\end{align}$$

$$\begin{align}
R\ket{\tilde d_i}&=\ket{\tilde u_i}+\ket{\tilde e_i}+\ket{\tilde\nu_i}
\end{align}$$











Maybe Neutron Decay?
$$\begin{align}
\ket{\tilde d_i}&=\ket{\tilde u_i}+\ket{\tilde e_i}+\ket{\tilde\nu_i}
\end{align}$$
The reverse of this is Proton fusion:
$$\begin{align}
D_Q\ket{\tilde d_i}&=D_Q\ket{\tilde u_i}+D_Q\ket{\tilde e_i}+D_Q\ket{\tilde\nu_i}\\
\ket{\tilde u_i}&=\ket{\tilde d_i}+C\ket{\tilde e_i}+C\ket{\tilde\nu_i}\\
\end{align}$$









For the Leptons, we can write the following:

Where $\ket{\tilde e_i}$ and $\ket{\tilde \nu_i}$ are *particle duals*.

For the Quarks, we can write the following:
$$\begin{align}

\end{align}$$
Where $\ket{\tilde u_i}$ and $\ket{\tilde d_i}$ are *particle duals*.

Note: There is also some sense of the leptons and quarks being duals of each other.







