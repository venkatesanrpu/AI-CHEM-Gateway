# Lesson 1


## The Schrödinger Equation


### 1.1 Quantum Chemistry


#### Quantum chemistry is a branch of chemistry that applies the principles of quantum mechanics to study the behavior of atoms, molecules, and chemical reactions at the microscopic level. It provides a theoretical framework for understanding:


#### Electronic Structure – How electrons are distributed in atoms and molecules.


#### Molecular Bonding – The nature of chemical bonds (e.g., covalent, ionic, hydrogen bonds).


#### Spectroscopy – How molecules interact with light (e.g., UV-Vis, IR, NMR).


#### Reaction Dynamics – How chemical reactions occur at the quantum level.


#### Key Methods in Quantum Chemistry:


##### Schrödinger Equation: The fundamental equation describing quantum systems.


##### Wavefunctions (Ψ): Represent the quantum state of a system.


##### Approximation Methods:


###### Hartree-Fock (HF): A mean-field approach for electron interactions.


###### Density Functional Theory (DFT): Uses electron density instead of wavefunctions (more efficient for large systems).


###### Post-Hartree-Fock Methods (e.g., MP2, CCSD(T)): Improve accuracy by accounting for electron correlation.


#### Applications:


##### Drug design (molecular interactions)


##### Materials science (semiconductors, catalysts)


##### Computational chemistry (predicting molecular properties before lab experiments)


##### Quantum chemistry bridges physics and chemistry, enabling precise predictions of molecular behavior that classical models cannot explain.


##### Would you like a deeper dive into any specific aspect?


### 1.2 Historical Background of Quantum Mechanics


#### 1.2 Historical Background of Quantum Mechanics


##### Quantum mechanics (QM) emerged in the early 20th century as physicists struggled to explain phenomena that classical physics could not. Below is a timeline of key developments:


##### 1. Pre-Quantum Foundations (Late 19th Century)


###### Blackbody Radiation Problem (1859-1900)


- Classical theory (Rayleigh-Jeans law) predicted infinite energy at short wavelengths ("ultraviolet catastrophe").

- Max Planck (1900) proposed that energy is quantized (E = hν), marking the birth of quantum theory.

###### Photoelectric Effect (1905)


- Albert Einstein explained that light behaves as discrete packets (photons), supporting Planck’s quantization idea.

##### 2. Early Quantum Theory (1910s–1920s)


###### Bohr’s Atomic Model (1913)


- Niels Bohr proposed quantized electron orbits in atoms, explaining hydrogen’s spectral lines.

- Limitations: Only worked for hydrogen-like atoms.

###### Wave-Particle Duality (1924–1927)


- Louis de Broglie (1924) suggested particles (e.g., electrons) have wave-like properties (λ = h/p).

- Davisson-Germer Experiment (1927) confirmed electron diffraction, proving wave-particle duality.

##### 3. Formal Quantum Mechanics (1925–1930s)


###### Matrix Mechanics (Werner Heisenberg, 1925)


- Used matrices to describe quantum states, leading to the uncertainty principle (1927): Δx·Δp ≥ ħ/2.

###### Wave Mechanics (Erwin Schrödinger, 1926)


- Introduced the Schrödinger equation: ĤΨ = EΨ, describing quantum systems via wavefunctions (Ψ).

###### Born’s Probability Interpretation (1926)


- Max Born proposed that |Ψ|² gives the probability density of finding a particle.

###### Dirac’s Unification (1928)


- Paul Dirac combined QM with special relativity, predicting antimatter.

##### 4. Later Developments & Quantum Chemistry (1930s–Present)


###### Hartree-Fock Method (1930s) – Early computational approach for electron orbitals.


###### Density Functional Theory (DFT, 1960s) – Walter Kohn’s method for electron density calculations.


###### Quantum Computing (1980s–Present) – Exploits superposition & entanglement for computation.


#### Impact on Chemistry


##### Quantum mechanics revolutionized chemistry by explaining:


##### Chemical bonding (valence bond theory, molecular orbitals).


##### Spectroscopy (absorption/emission of light).


##### Reaction mechanisms (transition state theory).


##### Would you like more details on any specific event or theory?


### 1.3 The Uncertainty Principle


#### 1.3 The Uncertainty Principle


##### 1. Definition & Origin


###### The Heisenberg Uncertainty Principle, formulated by Werner Heisenberg (1927), states that certain pairs of physical properties cannot be simultaneously measured with absolute precision. The most common form is:


###### [ \Delta x \cdot \Delta p \geq \frac{\hbar}{2} ]


###### where:


###### Δx = uncertainty in position


###### Δp = uncertainty in momentum


###### ħ (h-bar) = reduced Planck’s constant (ħ = h/2π ≈ 1.05 × 10⁻³⁴ J·s)


###### This implies that the more precisely you know a particle’s position, the less precisely you can know its momentum, and vice versa.


##### 2. Physical Interpretation


###### Not a measurement limitation, but a fundamental property of quantum systems.


###### Arises from wave-particle duality: A particle’s wavefunction (Ψ) cannot simultaneously be a sharp position and a sharp momentum state.


###### Analogous to Fourier transform pairs in signal processing (e.g., a short pulse in time has a broad frequency spectrum).


##### 3. Other Forms of the Uncertainty Principle


