# Lesson 2


## The Particle in a Box


### 2.1 Differential Equations


#### 2.1 Differential Equations in Quantum Mechanics


##### Differential equations (DEs) are the backbone of quantum mechanics, governing the behavior of wavefunctions and quantum systems. The Schrödinger equation itself is a differential equation, and solving it requires techniques from both ordinary (ODE) and partial (PDE) differential equations.


#### 1. Types of Differential Equations in QM


##### (a) Ordinary Differential Equations (ODEs)


###### Time-Independent Schrödinger Equation (TISE): [ -\frac{\hbar^2}{2m} \frac{d^2 \psi}{dx^2} + V(x) \psi(x) = E \psi(x) ]


- A second-order linear ODE.

- Solutions give quantized energy levels (E_n) and stationary states (\psi_n(x)).

###### Examples:


- Particle in a box.

- Quantum harmonic oscillator.

- Hydrogen atom (radial equation).

##### (b) Partial Differential Equations (PDEs)


###### Time-Dependent Schrödinger Equation (TDSE): [ i\hbar \frac{\partial \Psi(x,t)}{\partial t} = \left( -\frac{\hbar^2}{2m} \frac{\partial^2}{\partial x^2} + V(x) \right) \Psi(x,t) ]


- A linear PDE in (x) and (t).

- Describes wavefunction evolution over time.

###### Examples:


- Wave packet dynamics.

- Scattering problems.

#### 2. Key Solution Techniques


##### (a) Separation of Variables


###### Used to convert PDEs into ODEs.


###### Example: Solving the TDSE by assuming (\Psi(x,t) = \psi(x) \phi(t)).


##### (b) Power Series Solutions


###### Used for potentials like the quantum harmonic oscillator.


###### Leads to solutions in terms of Hermite polynomials.


##### (c) Frobenius Method


###### Solves ODEs with singular points (e.g., hydrogen atom radial equation).


###### Yields Laguerre polynomials for bound states.


##### (d) Green’s Functions & Integral Transforms


###### Used in scattering theory and perturbation theory.


###### Fourier transforms convert between position and momentum space.


#### 3. Importance in Quantum Mechanics


##### Quantization of Energy → Solutions to ODEs give discrete energy levels.


##### Wavefunction Evolution → PDEs describe how (\Psi(x,t)) changes over time.


##### Operators as Differential Equations → Momentum ((\hat{p} = -i\hbar \frac{\partial}{\partial x})) and Hamiltonian ((\hat{H})) involve derivatives.


##### Boundary Conditions Matter → Only certain solutions (eigenfunctions) are physically allowed.


#### 4. Example: Particle in a 1D Box


##### TISE: [ -\frac{\hbar^2}{2m} \frac{d^2 \psi}{dx^2} = E \psi ] General Solution: [ \psi(x) = A \sin(kx) + B \cos(kx) ] Boundary Conditions: (\psi(0) = \psi(L) = 0) → Quantized (k = \frac{n\pi}{L}). Final Solution: [ \psi_n(x) = \sqrt{\frac{2}{L}} \sin\left( \frac{n\pi x}{L} \right), \quad E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2} ]


##### (A simple ODE with profound quantum implications!)


##### Conclusion


###### ODEs → Quantized states (TISE).


###### PDEs → Time evolution (TDSE).


###### Differential operators → Fundamental to QM formalism.


###### Would you like a deeper dive into a specific DE technique (e.g., Frobenius method for hydrogen atom)?


### 2.2 Particle in a One-Dimensional Box


#### 2.2 Particle in a One-Dimensional Box


##### 1. Introduction


###### The particle in a 1D box (or infinite potential well) is one of the simplest quantum mechanical systems, yet it illustrates key concepts like quantization of energy, wavefunctions, and boundary conditions.


#### 2. The Setup


##### A particle of mass ( m ) is confined in a box of length ( L ) with infinite potential barriers at ( x = 0 ) and ( x = L ).


##### Potential Function: [ V(x) = \begin{cases} 0 & \text{if } 0 < x < L, \ \infty & \text{otherwise.} \end{cases} ]