###### Energy-Time Uncertainty [ \Delta E \cdot \Delta t \geq \frac{\hbar}{2} ]


- ΔE = uncertainty in energy

- Δt = uncertainty in time

- Explains virtual particles in quantum field theory (brief violations of energy conservation).

###### Angular Momentum Uncertainty


- For quantum spins, certain components (e.g., Sₓ, Sᵧ) cannot be known simultaneously.

##### 4. Implications in Chemistry & Physics


###### Atomic orbitals: Electrons do not have well-defined orbits (Bohr model fails); instead, they occupy "fuzzy" probability clouds (|Ψ|²).


###### Molecular spectroscopy: Spectral lines have natural linewidths due to energy-time uncertainty.


###### Tunneling effect: Particles can "tunnel" through barriers (explains alpha decay, scanning tunneling microscopy).


##### 5. Common Misconceptions


###### Not due to observer effect: It’s not about measurement disturbance but intrinsic quantum behavior.


###### Not about ignorance: The uncertainty is inherent, not due to lack of knowledge.


##### 6. Thought Experiment: Heisenberg’s Microscope


###### Heisenberg imagined trying to measure an electron’s position with a photon:


###### To locate the electron precisely (small Δx), a high-energy (short λ) photon is needed.


###### But such a photon transfers momentum to the electron, increasing Δp.


###### Thus, position and momentum cannot both be known exactly.


#### Conclusion


##### The Uncertainty Principle is a cornerstone of quantum mechanics, with profound implications for chemistry (e.g., bonding, spectroscopy) and technology (e.g., quantum computing). It fundamentally limits classical determinism, replacing it with probabilistic quantum behavior.


##### Would you like a deeper discussion on its mathematical derivation or applications?


### 1.4 The Time-Dependent Schrödinger Equation


#### 1.4 The Time-Dependent Schrödinger Equation (TDSE)


##### The Time-Dependent Schrödinger Equation (TDSE) is the fundamental equation of quantum mechanics that describes how a quantum system evolves over time. It extends the static picture of the time-independent Schrödinger equation (TISE) to dynamic processes, such as chemical reactions, spectroscopy, and quantum dynamics.


#### 1. Mathematical Formulation


##### The TDSE is given by:


##### [ i\hbar \frac{\partial}{\partial t} \Psi(\mathbf{r}, t) = \hat{H} \Psi(\mathbf{r}, t) ]


##### where:


##### (\Psi(\mathbf{r}, t)) = time-dependent wavefunction (probability amplitude)


##### (\hat{H}) = Hamiltonian operator (total energy operator)


##### (i) = imaginary unit ((i = \sqrt{-1}))


##### (\hbar) = reduced Planck’s constant ((\hbar = h/2\pi))


#### 2. Key Features


##### (a) Wavefunction Evolution


###### The TDSE governs how (\Psi(\mathbf{r}, t)) changes with time.


###### Unlike classical mechanics, quantum states evolve deterministically (via the TDSE) but are probabilistic when measured (Born rule).


##### (b) Hamiltonian ((\hat{H}))


###### For a single particle in a potential (V(\mathbf{r}, t)):


###### [ \hat{H} = -\frac{\hbar^2}{2m} \nabla^2 + V(\mathbf{r}, t) ]


###### where:


###### (-\frac{\hbar^2}{2m} \nabla^2) = kinetic energy operator


###### (V(\mathbf{r}, t)) = potential energy (may be time-dependent)


##### (c) Linearity & Superposition


###### The TDSE is linear: If (\Psi_1) and (\Psi_2) are solutions, then (a\Psi_1 + b\Psi_2) is also a solution.


###### This allows quantum superposition (e.g., electron orbitals, qubits in quantum computing).


#### 3. Solutions to the TDSE


##### (a) Separation of Variables (for time-independent potentials)


###### If (\hat{H}) does not depend on time (i.e., (V(\mathbf{r}, t) = V(\mathbf{r}))), the wavefunction can be written as:


###### [ \Psi(\mathbf{r}, t) = \psi(\mathbf{r}) \cdot \phi(t) ]


###### Substituting into the TDSE gives:


###### Time-independent part (TISE): [ \hat{H} \psi(\mathbf{r}) = E \psi(\mathbf{r}) ]


###### Time-dependent part: [ \phi(t) = e^{-iEt/\hbar} ]


###### Thus, the full solution is:


###### [ \Psi(\mathbf{r}, t) = \psi(\mathbf{r}) , e^{-iEt/\hbar} ]


###### Stationary states: The probability density (|\Psi|^2) does not change with time.


###### Phase factor: The term (e^{-iEt/\hbar}) introduces a time-dependent phase oscillation.


##### (b) General Solution (Superposition of States)


###### For a general potential, the solution is a linear combination of eigenstates:


###### [ \Psi(\mathbf{r}, t) = \sum_n c_n \psi_n(\mathbf{r}) e^{-iE_n t / \hbar} ]


###### where (c_n) are coefficients determined by initial conditions.


#### 4. Applications in Chemistry


##### (a) Spectroscopy


###### Absorption/emission of light involves transitions between states, governed by TDSE.


###### Fermi’s Golden Rule predicts transition rates using time-dependent perturbation theory.


##### (b) Chemical Reaction Dynamics


###### Describes how molecular wavefunctions evolve during reactions (e.g., transition states).