##### Boundary Conditions:


###### ( \psi(0) = 0 ) (wavefunction must vanish at walls).


###### ( \psi(L) = 0 ).


#### 3. Solving the Schrödinger Equation


##### (a) Time-Independent Schrödinger Equation (TISE)


###### Inside the box (( V = 0 )): [ -\frac{\hbar^2}{2m} \frac{d^2 \psi}{dx^2} = E \psi ] Rewriting: [ \frac{d^2 \psi}{dx^2} + k^2 \psi = 0, \quad \text{where } k = \sqrt{\frac{2mE}{\hbar^2}} ]


##### (b) General Solution


###### The differential equation has solutions: [ \psi(x) = A \sin(kx) + B \cos(kx) ]


##### (c) Applying Boundary Conditions


###### At ( x = 0 ): [ \psi(0) = B = 0 \implies \psi(x) = A \sin(kx) ]


###### At ( x = L ): [ \psi(L) = A \sin(kL) = 0 ] For non-trivial solutions, ( \sin(kL) = 0 ), so: [ kL = n\pi \quad (n = 1, 2, 3, \dots) ] Thus, ( k = \frac{n\pi}{L} ).


##### (d) Quantized Energy Levels


###### From ( k = \sqrt{\frac{2mE}{\hbar^2}} ), we get: [ E_n = \frac{\hbar^2 k^2}{2m} = \frac{n^2 \pi^2 \hbar^2}{2mL^2} ]


###### Energy is quantized (only certain discrete values allowed).


###### The lowest energy (( n=1 )) is called the ground state energy.


##### (e) Normalized Wavefunctions


###### Using normalization ( \int_0^L |\psi(x)|^2 dx = 1 ): [ \psi_n(x) = \sqrt{\frac{2}{L}} \sin\left( \frac{n\pi x}{L} \right) ]


#### 4. Key Observations


##### (a) Wavefunction Properties


###### Nodes: The ( n )-th state has ( (n-1) ) nodes (points where ( \psi(x) = 0 )).


###### Orthogonality: Different states are orthogonal: [ \int_0^L \psi_n(x) \psi_m(x) , dx = \delta_{nm} ]


##### (b) Energy Spectrum


###### ( E_n \propto n^2 ) → Higher ( n ) means much larger energy gaps.


###### Zero-Point Energy: Even the ground state (( n=1 )) has non-zero energy (( E_1 = \frac{\pi^2 \hbar^2}{2mL^2} )).


##### (c) Classical vs Quantum Behavior


###### Classical: Particle can have any energy.


###### Quantum: Only discrete energies allowed.


#### 5. Applications & Extensions


##### Model for electrons in quantum dots.


##### Basis for understanding more complex potentials.


##### Extension to 2D/3D boxes (quantum wells, quantum dots).


#### 6. Summary of Results


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Property</th>
<th>Expression</th>
</tr>
</thead>
<tbody><tr>
<td>Wavefunction</td>
<td>( \psi_n(x) = \sqrt{\frac{2}{L}} \sin\left( \frac{n\pi x}{L} \right) )</td>
</tr>
<tr>
<td>Energy Levels</td>
<td>( E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2} )</td>
</tr>
<tr>
<td>Zero-Point Energy</td>
<td>( E_1 = \frac{\pi^2 \hbar^2}{2mL^2} )</td>
</tr>
<tr>
<td>Number of Nodes</td>
<td>( n-1 )</td>
</tr>
</tbody></table></p>

##### Conclusion


###### The particle in a 1D box demonstrates: ✅ Quantization of energy (discrete ( E_n )). ✅ Wave-particle duality (standing wave solutions). ✅ Importance of boundary conditions (only certain ( \psi_n ) allowed).


###### Would you like an extension to a 2D/3D box or a finite potential well?


### 2.3 The Free Particle in One Dimension


#### 2.3 The Free Particle in One Dimension


##### 1. Introduction


###### A free particle in quantum mechanics is one that experiences no potential (( V(x) = 0 )) and is not confined. Unlike the particle in a box, its energy spectrum is continuous, and its wavefunctions are plane waves.