##### (c) Quantum Control


###### Laser pulses can manipulate molecular states (e.g., coherent control in photochemistry).


#### 5. Comparison with Classical Mechanics


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Aspect</th>
<th>Classical Mechanics</th>
<th>Quantum Mechanics (TDSE)</th>
</tr>
</thead>
<tbody><tr>
<td>Governing Equation</td>
<td>Newton’s (F = ma)</td>
<td>Schrödinger Equation</td>
</tr>
<tr>
<td>State Description</td>
<td>Trajectory (\mathbf{r}(t))</td>
<td>Wavefunction (\Psi(\mathbf{r}, t))</td>
</tr>
<tr>
<td>Determinism</td>
<td>Exact paths</td>
<td>Probabilistic outcomes</td>
</tr>
<tr>
<td>Time Evolution</td>
<td>ODEs (Ordinary Diff. Eq.)</td>
<td>PDE (Partial Diff. Eq.)</td>
</tr>
</tbody></table></p>

#### 6. Advanced Topics


##### Time-dependent perturbation theory (for external fields, like lasers).


##### Non-Hermitian quantum mechanics (open quantum systems).


##### Numerical methods (e.g., split-operator technique for solving TDSE).


##### Conclusion


###### The TDSE is the cornerstone of quantum dynamics, essential for understanding time-dependent phenomena in chemistry, such as spectroscopy, reaction mechanisms, and quantum control. Its solutions reveal how quantum states evolve, bridging theory with experimental observations.


###### Would you like a deeper discussion on numerical methods for solving the TDSE or time-dependent perturbation theory?


### 1.5 The Time-Independent Schrödinger Equation


#### 1.5 The Time-Independent Schrödinger Equation (TISE)


##### The Time-Independent Schrödinger Equation (TISE) is a fundamental equation in quantum mechanics that describes stationary states—quantum systems with well-defined energies that do not change over time. It is derived from the time-dependent Schrödinger equation (TDSE) under the assumption that the Hamiltonian does not explicitly depend on time.


#### 1. Mathematical Formulation


##### The TISE is given by:


##### [ \hat{H} \psi(\mathbf{r}) = E \psi(\mathbf{r}) ]


##### where:


##### (\hat{H}) = Hamiltonian operator (total energy operator)


##### (\psi(\mathbf{r})) = time-independent wavefunction (eigenfunction)


##### (E) = energy eigenvalue (a constant)


##### For a single particle in a potential (V(\mathbf{r})):


##### [ \left[ -\frac{\hbar^2}{2m} \nabla^2 + V(\mathbf{r}) \right] \psi(\mathbf{r}) = E \psi(\mathbf{r}) ]


#### 2. Key Features


##### (a) Stationary States


###### Solutions to the TISE are called stationary states because their probability densities (|\psi(\mathbf{r})|^2) do not change with time.


###### The full time-dependent wavefunction is:


###### [ \Psi(\mathbf{r}, t) = \psi(\mathbf{r}) , e^{-iEt/\hbar} ]


##### (b) Quantization of Energy


###### The TISE is an eigenvalue equation, meaning it only has solutions for certain discrete (or continuous) energy values (E).


###### This leads to quantized energy levels in bound systems (e.g., electrons in atoms).


##### (c) Boundary Conditions


###### The wavefunction (\psi(\mathbf{r})) must satisfy physical constraints:


- Continuity (no jumps in (\psi) or (\nabla \psi))

- Normalizability ((\int |\psi|^2 , d\mathbf{r} < \infty) for bound states)

#### 3. Solving the TISE: Key Examples


##### (a) Particle in a 1D Box


###### Potential: (V(x) = 0) inside ([0, L]), infinite outside.


###### Solutions: [ \psi_n(x) = \sqrt{\frac{2}{L}} \sin\left( \frac{n\pi x}{L} \right), \quad E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2} ]


###### Implications:


- Quantized energy levels ((n = 1, 2, 3, \dots))

- Zero-point energy ((E_1 > 0))

##### (b) Quantum Harmonic Oscillator


###### Potential: (V(x) = \frac{1}{2} m \omega^2 x^2)


###### Solutions: Hermite polynomials (H_n(x)): [ \psi_n(x) = \left( \frac{m\omega}{\pi \hbar} \right)^{1/4} \frac{1}{\sqrt{2^n n!}} H_n\left( \sqrt{\frac{m\omega}{\hbar}} x \right) e^{-m\omega x^2 / 2\hbar} ] [ E_n = \left( n + \frac{1}{2} \right) \hbar \omega ]


###### Implications:


- Equally spaced energy levels

- Ground state has nonzero energy ((E_0 = \frac{1}{2}\hbar \omega))

##### (c) Hydrogen Atom (Coulomb Potential)


###### Potential: (V(r) = -\frac{e^2}{4\pi \epsilon_0 r})


###### Solutions:


- Radial part: Laguerre polynomials

- Angular part: Spherical harmonics (Y_{lm}(\theta, \phi))

- Energies: [ E_n = -\frac{13.6 , \text{eV}}{n^2} \quad (n = 1, 2, 3, \dots) ]

#### 4. Physical Interpretation


##### Eigenfunctions (\psi(\mathbf{r})) represent standing waves of probability amplitude.


##### Eigenvalues (E) correspond to allowed energy levels (discrete for bound states, continuous for scattering states).


##### Superposition principle: Any state can be written as a sum of eigenstates: [ \Psi(\mathbf{r}, t) = \sum_n c_n \psi_n(\mathbf{r}) e^{-iE_n t / \hbar} ]


#### 5. Applications in Chemistry


##### (a) Atomic & Molecular Orbitals


###### Solutions to the TISE give electron wavefunctions (e.g., (1s, 2p) orbitals).


###### Explains chemical bonding (e.g., hybridization, molecular orbital theory).


##### (b) Spectroscopy


###### Energy differences ((E_n - E_m)) determine absorption/emission frequencies: [ \Delta E = h\nu ]


##### (c) Quantum Tunneling


###### Even in classically forbidden regions ((E < V)), (\psi(x)) can be nonzero (e.g., alpha decay, scanning tunneling microscopy).


#### 6. Comparison with TDSE


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Aspect</th>
<th>Time-Independent (TISE)</th>
<th>Time-Dependent (TDSE)</th>
</tr>
</thead>
<tbody><tr>
<td>Equation</td>
<td>(\hat{H}\psi = E\psi)</td>
<td>(i\hbar \partial_t \Psi = \hat{H} \Psi)</td>
</tr>
<tr>
<td>Solutions</td>
<td>Stationary states (fixed (E))</td>
<td>Evolving states (time-dependent (\Psi))</td>
</tr>
<tr>
<td>Use Case</td>
<td>Equilibrium systems (atoms, molecules)</td>
<td>Dynamics (reactions, spectroscopy)</td>
</tr>
</tbody></table></p>

#### 7. Advanced Topics


##### Perturbation theory (for small changes in potential).


##### Variational method (approximate ground-state energies).


##### WKB approximation (semiclassical limit).


##### Conclusion


###### The TISE is essential for understanding quantized energy levels in atoms, molecules, and solids. Its solutions form the basis for quantum chemistry, spectroscopy, and materials science.


###### Would you like a deeper dive into perturbation theory or numerical methods for solving the TISE?


### 1.6 Probability


#### 1.6 Probability in Quantum Mechanics


##### In quantum mechanics, probability plays a central role because the theory does not predict exact outcomes but rather probability distributions for measurements. The probabilistic nature arises from the wavefunction (\Psi(\mathbf{r}, t)), which encodes all information about a quantum system.


#### 1. Born’s Rule: Probability Density


##### The Born interpretation (1926) states that:


##### [ P(\mathbf{r}, t) = |\Psi(\mathbf{r}, t)|^2 ]


##### (P(\mathbf{r}, t)) is the probability density of finding the particle at position (\mathbf{r}) at time (t).


##### For normalized wavefunctions: [ \int_{-\infty}^{\infty} |\Psi(\mathbf{r}, t)|^2 , d^3\mathbf{r} = 1 ] (Ensures total probability = 1.)


##### Example: Particle in a Box


###### For (\psi_n(x) = \sqrt{\frac{2}{L}} \sin\left( \frac{n\pi x}{L} \right)), the probability density is: [ P_n(x) = \frac{2}{L} \sin^2\left( \frac{n\pi x}{L} \right) ]


###### Peaks correspond to higher likelihood of finding the particle.


#### 2. Expectation Values (Quantum Averages)


##### Since exact positions/momenta are uncertain, we compute expectation values (statistical averages):


##### (a) Position Expectation Value


###### [ \langle x \rangle = \int_{-\infty}^{\infty} \Psi^*(x,t) , x , \Psi(x,t) , dx ]


##### (b) Momentum Expectation Value


###### [ \langle p \rangle = \int_{-\infty}^{\infty} \Psi^*(x,t) \left( -i\hbar \frac{\partial}{\partial x} \right) \Psi(x,t) , dx ]


##### (c) General Observable (\hat{A})


###### For any operator (\hat{A}): [ \langle A \rangle = \int \Psi^* \hat{A} \Psi , d^3\mathbf{r} ]


##### Example: Harmonic Oscillator Ground State


###### For (\psi_0(x) = \left( \frac{m\omega}{\pi \hbar} \right)^{1/4} e^{-m\omega x^2 / 2\hbar}):


###### (\langle x \rangle = 0) (symmetric wavefunction)


###### (\langle p \rangle = 0) (no net momentum)


#### 3. Uncertainty Principle


##### Heisenberg’s Uncertainty Principle states:


##### [ \sigma_x \sigma_p \geq \frac{\hbar}{2} ]


##### where:


##### (\sigma_x = \sqrt{\langle x^2 \rangle - \langle x \rangle^2}) (position uncertainty)


##### (\sigma_p = \sqrt{\langle p^2 \rangle - \langle p \rangle^2}) (momentum uncertainty)


##### Example: Gaussian Wavepacket


###### A Gaussian (\Psi(x)) minimizes (\sigma_x \sigma_p = \hbar/2).


#### 4. Probability Current (Conservation of Probability)


##### The probability current density (\mathbf{J}) ensures probability is conserved:


##### [ \mathbf{J}(\mathbf{r}, t) = \frac{\hbar}{2mi} \left( \Psi^* \nabla \Psi - \Psi \nabla \Psi^* \right) ]


##### Continuity equation: [ \frac{\partial P}{\partial t} + \nabla \cdot \mathbf{J} = 0 ] (Ensures no probability is lost.)