#### 2. The Schrödinger Equation for a Free Particle


##### (a) Time-Independent Schrödinger Equation (TISE)


###### Since ( V(x) = 0 ), the equation becomes: [ -\frac{\hbar^2}{2m} \frac{d^2 \psi}{dx^2} = E \psi ] Rewriting: [ \frac{d^2 \psi}{dx^2} + k^2 \psi = 0, \quad \text{where } k = \sqrt{\frac{2mE}{\hbar^2}} ] This is the same as the classical wave equation, with solutions: [ \psi(x) = A e^{ikx} + B e^{-ikx} ]


##### (b) Physical Interpretation


###### ( e^{ikx} ) → A wave moving to the right (positive ( x )-direction).


###### ( e^{-ikx} ) → A wave moving to the left (negative ( x )-direction).


##### (c) Energy Spectrum


###### Since ( k ) can take any real value, the energy is continuous: [ E = \frac{\hbar^2 k^2}{2m} ]


###### No quantization (unlike the particle in a box).


###### All ( E \geq 0 ) are allowed.


#### 3. Wavefunction Properties


##### (a) Plane Waves and Momentum Eigenstates


###### The wavefunction ( \psi(x) = e^{ikx} ) is an eigenstate of momentum: [ \hat{p} \psi = -i\hbar \frac{d}{dx} \left( e^{ikx} \right) = \hbar k \psi ] Thus, the momentum eigenvalue is ( p = \hbar k ).


##### (b) Non-Normalizability


###### The free-particle wavefunction is not normalizable in the usual sense: [ \int_{-\infty}^{\infty} |\psi(x)|^2 , dx = \infty ]


###### Solution: Use wave packets (superpositions of plane waves) for physically realizable states.


##### (c) Wave Packets & Dispersion


###### A localized free particle is described by a wave packet: [ \Psi(x,t) = \int_{-\infty}^{\infty} \phi(k) e^{i(kx - \omega t)} , dk ] where ( \omega = \frac{\hbar k^2}{2m} ) (dispersion relation).


###### Over time, the wave packet spreads out due to dispersion.


#### 4. Comparison with Classical Mechanics


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Property</th>
<th>Classical Free Particle</th>
<th>Quantum Free Particle</th>
</tr>
</thead>
<tbody><tr>
<td>Energy</td>
<td>Continuous, ( E = \frac{p^2}{2m} )</td>
<td>Continuous, ( E = \frac{\hbar^2 k^2}{2m} )</td>
</tr>
<tr>
<td>Wavefunction</td>
<td>Not applicable</td>
<td>Plane waves ( e^{ikx} ) or wave packets</td>
</tr>
<tr>
<td>Momentum</td>
<td>Exact value ( p )</td>
<td>Momentum eigenstates ( p = \hbar k )</td>
</tr>
<tr>
<td>Localization</td>
<td>Exact position ( x(t) )</td>
<td>Wave packet spreads over time</td>
</tr>
</tbody></table></p>

#### 5. Key Takeaways


##### ✅ Energy is continuous (no quantization). ✅ Momentum eigenstates are plane waves ( e^{ikx} ). ✅ Wave packets describe localized particles but spread over time. ✅ No bound states (unlike particle in a box).


#### 6. Extensions & Applications


##### Scattering problems (particle incident on a barrier).


##### Band theory in solids (electrons in periodic potentials).


##### Wave packet dynamics in quantum optics.


##### Conclusion


###### The free particle is the simplest quantum system but introduces key concepts like continuous spectra, momentum eigenstates, and wave packets.


###### Would you like to explore wave packet dynamics or scattering problems next?


### 2.4 Particle in a Rectangular Well


#### 2.4 Particle in a Rectangular Well


##### 1. Introduction


###### A particle in a rectangular well (or finite potential well) is a quantum system where a particle is confined within a region of finite potential depth. Unlike the infinite well, the particle can tunnel into classically forbidden regions, leading to quantized bound states and continuous scattering states.


#### 2. The Potential Function


##### (a) Definition of the Well


###### Consider a symmetric well of width ( L ) and depth ( V_0 ): [ V(x) = \begin{cases} -V_0 & \text{if } -L/2 < x < L/2, \ 0 & \text{otherwise.} \end{cases} ]


###### Bound states (( E < 0 )): Particle is trapped inside the well.


###### Scattering states (( E > 0 )): Particle can escape to infinity.


#### 3. Solving for Bound States (( E < 0 ))


##### (a) Time-Independent Schrödinger Equation (TISE)


###### Inside the well (( -L/2 < x < L/2 )): [ -\frac{\hbar^2}{2m} \frac{d^2 \psi}{dx^2} - V_0 \psi = E \psi ] [ \implies \frac{d^2 \psi}{dx^2} + k^2 \psi = 0, \quad \text{where } k = \sqrt{\frac{2m(E + V_0)}{\hbar^2}} ]


###### Outside the well (( |x| > L/2 )): [ \frac{d^2 \psi}{dx^2} - \kappa^2 \psi = 0, \quad \text{where } \kappa = \sqrt{\frac{-2mE}{\hbar^2}} ]


##### (b) General Solutions


###### Inside the well: [ \psi(x) = A \cos(kx) \quad (\text{even parity}) \quad \text{or} \quad B \sin(kx) \quad (\text{odd parity}) ]


###### Outside the well: [ \psi(x) = C e^{-\kappa |x|} \quad (\text{decaying exponential}) ]


##### (c) Boundary Conditions


###### Continuity of ( \psi(x) ) and ( \psi'(x) ) at ( x = \pm L/2 ).


###### Normalization: ( \int_{-\infty}^{\infty} |\psi(x)|^2 , dx = 1 ).


##### (d) Quantization Condition


###### Applying boundary conditions leads to transcendental equations for allowed energies:


###### Even states: [ k \tan\left(\frac{kL}{2}\right) = \kappa ]


###### Odd states: [ k \cot\left(\frac{kL}{2}\right) = -\kappa ]


###### These must be solved numerically or graphically.


##### (e) Number of Bound States


###### The number of bound states depends on ( V_0 ) and ( L ).


###### For a shallow well, there may be only one bound state.


###### For a deep well, multiple bound states exist.


#### 4. Solving for Scattering States (( E > 0 ))


##### (a) General Solution


###### For ( E > 0 ), the particle is not bound, and the wavefunction consists of incoming, reflected, and transmitted waves:


###### For ( x < -L/2 ): [ \psi(x) = A e^{ikx} + B e^{-ikx} ]


###### For ( -L/2 < x < L/2 ): [ \psi(x) = C e^{iqx} + D e^{-iqx}, \quad q = \sqrt{\frac{2m(E + V_0)}{\hbar^2}} ]


###### For ( x > L/2 ): [ \psi(x) = F e^{ikx} ]


##### (b) Transmission & Reflection Coefficients


###### Transmission probability (( T )): Fraction of particles that pass through the well.


###### Reflection probability (( R )): Fraction reflected back.


###### Resonances: At certain energies, ( T = 1 ) (perfect transmission).


#### 5. Key Observations


##### (a) Bound States vs. Scattering States


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Property</th>
<th>Bound States (( E &lt; 0 ))</th>
<th>Scattering States (( E &gt; 0 ))</th>
</tr>
</thead>
<tbody><tr>
<td>Energy Spectrum</td>
<td>Quantized (discrete)</td>
<td>Continuous</td>
</tr>
<tr>
<td>Wavefunction</td>
<td>Exponentially decaying outside well</td>
<td>Plane waves inside and outside</td>
</tr>
<tr>
<td>Physical Meaning</td>
<td>Localized particle</td>
<td>Free particle with partial reflection</td>
</tr>
</tbody></table></p>

##### (b) Tunneling Effect


###### Even for ( E < V_0 ), there is a non-zero probability of finding the particle outside the well.


###### This is impossible classically but allowed in QM.