##### Example: Free Particle


###### For (\Psi(x,t) = A e^{i(kx - \omega t)}): [ J = \frac{\hbar k}{m} |A|^2 = v |A|^2 ] (Probability flows with velocity (v = \hbar k / m).)


#### 5. Tunneling (Nonzero Probability in Classically Forbidden Regions)


##### In quantum mechanics, particles can tunnel through barriers where (E < V):


##### Transmission probability depends on barrier width and height.


##### Example: Alpha decay, scanning tunneling microscope (STM).


#### 6. Measurement & Collapse of the Wavefunction


##### When a measurement is made, (\Psi) collapses to an eigenstate of the observable.


##### Example: Measuring position collapses (\Psi) to a delta function (\delta(x - x_0)).


#### 7. Summary of Key Points


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Concept</th>
<th>Mathematical Form</th>
<th>Physical Meaning</th>
</tr>
</thead>
<tbody><tr>
<td>Probability Density</td>
<td>(P =</td>
<td>\Psi</td>
</tr>
<tr>
<td>Expectation Value</td>
<td>(\langle A \rangle = \int \Psi^* \hat{A} \Psi , d^3\mathbf{r})</td>
<td>Quantum average of observable (A)</td>
</tr>
<tr>
<td>Uncertainty Principle</td>
<td>(\sigma_x \sigma_p \geq \hbar/2)</td>
<td>Fundamental limit on simultaneous precision</td>
</tr>
<tr>
<td>Probability Current</td>
<td>(\mathbf{J} = \frac{\hbar}{2mi} (\Psi^* \nabla \Psi - \Psi \nabla \Psi^*))</td>
<td>Flow of probability</td>
</tr>
</tbody></table></p>

##### Conclusion


###### Probability in quantum mechanics is fundamental—unlike classical mechanics, we can only predict likelihoods, not certainties. This leads to phenomena like quantum tunneling, energy quantization, and wavefunction collapse.


###### Would you like a deeper dive into quantum measurement theory or numerical methods for computing probabilities?


### 1.7 Complex Numbers


#### 1.7 Complex Numbers in Quantum Chemistry


##### Quantum mechanics relies heavily on complex numbers because the wavefunction (\Psi(\mathbf{r}, t)) is generally a complex-valued function. Understanding complex numbers is essential for solving quantum problems, interpreting wavefunctions, and computing probabilities.


#### 1. Why Complex Numbers in Quantum Mechanics?


##### Wavefunctions are complex: (\Psi = \text{Re}(\Psi) + i \text{Im}(\Psi))


##### Superposition principle: Quantum states can be added like waves (interference effects).


##### Phase matters: The relative phase between quantum states affects probabilities (e.g., in interference experiments).


#### 2. Basics of Complex Numbers


##### A complex number (z) is written as: [ z = a + ib ] where:


##### (a = \text{Re}(z)) (real part)


##### (b = \text{Im}(z)) (imaginary part)


##### (i = \sqrt{-1}) (imaginary unit)


##### Key Operations


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Operation</th>
<th>Formula</th>
<th>Example</th>
</tr>
</thead>
<tbody><tr>
<td>Addition</td>
<td>((a+ib) + (c+id) = (a+c) + i(b+d))</td>
<td>((3+2i) + (1-4i) = 4 - 2i)</td>
</tr>
<tr>
<td>Multiplication</td>
<td>((a+ib)(c+id) = (ac - bd) + i(ad + bc))</td>
<td>((1+i)(1-i) = 1 - i^2 = 2)</td>
</tr>
<tr>
<td>Complex Conjugate</td>
<td>(z^* = a - ib)</td>
<td>((3+4i)^* = 3-4i)</td>
</tr>
<tr>
<td>Modulus (Magnitude)</td>
<td>(</td>
<td>z</td>
</tr>
<tr>
<td>Phase (Argument)</td>
<td>(\theta = \tan^{-1}(b/a))</td>
<td>(\text{arg}(1+i) = \pi/4)</td>
</tr>
</tbody></table></p>

##### Polar Form (Euler’s Formula)


###### [ z = |z| e^{i\theta} = |z| (\cos \theta + i \sin \theta) ]


###### Useful for describing wave phases in quantum mechanics.


#### 3. Complex Numbers in Quantum Mechanics


##### (a) Wavefunctions are Complex


###### The time-dependent Schrödinger equation: [ i\hbar \frac{\partial \Psi}{\partial t} = \hat{H} \Psi ] (The (i) ensures wavefunction evolution is unitary, preserving probability.)


###### Stationary states: (\Psi_n(\mathbf{r}, t) = \psi_n(\mathbf{r}) e^{-iE_n t / \hbar})


- The phase factor (e^{-iE_n t / \hbar}) is crucial for time evolution.

##### (b) Probability Amplitude & Interference


###### The probability density is: [ P(\mathbf{r}, t) = |\Psi(\mathbf{r}, t)|^2 = \Psi^* \Psi ]


###### Superposition of states: [ \Psi = c_1 \psi_1 + c_2 \psi_2 ]


- The relative phase between (c_1) and (c_2) affects interference.

##### (c) Expectation Values & Operators


###### Hermitian operators (e.g., (\hat{x}, \hat{p})) have real eigenvalues.


###### Momentum operator: [ \hat{p} = -i\hbar \frac{\partial}{\partial x} ] (The (i) ensures (\hat{p}) is Hermitian.)


#### 4. Examples in Quantum Chemistry


##### (a) Particle in a Box (Complex Solutions)


###### General solution: [ \Psi_n(x,t) = \sqrt{\frac{2}{L}} \sin\left( \frac{n\pi x}{L} \right) e^{-iE_n t / \hbar} ]


- The time-dependent phase is complex.

##### (b) Hydrogen Atom Wavefunctions


###### The radial and angular parts involve complex spherical harmonics: [ Y_l^m(\theta, \phi) = (-1)^m \sqrt{\frac{(2l+1)}{4\pi} \frac{(l-m)!}{(l+m)!}} P_l^m(\cos \theta) e^{im\phi} ] (The (e^{im\phi}) term introduces complex phases.)


##### (c) Quantum Tunneling (Complex Transmission Coefficient)


###### For a barrier (V_0 > E), the wavefunction in the barrier region is: [ \psi(x) = A e^{-\kappa x} + B e^{\kappa x}, \quad \kappa = \sqrt{\frac{2m(V_0 - E)}{\hbar^2}} ]


- The transmission probability involves complex amplitudes.

#### 5. Summary of Key Concepts


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Concept</th>
<th>Role in Quantum Chemistry</th>
</tr>
</thead>
<tbody><tr>
<td>Complex Wavefunction</td>
<td>(\Psi(\mathbf{r}, t)) is generally complex-valued.</td>
</tr>
<tr>
<td>Probability Density</td>
<td>(P =</td>
</tr>
<tr>
<td>Phase Factor</td>
<td>(e^{i\theta}) governs time evolution &amp; interference.</td>
</tr>
<tr>
<td>Hermitian Operators</td>
<td>Ensure real eigenvalues (observable quantities).</td>
</tr>
<tr>
<td>Spherical Harmonics</td>
<td>Angular part of atomic orbitals is complex.</td>
</tr>
</tbody></table></p>

#### 6. Practical Tips for Quantum Chemistry


##### Normalization: Always check (\int |\Psi|^2 , d^3\mathbf{r} = 1).


##### Complex Conjugates: When computing expectation values, use (\langle A \rangle = \int \Psi^* \hat{A} \Psi , d^3\mathbf{r}).


##### Phase Cancellation: Relative phases affect interference (e.g., in diffraction experiments).


##### Conclusion


###### Complex numbers are essential in quantum chemistry because:


###### They describe wave-like behavior (interference, superposition).


###### They encode phase information (time evolution, probability amplitudes).


###### They ensure Hermitian operators yield real measurable quantities.


###### Would you like a deeper dive into complex algebra in quantum problems or numerical methods for complex wavefunctions?


### 1.8 Units


#### 1.8 Units in Quantum Mechanics


##### Quantum mechanics introduces fundamental constants that define natural scales for energy, length, time, and other physical quantities. Choosing appropriate units simplifies calculations and provides deeper insight into quantum systems.


#### 1. Fundamental Constants in Quantum Mechanics


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Constant</th>
<th>Symbol</th>
<th>Value (SI Units)</th>
<th>Significance</th>
</tr>
</thead>
<tbody><tr>
<td>Planck’s constant</td>
<td>( h )</td>
<td>( 6.626 \times 10^{-34} , \text{J} \cdot \text{s} )</td>
<td>Quantum of action</td>
</tr>
<tr>
<td>Reduced Planck’s constant</td>
<td>( \hbar = h/2\pi )</td>
<td>( 1.054 \times 10^{-34} , \text{J} \cdot \text{s} )</td>
<td>Appears in Schrödinger’s equation</td>
</tr>
<tr>
<td>Speed of light</td>
<td>( c )</td>
<td>( 2.998 \times 10^8 , \text{m/s} )</td>
<td>Relates energy and mass ((E=mc^2))</td>
</tr>
<tr>
<td>Electron mass</td>
<td>( m_e )</td>
<td>( 9.109 \times 10^{-31} , \text{kg} )</td>
<td>Mass scale in atomic physics</td>
</tr>
<tr>
<td>Elementary charge</td>
<td>( e )</td>
<td>( 1.602 \times 10^{-19} , \text{C} )</td>
<td>Charge of an electron/proton</td>
</tr>
</tbody></table></p>

#### 2. Natural Units in Quantum Mechanics


##### To simplify equations, physicists often use natural units where key constants are set to 1:


##### (a) Atomic Units (a.u.)


###### Used in quantum chemistry and atomic physics.


###### Defined by: [ \hbar = 1, \quad m_e = 1, \quad e = 1, \quad 4\pi \epsilon_0 = 1 ]


###### Consequences:


- Length: Bohr radius ((a_0)) = 1 a.u. ≈ (5.29 \times 10^{-11} , \text{m})

- Energy: Hartree ((E_h)) = 1 a.u. ≈ (27.2 , \text{eV})

- Time: ( \hbar / E_h \approx 2.42 \times 10^{-17} , \text{s} )

##### (b) Hartree Atomic Units


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Quantity</th>
<th>Atomic Unit</th>
<th>SI Equivalent</th>
</tr>
</thead>
<tbody><tr>
<td>Length</td>
<td>(a_0 = \frac{4\pi \epsilon_0 \hbar^2}{m_e e^2})</td>
<td>(5.29 \times 10^{-11} , \text{m})</td>
</tr>
<tr>
<td>Energy</td>
<td>(E_h = \frac{e^2}{4\pi \epsilon_0 a_0})</td>
<td>(4.36 \times 10^{-18} , \text{J} \approx 27.2 , \text{eV})</td>
</tr>
<tr>
<td>Time</td>
<td>(\hbar / E_h)</td>
<td>(2.42 \times 10^{-17} , \text{s})</td>
</tr>
<tr>
<td>Momentum</td>
<td>(\hbar / a_0)</td>
<td>(1.99 \times 10^{-24} , \text{kg} \cdot \text{m/s})</td>
</tr>
</tbody></table></p>

##### (c) Electron-Volts (eV)


###### Common in solid-state physics and particle physics.


###### (1 , \text{eV} = ) energy gained by an electron moving through (1 , \text{V}).


###### (1 , \text{eV} \approx 1.602 \times 10^{-19} , \text{J}).


#### 3. Dimensional Analysis in Quantum Mechanics


##### (a) Schrödinger Equation in Different Units


###### General form: [ i\hbar \frac{\partial \Psi}{\partial t} = \left( -\frac{\hbar^2}{2m} \nabla^2 + V \right) \Psi ]


###### In atomic units ((\hbar = m_e = 1)): [ i \frac{\partial \Psi}{\partial t} = \left( -\frac{1}{2} \nabla^2 + V \right) \Psi ]


##### (b) Example: Hydrogen Atom Energy Levels


###### In SI units: [ E_n = -\frac{m_e e^4}{8 \epsilon_0^2 h^2 n^2} ]


###### In atomic units: [ E_n = -\frac{1}{2n^2} , \text{a.u.} ]


###### In eV: [ E_n \approx -\frac{13.6 , \text{eV}}{n^2} ]


#### 4. Practical Unit Conversions


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Quantity</th>
<th>SI Unit</th>
<th>Atomic Unit (a.u.)</th>
<th>eV</th>
</tr>
</thead>
<tbody><tr>
<td>Length</td>
<td>(1 , \text{m})</td>
<td>(1.89 \times 10^{10} , a_0)</td>
<td>—</td>
</tr>
<tr>
<td>Energy</td>
<td>(1 , \text{J})</td>
<td>(2.29 \times 10^{17} , E_h)</td>
<td>(6.24 \times 10^{18} , \text{eV})</td>
</tr>
<tr>
<td>Time</td>
<td>(1 , \text{s})</td>
<td>(4.13 \times 10^{16} , \hbar / E_h)</td>
<td>—</td>
</tr>
<tr>
<td>Electric Field</td>
<td>(1 , \text{V/m})</td>
<td>(1.94 \times 10^{-12} , \text{a.u.})</td>
<td>—</td>
</tr>
</tbody></table></p>

#### 5. Summary of Key Points


##### Atomic units (a.u.) simplify quantum equations by setting (\hbar = m_e = e = 1).


##### Hartree energy ((E_h)) is the natural energy scale in atomic systems (~27.2 eV).


##### Electron-volts (eV) are convenient for energy scales in condensed matter and particle physics.


##### Dimensional analysis helps convert between different unit systems.


##### Conclusion


###### Understanding units in quantum mechanics is crucial for:


###### Simplifying equations (e.g., Schrödinger equation in a.u.).


###### Comparing experimental results with theory.


###### Transitioning between different fields (e.g., chemistry vs. particle physics).


###### Would you like examples of unit conversions in quantum problems or a deeper look into natural units in relativistic QM?


### 1.9 Calculus


#### 1.9 Importance of Calculus in Quantum Mechanics


##### Calculus is the mathematical foundation of quantum mechanics (QM). Nearly every key concept—from wavefunctions to operators and Schrödinger’s equation—relies on differential and integral calculus. Below, we explore its critical role in QM.


#### 1. Key Areas Where Calculus is Essential


##### (a) Wavefunctions and Probability


###### The wavefunction ( \Psi(x,t) ) describes a quantum state.


###### Probability density: ( |\Psi(x,t)|^2 ) requires integration over space: [ \int_{-\infty}^{\infty} |\Psi(x,t)|^2 , dx = 1 \quad \text{(Normalization)} ]


###### Expectation values (e.g., position, momentum) involve integrals: [ \langle x \rangle = \int \Psi^*(x,t) , x , \Psi(x,t) , dx ]


##### (b) Schrödinger Equation (Differential Calculus)


###### The time-dependent Schrödinger equation: [ i\hbar \frac{\partial \Psi}{\partial t} = \hat{H} \Psi ] requires solving partial differential equations (PDEs).


###### The time-independent Schrödinger equation: [ -\frac{\hbar^2}{2m} \frac{d^2 \psi}{dx^2} + V(x) \psi = E \psi ] is a second-order ordinary differential equation (ODE).


##### (c) Operators and Eigenvalue Problems


###### Momentum operator: ( \hat{p} = -i\hbar \frac{\partial}{\partial x} ) (derivative-based).


###### Hamiltonian operator: ( \hat{H} = -\frac{\hbar^2}{2m} \nabla^2 + V(x) ) (Laplacian (\nabla^2) involves second derivatives).


###### Solving ( \hat{H} \psi = E \psi ) requires eigenvalue techniques from calculus.


##### (d) Fourier Transforms and Momentum Space


###### The position-momentum relationship is governed by Fourier transforms: [ \phi(p) = \frac{1}{\sqrt{2\pi \hbar}} \int_{-\infty}^{\infty} \psi(x) e^{-ipx/\hbar} , dx ] (Requires integral calculus).


##### (e) Perturbation Theory and Variational Methods


###### Time-independent perturbation theory uses Taylor series expansions.


###### The variational principle involves minimizing energy functionals: [ E[\psi] = \frac{\langle \psi | \hat{H} | \psi \rangle}{\langle \psi | \psi \rangle} ] (Calculus of variations).


#### 2. Practical Examples


##### (a) Particle in a Box


###### Solve the Schrödinger equation: [ -\frac{\hbar^2}{2m} \frac{d^2 \psi}{dx^2} = E \psi ] with boundary conditions ( \psi(0) = \psi(L) = 0 ).


###### Solution: [ \psi_n(x) = \sqrt{\frac{2}{L}} \sin\left( \frac{n\pi x}{L} \right), \quad E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2} ] (Requires solving ODEs and normalization integrals).


##### (b) Quantum Harmonic Oscillator


###### Hamiltonian: [ \hat{H} = -\frac{\hbar^2}{2m} \frac{d^2}{dx^2} + \frac{1}{2} m \omega^2 x^2 ]


###### Solutions involve Hermite polynomials (derived via power series methods).


##### (c) Hydrogen Atom (Radial Equation)


###### The radial Schrödinger equation: [ -\frac{\hbar^2}{2m} \frac{d^2 u}{dr^2} + \left[ \frac{\ell(\ell+1)\hbar^2}{2mr^2} - \frac{e^2}{4\pi \epsilon_0 r} \right] u = Eu ] is solved using series solutions (calculus-based techniques).


#### 3. Advanced Topics Requiring Calculus


<p><style>table{border-collapse:collapse;display:block;width:100%;word-break:keep-all; font-size:10pt;font-family: "Microsoft YaHei","Meiryo UI","Malgun Gothic","Segoe UI";}table th{font-weight:bold;}table th,table td{padding:6px 13px;border:1px solid #ddd;}table tr{background-color:#fff;border-top:1px solid #ccc;}table thead tr{background-color:#F8F8F8;text-align:left;}</style><table>
<thead>
<tr>
<th>Topic</th>
<th>Calculus Used</th>
</tr>
</thead>
<tbody><tr>
<td>Path Integrals (Feynman)</td>
<td>Functional integrals</td>
</tr>
<tr>
<td>Scattering Theory</td>
<td>Partial wave analysis (Legendre polynomials)</td>
</tr>
<tr>
<td>Density Matrices</td>
<td>Trace operations (linear algebra + calculus)</td>
</tr>
<tr>
<td>Quantum Field Theory (QFT)</td>
<td>Functional derivatives, Green’s functions</td>
</tr>
</tbody></table></p>

#### 4. Why is Calculus Indispensable?


##### Describes continuous change (wavefunction evolution).


##### Solves eigenvalue problems (energy levels, orbitals).


##### Connects position and momentum (Fourier transforms).


##### Enables approximations (perturbation theory, variational methods).


##### Conclusion


###### Without calculus, quantum mechanics would lack:


###### The Schrödinger equation (PDEs).


###### Probability interpretations (integrals).


###### Operator formalism (derivatives).


###### Advanced methods (perturbation theory, path integrals).


###### Would you like a deeper dive into a specific topic (e.g., solving the hydrogen atom with calculus)?


### Summary


#### Summary of the Schrödinger Equation


##### The Schrödinger equation is the fundamental equation of quantum mechanics, describing how quantum systems evolve over time.


##### 1. Time-Dependent Schrödinger Equation (TDSE)


###### [ i\hbar \frac{\partial \Psi(\mathbf{r}, t)}{\partial t} = \hat{H} \Psi(\mathbf{r}, t) ]


###### (\Psi(\mathbf{r}, t)): Wavefunction (contains all quantum state information).


###### (\hat{H}): Hamiltonian operator (total energy: kinetic + potential).


###### (i\hbar \frac{\partial}{\partial t}): Time evolution operator.


##### 2. Time-Independent Schrödinger Equation (TISE)


###### For stationary states (constant energy (E)): [ \hat{H} \psi(\mathbf{r}) = E \psi(\mathbf{r}) ]


###### (\psi(\mathbf{r})): Spatial part of the wavefunction.


###### Solutions: Give quantized energy levels (eigenvalues) and wavefunctions (eigenstates).


##### 3. Key Features


###### Wave-Particle Duality: Describes particles as wave-like entities.


###### Probability Interpretation: (|\Psi|^2) gives the probability density.


###### Quantization: Naturally leads to discrete energy levels (e.g., atoms).


##### 4. Applications


###### Particle in a Box (quantized energies).


###### Harmonic Oscillator (quantized vibrations).


###### Hydrogen Atom (electron orbitals).


##### 5. Importance


###### Foundation for all non-relativistic quantum mechanics.


###### Essential for understanding atoms, molecules, and solids.


###### Would you like a specific example (e.g., solving for a free particle)?