##### (c) Comparison with Infinite Well


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Feature</th>
<th>Infinite Well</th>
<th>Finite Well</th>
</tr>
</thead>
<tbody><tr>
<td>Energy Levels</td>
<td>( E_n \propto n^2 )</td>
<td>Fewer, lower energies</td>
</tr>
<tr>
<td>Wavefunction at Boundaries</td>
<td>Zero at walls</td>
<td>Exponentially decaying</td>
</tr>
<tr>
<td>Number of States</td>
<td>Infinite</td>
<td>Finite (depends on ( V_0 ))</td>
</tr>
</tbody></table></p>

#### 6. Applications


##### Quantum dots (artificial atoms).


##### Nuclear physics (alpha decay via tunneling).


##### Semiconductor heterostructures (electron confinement).


#### 7. Summary of Results


##### Bound States (( E < 0 ))


###### Wavefunctions:


- Even: ( \psi(x) = A \cos(kx) ) inside, ( C e^{-\kappa |x|} ) outside.

- Odd: ( \psi(x) = B \sin(kx) ) inside, ( C e^{-\kappa |x|} ) outside.

###### Quantization: Solved via ( k \tan(kL/2) = \kappa ) (even) or ( k \cot(kL/2) = -\kappa ) (odd).


##### Scattering States (( E > 0 ))


###### Transmission/Reflection: Depends on energy and well depth.


##### Conclusion


###### The finite well combines quantization, tunneling, and scattering, making it a fundamental model in quantum mechanics.


###### Would you like numerical examples or a deeper dive into tunneling?


### 2.5 Tunneling


#### 2.5 Quantum Tunneling


##### 1. Introduction


###### Quantum tunneling is a phenomenon where a particle passes through a classically forbidden region (where ( E < V(x) )). This is impossible in classical mechanics but allowed in quantum mechanics due to the wave-like nature of particles.


###### Key Examples:


###### Alpha decay (nucleus emits an alpha particle despite Coulomb barrier).


###### Scanning tunneling microscopes (STM) (electrons tunnel across a vacuum gap).


###### Semiconductor devices (tunneling diodes).


#### 2. The Rectangular Barrier Problem


##### (a) Potential Definition


###### Consider a barrier of height ( V_0 ) and width ( L ): [ V(x) = \begin{cases} 0 & \text{if } x < 0 \quad (\text{Region I}), \ V_0 & \text{if } 0 \leq x \leq L \quad (\text{Region II}), \ 0 & \text{if } x > L \quad (\text{Region III}). \end{cases} ]


##### (b) Cases of Interest


###### ( E > V_0 ) → Classical transmission (not tunneling).


###### ( E < V_0 ) → Quantum tunneling occurs.


#### 3. Solving the Tunneling Problem (( E < V_0 ))


##### (a) Time-Independent Schrödinger Equation (TISE)


###### Region I (Incident + Reflected Wave): [ \psi_I(x) = A e^{ikx} + B e^{-ikx}, \quad k = \sqrt{\frac{2mE}{\hbar^2}} ]


###### Region II (Exponential Decay/Growth): [ \psi_{II}(x) = C e^{\kappa x} + D e^{-\kappa x}, \quad \kappa = \sqrt{\frac{2m(V_0 - E)}{\hbar^2}} ]


###### Region III (Transmitted Wave): [ \psi_{III}(x) = F e^{ikx} ]


##### (b) Boundary Conditions


###### Continuity of ( \psi(x) ) and ( \psi'(x) ) at ( x = 0 ) and ( x = L ).


###### No left-moving wave in Region III (( D = 0 )).


##### (c) Transmission Probability (( T ))


###### After solving, we get: [ T = \left| \frac{F}{A} \right|^2 = \frac{1}{1 + \frac{V_0^2 \sinh^2(\kappa L)}{4E(V_0 - E)}} ] For thick barriers (( \kappa L \gg 1 )), this simplifies to: [ T \approx \frac{16E(V_0 - E)}{V_0^2} e^{-2\kappa L} ] Key Observations:


###### ( T ) decreases exponentially with barrier width ( L ).


###### ( T ) decreases exponentially with ( \sqrt{V_0 - E} ).


#### 4. Applications of Tunneling


##### (a) Alpha Decay


###### Nucleus emits an alpha particle despite Coulomb repulsion.


###### Gamow’s theory explains decay rates via tunneling.


##### (b) Scanning Tunneling Microscope (STM)


###### A sharp tip scans a surface at atomic distances.


###### Electrons tunnel between tip and sample, producing an image.


##### (c) Tunnel Diodes (Esaki Diodes)


###### Semiconductor device exploiting tunneling for negative resistance.


###### Used in high-speed electronics.


#### 5. Key Concepts


##### (a) Wavefunction Penetration


###### Even in forbidden regions (( E < V_0 )), ( \psi(x) \neq 0 ).


###### The wavefunction decays exponentially inside the barrier.


##### (b) Comparison with Classical Mechanics


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Aspect</th>
<th>Classical Mechanics</th>
<th>Quantum Mechanics</th>
</tr>
</thead>
<tbody><tr>
<td>Barrier Crossing</td>
<td>Impossible if ( E &lt; V_0 )</td>
<td>Possible (tunneling)</td>
</tr>
<tr>
<td>Transmission</td>
<td>( T = 0 ) if ( E &lt; V_0 )</td>
<td>( T &gt; 0 )</td>
</tr>
</tbody></table></p>

##### (c) WKB Approximation (Advanced Topic)


###### Used for non-rectangular barriers (e.g., Coulomb barrier).


###### Transmission probability: [ T \approx e^{-2 \int_{x_1}^{x_2} \kappa(x) , dx}, \quad \kappa(x) = \sqrt{\frac{2m(V(x) - E)}{\hbar^2}} ]


#### 6. Summary of Results


##### Tunneling occurs when ( E < V_0 ).


##### Transmission probability ( T ) decays exponentially with barrier width.


##### Applications: Nuclear physics (alpha decay), STM, semiconductor devices.


##### Conclusion


###### Quantum tunneling is a uniquely quantum phenomenon with wide-ranging implications in physics and technology.


###### Would you like a numerical example or a deeper discussion on the WKB method?


### Summary


#### Summary of Key Topics in the Workbench on Quantum Tunneling


##### Introduction to Quantum Tunneling


###### A quantum phenomenon where a particle passes through a classically forbidden potential barrier ((E < V_0)).


###### Examples: Alpha decay, scanning tunneling microscopes (STM), tunnel diodes.


##### Rectangular Barrier Problem


###### Potential Definition: A barrier of height (V_0) and width (L).


###### Two Cases:


- (E > V_0) → Classical transmission.

- (E < V_0) → Quantum tunneling.

##### Mathematical Solution of Tunneling


###### Wavefunctions in Different Regions:


- Incident + reflected wave (Region I).

- Exponentially decaying/growing wave (Region II).

- Transmitted wave (Region III).

###### Transmission Probability ((T)):


- Exact solution: (T = \left| \frac{F}{A} \right|^2).

- For thick barriers ((\kappa L \gg 1)): (T \approx e^{-2\kappa L}).

##### Applications of Tunneling


###### Alpha Decay: Nuclei emit alpha particles despite Coulomb barrier.


###### STM: Electrons tunnel between a tip and a surface, enabling atomic-scale imaging.


###### Tunnel Diodes: Semiconductor devices using tunneling for high-speed electronics.


##### Key Concepts & Comparisons


###### Wavefunction Penetration: Non-zero probability inside the barrier.


###### Classical vs. Quantum:


- Classical: No transmission if (E < V_0).

- Quantum: Non-zero transmission via tunneling.

###### WKB Approximation (Advanced): Estimates tunneling probability for arbitrary barriers.


##### Conclusion


###### Tunneling is a fundamental quantum effect with critical applications in nuclear physics, nanotechnology, and electronics.


#### Final Remarks


##### This workbench covers the theory, mathematical treatment, and real-world applications of quantum tunneling. If you need further details on numerical examples or the WKB method, let me know!


