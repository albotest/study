# QUANTUM COMPUTING - EXAM NOTES (THANGLISH)

---

## PART-A (2 MARKS)

### 1. Hermitian Operators - Importance

**Definition:** Hermitian operators observable quantities represent panrom (measurement values).

**Why Important:**
1. **Real eigenvalues** - Measurement results always real numbers
2. **Orthogonal eigenvectors** - Different states distinguish pannalam
3. **Physical observables** - Energy, momentum, position represent panrom

---

### 2. Wave Nature of Light - Experimental Observation

**Observation:** **Double-slit experiment** - Light screen la interference pattern create panrum (bright & dark fringes).

**Explanation:**
- Waves constructive & destructive interference show panrum
- Particle behavior irundhaa pattern varaadhu
- Wave nature-a confirm panrudhu

---

### 3. Heisenberg Uncertainty Principle - Statement

**Statement:** "Position and momentum simultaneous-a exact-a measure panna mudiyaadhu."

**Formula:**
```
ΔxΔp ≥ ℏ/2
```

**Meaning:**
- Δx = Position uncertainty
- Δp = Momentum uncertainty
- ℏ = Reduced Planck's constant
- One accurately measure pannaa, mathadu uncertain aagum

---

### 4. Inner Product - Definition

**Definition:** Two vectors ku idaila scalar value calculate panra operation.

**Notation:** `⟨ψ|φ⟩`

**Properties:**
- Probability amplitude calculate panna use
- Orthogonality check panna
- Complex conjugate involve aagum

**Example:**
```
⟨ψ|φ⟩ = ψ₁*φ₁ + ψ₂*φ₂
```

---

### 5. Pauli Gates (Any Two)

1. **Pauli-X Gate** (NOT gate)
   - |0⟩ → |1⟩
   - |1⟩ → |0⟩

2. **Pauli-Z Gate** (Phase flip)
   - |0⟩ → |0⟩
   - |1⟩ → -|1⟩

**Other:** Pauli-Y (X + Z combination)

---

### 6. Hadamard Gate - Function

**Function:** Qubit-a equal superposition state-la convert panrum.

**Action:**
- |0⟩ → (|0⟩ + |1⟩)/√2
- |1⟩ → (|0⟩ - |1⟩)/√2

**Use:** Quantum algorithms la superposition create panna.

---

### 7. Entanglement - Definition

**Definition:** Two or more qubits strongly correlated aagi, one qubit measure pannaa mathadu instant-a affect aagura state.

**Key Point:**
- Einstein "spooky action at a distance" sonnaaru
- Classical physics la illa
- Quantum communication ku essential

**Example:** Bell state |Φ⁺⟩ = (|00⟩ + |11⟩)/√2

---

### 8. Bell States

**Definition:** Maximum-a entangled aana two-qubit states.

**Four Bell States:**
1. |Φ⁺⟩ = (|00⟩ + |11⟩)/√2
2. |Φ⁻⟩ = (|00⟩ - |11⟩)/√2
3. |Ψ⁺⟩ = (|01⟩ + |10⟩)/√2
4. |Ψ⁻⟩ = (|01⟩ - |10⟩)/√2

**Use:** Quantum teleportation, cryptography

---

### 9. Dirac Notation

**Definition:** Quantum states represent panna use panra mathematical notation (Paul Dirac create pannaru).

**Two Parts:**
- **Ket:** |ψ⟩ (Column vector - state)
- **Bra:** ⟨ψ| (Row vector - conjugate)

**Example:**
```
|ψ⟩ = α|0⟩ + β|1⟩
⟨ψ| = α*⟨0| + β*⟨1|
```

---

### 10. Ket Vector

**Definition:** Quantum state represent panra column vector (Dirac notation la).

**Notation:** |ψ⟩

**Example:**
```
|0⟩ = [1]
      [0]

|1⟩ = [0]
      [1]
```

**Meaning:** System oda state vector-a represent panrum.

---

## PART-B (13 MARKS)

### 11A. Wave-Particle Duality & Observation Effect

#### **Wave-Particle Duality Concept:**

Light and matter rendu properties-um show panrum - sometimes wave maari, sometimes particle maari behave panrum. Idhu classical physics expectations-a completely contradict panrum.

---

#### **Experimental Evidence:**

**1. Double-Slit Experiment (Wave Nature):**

**Setup:**
```
Light Source → Two Slits → Screen

Without observation:
│    │
│ S1 │  ╱╲╱╲╱╲  (Interference pattern)
│    │  ▓░▓░▓░
│ S2 │  ╲╱╲╱╲╱
│    │
```

**Results:**
- Light rendu slits through pass aagi screen la **interference fringes** form aagum
- **Bright fringes:** Constructive interference (waves reinforce)
- **Dark fringes:** Destructive interference (waves cancel)
- Idhu clear wave behavior evidence

**Why Wave Behavior:**
- Particle irundhaa two bands mattum form aagum
- Wave behavior allows interference pattern
- Path difference based on wavelength constructive/destructive decide panrum

---

**2. Photoelectric Effect (Particle Nature):**

**Observation:**
- Light metal surface-la incident aaga electrons emit aagum
- **Key finding:** Intensity increase pannaa more electrons, aana energy same
- Frequency increase pannaa electron energy increase aagum

**Einstein's Explanation:**
- Light photons (particles) la travel panrum
- Each photon energy: E = hf (h = Planck's constant, f = frequency)
- Particle nature-a confirm panrum

**Why Particle Behavior:**
- Wave theory predict panna intensity increase pannaa electron energy increase aaganum
- Aana actually frequency mattum energy decide panrum
- Discrete energy packets (quanta) particle behavior show panrum

---

**3. Compton Scattering (Particle Nature):**

- X-rays electrons-ku scatter aaga wavelength change aagum
- Particle collision maari behave panrum
- Momentum conservation follow aagum

---

#### **Effect of Observation on Interference Pattern:**

**Critical Experiment: Which-Path Detection**

**Scenario 1: No Detector (No Observation)**
```
Light → S1 → ╱╲╱╲  Interference pattern
        S2 → ╲╱╲╱
```
- Interference fringes clearly visible
- Wave nature dominate
- Photon "both slits through pass" analogy

**Scenario 2: Detector Added (Observation)**
```
Light → S1 [Detector] → │▓│  Two bands only
        S2 [Detector] → │▓│
```
- Interference pattern vanish aagum!
- Two separate bands form (particle behavior)
- Which slit-nu therindhaa wave nature collapse

---

#### **Why Observation Matters:**

**Quantum Mechanics Explanation:**

1. **Before Measurement:**
   - Photon superposition state la irukum (both paths simultaneously)
   - Wave function: |ψ⟩ = (|S1⟩ + |S2⟩)/√2
   - Interference possible

2. **After Measurement:**
   - Wave function collapse aagum
   - Definite path determined
   - |ψ⟩ → |S1⟩ OR |S2⟩
   - No more superposition, no interference

**Physical Significance:**
- Measurement process quantum state-a fundamentally disturb panrum
- Observer system interact aana instant collapse happen
- "Reality" observation based on depend panrum (philosophy)

---

#### **Complementarity Principle (Niels Bohr):**

- Wave and particle aspects **complementary**
- Rendu simultaneously exhibit panna mudiyaadhu
- Which aspect display aagum depends on experimental setup
- Example: Interference setup → wave; photoelectric setup → particle

---

#### **Modern Understanding:**

- Light neither pure wave nor pure particle
- **Quantum object** - dual nature
- Classical analogies inadequate
- Mathematics (wave function) accurately predict
- Observation fundamentally quantum reality affect panrum

---

**Summary:**
- Double-slit: Wave nature (interference)
- Photoelectric: Particle nature (quanta)
- Observation: Pattern-a collapse panrum
- Complementarity: Setup determines behavior

---

### 11B. Heisenberg Uncertainty Principle

#### **Statement & Concept:**

**Formal Statement:**
"Position and momentum of a particle simultaneous-a arbitrary accuracy-oda measure panna impossible."

**Extended Statement:**
"Any two conjugate variables (position-momentum, energy-time) ku idaila fundamental limit irukum for simultaneous precise measurement."

---

#### **Mathematical Formulation:**

**1. Position-Momentum Uncertainty:**
```
ΔxΔp ≥ ℏ/2
```

**Where:**
- Δx = Standard deviation of position (uncertainty)
- Δp = Standard deviation of momentum
- ℏ = h/2π = 1.054 × 10⁻³⁴ J·s (Reduced Planck's constant)

**Meaning:**
- Product of uncertainties minimum value irukum
- One accurately measure → other more uncertain
- Not experimental limitation, fundamental nature of reality

---

**2. Energy-Time Uncertainty:**
```
ΔEΔt ≥ ℏ/2
```

**Where:**
- ΔE = Energy uncertainty
- Δt = Time duration uncertainty

**Implication:**
- Short time la energy measurement → large uncertainty
- Virtual particles briefly exist pannalam (quantum fluctuations)

---

#### **Physical Significance:**

**1. Fundamental Limit (Not Measurement Error):**

**Classical View (Wrong):**
- Better instruments use pannaa uncertainty reduce pannalam
- Observer skill improve pannaa perfect measurement possible

**Quantum View (Correct):**
- Nature inherent property
- No instrument perfect-a measure panna help pannaadhau
- Universe fundamental behavior
- Particle exact position & momentum simultaneously "possess" panna maataadhau

---

**2. Wave-Particle Duality Connection:**

**Why Uncertainty Exists:**
- Particle wave-like nature due
- Wave → spread out (localized illa)
- Position well-defined na → wave packet narrow → wavelength uncertain → momentum uncertain
- Momentum well-defined na → plane wave (infinite spread) → position uncertain

**Mathematical Connection:**
- Position measure: Real space representation
- Momentum measure: Fourier space representation
- Fourier transform property: Narrow in one → broad in other

---

**3. Examples & Applications:**

**Example 1: Electron in Atom**
```
Electron nucleus close-a confined (small Δx)
→ High momentum uncertainty (large Δp)
→ High kinetic energy
→ Prevents collapse into nucleus
```

**Why Atoms Stable:**
- Electron nucleus-ku romba close pona → Δx very small
- Then Δp large aaganum → high speed → kinetic energy increase
- Balance maintain panni stable orbit form aagum
- Classical physics atom collapse predict panna
- Uncertainty principle stability explain panrum

---

**Example 2: Ground State Energy**
- System minimum energy (zero-point energy) endrum positive
- Complete rest impossible (that means Δp = 0, then Δx = ∞)
- Always some motion irukanum
- Example: Helium liquid state even at absolute zero (quantum effects)

---

**Example 3: Tunneling Effect**
- Particle barrier-a cross pannalam even if energy insufficient
- Energy-time uncertainty allow: ΔE = barrier height, Δt = tunneling time
- Applications: Nuclear fusion (sun), scanning tunneling microscope

---

**Example 4: Electron Microscope Limit**
```
Better resolution venum → smaller wavelength
Smaller wavelength → higher energy photons
Higher energy → sample disturb
Trade-off exist
```

---

#### **Derivation Outline (Concept):**

**Using Wave Packets:**

1. **Narrow Wave Packet** (Position well-defined):
   - Requires many wavelengths superposition
   - Range of k values (wave vector) large
   - Δk large → Δp = ℏΔk large

2. **Broad Wave Packet** (Momentum well-defined):
   - Single wavelength close-a irukum
   - Δk small → Δp small
   - But spatial extent large → Δx large

**Mathematical Result:**
```
ΔxΔk ≥ 1/2
Since p = ℏk,
ΔxΔp ≥ ℏ/2
```

---

#### **Philosophical Implications:**

**1. Determinism Breakdown:**
- Classical: Complete information → future predict
- Quantum: Complete information get panna impossible
- Indeterminacy fundamental

**2. Complementarity:**
- Position and momentum complementary observables
- Measuring one disturbs other
- Can't know both precisely

**3. Reality Nature:**
- Particle exact values "have" pannadhau illa measurement varaikum
- Probability distributions mattum exist
- Measurement process values "create" panrum (interpretation debate)

---

**Summary Table:**

| Aspect | Classical Physics | Quantum Physics |
|--------|------------------|-----------------|
| **Measurement** | Unlimited precision possible | Fundamental limit exist |
| **Cause** | Instrument limitations | Nature property |
| **Position & Momentum** | Both exact values | Trade-off mandatory |
| **Determinism** | Complete | Probabilistic |
| **Reality** | Pre-existing values | Measurement creates |

---

**Key Takeaways:**
- Not about measurement technology, nature fundamental
- Wave-particle duality mathematical expression
- Atom stability explain
- Quantum tunneling possible
- Determinism classical sense invalid
- Product ΔxΔp never zero aaga mudiyaadhu

---

### 12A. Vector Spaces in Quantum Mechanics

#### **Concept of Vector Spaces:**

**Definition:**
Vector space (or Hilbert space quantum mechanics la) collection of vectors with specific operations (addition, scalar multiplication) and properties.

**Why Quantum Mechanics:**
- Quantum states vectors-a represent pannurom
- Superposition principle naturally vectors la work aagum
- Linear algebra tools use pannalam

---

#### **Properties of Vector Space:**

**1. Vector Addition:**
- |ψ⟩ + |φ⟩ = |χ⟩ (also a valid state)
- **Physical meaning:** Superposition of states

**2. Scalar Multiplication:**
- c|ψ⟩ (c = complex number)
- **Physical meaning:** Amplitude scaling

**3. Closure:**
- Operations vector space-la mattum results produce

**4. Associativity & Commutativity:**
- (|ψ⟩ + |φ⟩) + |χ⟩ = |ψ⟩ + (|φ⟩ + |χ⟩)
- |ψ⟩ + |φ⟩ = |φ⟩ + |ψ⟩

**5. Zero Vector:**
- |0⟩ exists, |ψ⟩ + |0⟩ = |ψ⟩

---

#### **Basis & Dimension:**

**Basis Definition:**
Set of linearly independent vectors, ella vectors-ayum linear combination-a express panna use pannalam.

**Properties:**
- **Linearly independent:** No vector mathavanga combination-a write panna mudiyaadhu
- **Spanning:** Any vector basis vectors combination

---

**Dimension:**
Number of basis vectors = dimension of space

---

#### **Example 1: Two-Dimensional Qubit Space**

**Computational Basis:**
```
|0⟩ = [1]    |1⟩ = [0]
      [0]          [1]
```

**Dimension:** 2 (2D space)

**Any Qubit State:**
```
|ψ⟩ = α|0⟩ + β|1⟩
```

**Where:**
- α, β = Complex amplitudes
- |α|² + |β|² = 1 (Normalization)

**Physical Meaning:**
- |α|² = Probability of measuring |0⟩
- |β|² = Probability of measuring |1⟩
- Superposition both states simultaneously

---

**Example State:**
```
|ψ⟩ = (1/√2)|0⟩ + (1/√2)|1⟩

Probability |0⟩ = |1/√2|² = 1/2
Probability |1⟩ = |1/√2|² = 1/2
Equal superposition
```

---

#### **Example 2: Three-Dimensional System (Qutrit)**

**Basis:**
```
|0⟩ = [1]    |1⟩ = [0]    |2⟩ = [0]
      [0]          [1]          [0]
      [0]          [0]          [1]
```

**Dimension:** 3

**General State:**
```
|ψ⟩ = α|0⟩ + β|1⟩ + γ|2⟩
|α|² + |β|² + |γ|² = 1
```

**Physical System:**
- Spin-1 particle
- Three-level atom

---

#### **Example 3: Multi-Qubit Systems**

**Two Qubits:**

**Basis (Computational):**
```
|00⟩, |01⟩, |10⟩, |11⟩
```

**Dimension:** 2² = 4

**General State:**
```
|ψ⟩ = α₀₀|00⟩ + α₀₁|01⟩ + α₁₀|10⟩ + α₁₁|11⟩
```

**Normalization:**
```
|α₀₀|² + |α₀₁|² + |α₁₀|² + |α₁₁|² = 1
```

---

**Three Qubits:**
- Basis: |000⟩, |001⟩, |010⟩, ..., |111⟩
- Dimension: 2³ = 8
- 8 complex amplitudes

**General Pattern:**
- n qubits → 2ⁿ dimensional space
- 2ⁿ basis states
- Exponential growth (quantum advantage reason)

---

#### **Different Basis Choices:**

**1. Computational Basis (Z-basis):**
```
|0⟩, |1⟩
```
Standard choice, measurement la use.

---

**2. Hadamard Basis (X-basis):**
```
|+⟩ = (|0⟩ + |1⟩)/√2
|−⟩ = (|0⟩ - |1⟩)/√2
```

**Use:** Quantum algorithms, BB84 protocol

---

**3. Y-Basis:**
```
|i+⟩ = (|0⟩ + i|1⟩)/√2
|i−⟩ = (|0⟩ - i|1⟩)/√2
```

**Properties:**
- Any basis valid if orthonormal
- Basis change = Unitary transformation
- Different bases different measurement results

---

#### **Application: Quantum State Representation**

**Example: Spin-½ Particle**

**States:**
- |↑⟩ = spin up
- |↓⟩ = spin down

**General Spin State:**
```
|ψ⟩ = cos(θ/2)|↑⟩ + e^(iφ)sin(θ/2)|↓⟩
```

**Where:**
- θ = Polar angle (0 to π)
- φ = Azimuthal angle (0 to 2π)
- Bloch sphere representation

---

#### **Importance of Basis:**

**1. Measurement Outcomes:**
- Computational basis-la measure → |0⟩ or |1⟩ result
- X-basis la measure → |+⟩ or |−⟩ result
- Basis choice outcome determine panrum

**2. State Preparation:**
- Basis use panni state initialize
- Different bases different physical orientations

**3. Quantum Algorithms:**
- Basis transformations key operations
- Hadamard gate: Z-basis ↔ X-basis

---

**Summary:**
- Quantum states = Vectors in Hilbert space
- Basis = Reference frame for states
- Dimension = n qubits → 2ⁿ dimensions
- Linear combinations = Superposition
- Different bases → different perspectives
- Computational basis most common

---

### 12B. Inner Product - Role & Properties

#### **Definition of Inner Product:**

**Mathematical Definition:**
Two vectors ku idaila complex number-a calculate panra operation.

**Notation:**
```
⟨φ|ψ⟩
```

**Where:**
- ⟨φ| = bra (row vector, conjugate of |φ⟩)
- |ψ⟩ = ket (column vector)

---

**Formula (Finite Dimension):**
```
⟨φ|ψ⟩ = φ₁*ψ₁ + φ₂*ψ₂ + ... + φₙ*ψₙ
```

**Where:**
- φᵢ* = Complex conjugate of φᵢ
- Sum over all components

---

#### **Properties of Inner Product:**

**1. Linearity (Second Argument):**
```
⟨φ|(α|ψ₁⟩ + β|ψ₂⟩) = α⟨φ|ψ₁⟩ + β⟨φ|ψ₂⟩
```

**2. Conjugate Symmetry:**
```
⟨φ|ψ⟩ = ⟨ψ|φ⟩*
```

**3. Positive Definiteness:**
```
⟨ψ|ψ⟩ ≥ 0
⟨ψ|ψ⟩ = 0 iff |ψ⟩ = 0
```

---

#### **Role 1: Determining Probabilities**

**Physical Interpretation:**
Inner product probability amplitude give panrum.

**Born Rule:**
```
Probability = |⟨φ|ψ⟩|²
```

**Example:**
```
System state: |ψ⟩ = (1/√2)|0⟩ + (1/√2)|1⟩
Measure |0⟩-la: P(0) = |⟨0|ψ⟩|²

⟨0|ψ⟩ = ⟨0|(1/√2|0⟩ + 1/√2|1⟩)
      = 1/√2·⟨0|0⟩ + 1/√2·⟨0|1⟩
      = 1/√2·1 + 1/√2·0
      = 1/√2

P(0) = |1/√2|² = 1/2
```

**Physical Meaning:**
- 50% chance |0⟩ measure aagum
- 50% chance |1⟩ measure aagum

---

**General Measurement:**
State |ψ⟩-la irukum system basis state |φₙ⟩ measure panna:
```
P(φₙ) = |⟨φₙ|ψ⟩|²
```

---

#### **Role 2: Normalization**

**Normalization Condition:**
```
⟨ψ|ψ⟩ = 1
```

**Why Important:**
- Total probability = 1 aaganum
- All possible outcomes sum to 1

**Example:**
```
|ψ⟩ = α|0⟩ + β|1⟩

⟨ψ|ψ⟩ = (α*⟨0| + β*⟨1|)(α|0⟩ + β|1⟩)
      = α*α⟨0|0⟩ + α*β⟨0|1⟩ + β*α⟨1|0⟩ + β*β⟨1|1⟩
      = |α|² + |β|²

Normalization: |α|² + |β|² = 1
```

---

**Physical Significance:**
- Probability conservation
- Unitary evolution preserve panrum
- Measurement outcomes sum to 1

**Example Calculation:**
```
Given: |ψ⟩ = 3|0⟩ + 4|1⟩ (not normalized)

⟨ψ|ψ⟩ = |3|² + |4|² = 9 + 16 = 25

Normalized state:
|ψ⟩ₙ = (1/5)(3|0⟩ + 4|1⟩)
     = (3/5)|0⟩ + (4/5)|1⟩

Check: (3/5)² + (4/5)² = 9/25 + 16/25 = 1 ✓
```

---

#### **Role 3: Orthogonality**

**Orthogonal Definition:**
Two states orthogonal if:
```
⟨φ|ψ⟩ = 0
```

**Physical Meaning:**
- Distinguishable states
- Measurement la one-a detect pannaa mathadu definitely detect aagaadhu
- No overlap

---

**Example: Computational Basis**
```
⟨0|1⟩ = [1 0][0] = 0
              [1]

|0⟩ and |1⟩ orthogonal
```

**Consequence:**
- Measure |0⟩: 100% |0⟩, 0% |1⟩
- Measure |1⟩: 0% |0⟩, 100% |1⟩
- Perfectly distinguishable

---

**Orthonormal Basis:**
```
⟨φᵢ|φⱼ⟩ = δᵢⱼ = {1 if i=j
                {0 if i≠j
```

**Where δᵢⱼ = Kronecker delta**

**Example:**
```
⟨0|0⟩ = 1  (normalized)
⟨1|1⟩ = 1  (normalized)
⟨0|1⟩ = 0  (orthogonal)
⟨1|0⟩ = 0  (orthogonal)
```

---

#### **Applications in Quantum States:**

**1. State Overlap:**
```
|⟨φ|ψ⟩|² = "How similar are |φ⟩ and |ψ⟩?"
```

- Close to 1: Similar states
- Close to 0: Different states

---

**2. Projection:**
```
Component of |ψ⟩ along |φ⟩ = ⟨φ|ψ⟩|φ⟩
```

**Example:**
```
|ψ⟩ = (1/√2)|0⟩ + (1/√2)|1⟩
Project onto |0⟩:
⟨0|ψ⟩|0⟩ = (1/√2)|0⟩
```

---

**3. Completeness Relation:**
Orthonormal basis {|φₙ⟩} ku:
```
Σₙ |φₙ⟩⟨φₙ| = I (Identity)

Any state:
|ψ⟩ = Σₙ ⟨φₙ|ψ⟩|φₙ⟩
```

**Physical Meaning:**
- State-a basis la expand pannalam
- Coefficients = Inner products

---

#### **Example: State Analysis**

**Given:**
```
|ψ⟩ = (3/5)|0⟩ + (4/5)|1⟩
```

**Questions:**

**Q1: Is it normalized?**
```
⟨ψ|ψ⟩ = (3/5)² + (4/5)² = 9/25 + 16/25 = 1 ✓
```

**Q2: Probability of |0⟩?**
```
P(0) = |⟨0|ψ⟩|² = |3/5|² = 9/25 = 0.36
```

**Q3: Probability of |+⟩?**
```
|+⟩ = (|0⟩ + |1⟩)/√2

⟨+|ψ⟩ = (⟨0| + ⟨1|)/√2 · (3/5|0⟩ + 4/5|1⟩)
      = (1/√2)(3/5 + 4/5)
      = 7/(5√2)

P(+) = |7/(5√2)|² = 49/50 = 0.98
```

---

**Summary:**
- Inner product: Probability amplitudes
- Normalization: Total probability = 1
- Orthogonality: Distinguishable states
- |⟨φ|ψ⟩|²: Measurement probability
- Essential tool quantum mechanics la

---

### 13A. Postulates of Quantum Computing

Quantum computing mathematical foundation postulates-a base panrum. Idhu quantum systems behave panradhu and manipulate panradhu describe panrum.

---

#### **Postulate 1: State Space**

**Statement:**
"Any isolated physical system associated-a irukum complex vector space (Hilbert space). System completely state vector |ψ⟩ (unit vector) describe pannalam."

**Key Points:**

**Single Qubit:**
- 2D Hilbert space
- State: |ψ⟩ = α|0⟩ + β|1⟩
- Normalization: |α|² + |β|² = 1

**n Qubits:**
- 2ⁿ dimensional space
- Basis states: |0...0⟩ to |1...1⟩
- Superposition of all basis states

**Physical Significance:**
- State vector complete information encode
- Deterministic time evolution (until measurement)
- Superposition fundamental property
- Classical bit: |0⟩ OR |1⟩
- Quantum bit: α|0⟩ + β|1⟩ (both simultaneously)

**Example:**
```
Single qubit: 2 complex numbers (α, β)
             = Infinite possible states (unit sphere)
Classical bit: 2 states only (0 or 1)
```

---

#### **Postulate 2: Evolution**

**Statement:**
"Closed quantum system-oda evolution unitary operators describe pannalam. State time t₁ to t₂ ku evolve aagum via:
|ψ(t₂)⟩ = U|ψ(t₁)⟩"

**Properties of Unitary Operator U:**
```
U†U = UU† = I
(U† = Conjugate transpose)
```

**Key Characteristics:**

**1. Reversible:**
- U⁻¹ = U† exists
- Information loss illa
- Time reverse pannalam

**2. Norm Preserving:**
```
⟨ψ|ψ⟩ = 1 maintained
Probabilities conserved
```

**3. Linear:**
- Superposition preserve
- If U|ψ⟩ = |φ⟩ and U|χ⟩ = |η⟩
- Then U(α|ψ⟩ + β|χ⟩) = α|φ⟩ + β|η⟩

---

**Schrödinger Equation Connection:**
```
iℏ(d/dt)|ψ⟩ = H|ψ⟩

Solution:
U(t) = e^(-iHt/ℏ)
```

**Where:**
- H = Hamiltonian (energy operator)
- U(t) = Time evolution operator

**Physical Significance:**
- Quantum gates = Unitary matrices
- Computation = Sequence of unitaries
- Reversibility = Fundamental quantum property
- Example: Hadamard gate H² = I (self-inverse)

---

**Examples of Unitary Gates:**

**Pauli-X (NOT):**
```
X|0⟩ = |1⟩
X|1⟩ = |0⟩
X² = I
```

**Hadamard:**
```
H|0⟩ = |+⟩
H|+⟩ = |0⟩
H² = I
```

---

#### **Postulate 3: Measurement**

**Statement:**
"Quantum measurements projective measurements set {Mₘ} describe pannalam. Measurement outcome m probability:
p(m) = ⟨ψ|Mₘ†Mₘ|ψ⟩

Measurement piragu state:
|ψ'⟩ = (Mₘ|ψ⟩)/√(⟨ψ|Mₘ†Mₘ|ψ⟩)"

**Computational Basis Measurement:**

**For qubit |ψ⟩ = α|0⟩ + β|1⟩:**

**Measurement Operators:**
```
M₀ = |0⟩⟨0| (project onto |0⟩)
M₁ = |1⟩⟨1| (project onto |1⟩)
```

**Probabilities:**
```
P(0) = |⟨0|ψ⟩|² = |α|²
P(1) = |⟨1|ψ⟩|² = |β|²
```

**Post-Measurement States:**
```
If result 0: |ψ'⟩ = |0⟩
If result 1: |ψ'⟩ = |1⟩
```

---

**Key Properties:**

**1. Probabilistic:**
- Deterministic evolution, probabilistic measurement
- Cannot predict outcome, only probabilities

**2. State Collapse:**
- Superposition → Definite state
- Irreversible process
- Information partially lost

**3. Completeness:**
```
Σₘ Mₘ†Mₘ = I
(Probabilities sum to 1)
```

**4. Non-Cloning:**
- Cannot copy unknown quantum state
- Measurement destroys superposition

---

**Physical Significance:**

**Classical vs Quantum:**
```
Classical: Measure without disturbing
Quantum: Measurement fundamentally disturbs
```

**Example:**
```
State: |ψ⟩ = (|0⟩ + |1⟩)/√2
Measure: 50% chance |0⟩, 50% chance |1⟩
After measurement: Definitely |0⟩ OR |1⟩
Superposition gone forever
```

**Implications:**
- Quantum parallelism extract difficult
- Interference needed before measurement
- Algorithms carefully designed

---

#### **Postulate 4: Composite Systems**

**Statement:**
"Composite system-oda state space individual systems-oda tensor product.
System 1 (state space H₁) + System 2 (state space H₂)
→ Composite (H₁ ⊗ H₂)"

**Two Qubits Example:**

**Individual States:**
```
Qubit 1: |ψ⟩ = α|0⟩ + β|1⟩
Qubit 2: |φ⟩ = γ|0⟩ + δ|1⟩
```

**Composite State:**
```
|ψ⟩ ⊗ |φ⟩ = (α|0⟩ + β|1⟩) ⊗ (γ|0⟩ + δ|1⟩)
          = αγ|00⟩ + αδ|01⟩ + βγ|10⟩ + βδ|11⟩
```

**Dimension:**
- System 1: 2D
- System 2: 2D
- Composite: 2 × 2 = 4D

---

**Important Concept: Entanglement**

**Separable State:**
```
|ψ⟩ = |ψ₁⟩ ⊗ |ψ₂⟩
(Can write as product)
```

**Entangled State:**
```
|Φ⁺⟩ = (|00⟩ + |11⟩)/√2
(Cannot write as product!)
```

**Why Entangled:**
Try to write as (α|0⟩ + β|1⟩) ⊗ (γ|0⟩ + δ|1⟩):
```
= αγ|00⟩ + αδ|01⟩ + βγ|10⟩ + βδ|11⟩
```

For |Φ⁺⟩ need:
- αγ = 1/√2
- αδ = 0
- βγ = 0
- βδ = 1/√2

Contradictory! (If αδ = 0, then α = 0 or δ = 0, but αγ ≠ 0 needs α ≠ 0 and γ ≠ 0)

---

**Physical Significance:**

**Entanglement Properties:**
- Measure one qubit → instantly affect other
- Stronger than classical correlation
- Non-local correlations
- Quantum communication & cryptography base

**n Qubit System:**
```
Dimension = 2ⁿ
n = 3: 8D
n = 10: 1024D
n = 300: > atoms in universe!
```

**Quantum Advantage:**
- Exponential state space
- Classical simulation impractical
- Source of quantum speedup

---

#### **Summary of Postulates:**

| Postulate | Describes | Key Concept |
|-----------|-----------|-------------|
| **1: State Space** | System representation | Hilbert space, superposition |
| **2: Evolution** | Time dynamics | Unitary operators, reversible |
| **3: Measurement** | Observation | Collapse, probabilistic |
| **4: Composite** | Multiple systems | Tensor product, entanglement |

---

**Role in Quantum Computing:**

**Algorithm Design:**
1. Initialize (Postulate 1)
2. Apply gates (Postulate 2)
3. Create entanglement (Postulate 4)
4. Measure (Postulate 3)

**Example: Deutsch Algorithm**
```
1. Start: |0⟩ (Postulate 1)
2. Apply H: |0⟩ → |+⟩ (Postulate 2)
3. Apply Oracle (Postulate 2)
4. Apply H again (Postulate 2)
5. Measure (Postulate 3)
```

**Error Correction:**
- Postulate 2: Errors = unwanted unitaries
- Postulate 3: Measurement for syndrome
- Postulate 4: Entanglement for encoding

---

**Philosophical Implications:**
- Reality measurement varaikum indefinite
- Observer role central
- Information fundamental (not matter/energy)
- Universe computational process

---

### 13B. Bloch Sphere Representation

#### **Introduction:**

Qubit state-a geometric-a visualize panna Bloch sphere use pannurom. 3D sphere la any single qubit state represent pannalam.

---

#### **Arbitrary Single-Qubit State:**

**General Form:**
```
|ψ⟩ = α|0⟩ + β|1⟩
```

**Constraints:**
- α, β = complex numbers
- |α|² + |β|² = 1 (normalization)

**Degrees of Freedom:**
- 2 complex numbers = 4 real parameters
- Normalization: -1 constraint
- Global phase: -1 (unobservable)
- **Net: 2 real parameters** (θ, φ)

---

#### **Bloch Sphere Parameterization:**

**Standard Form:**
```
|ψ⟩ = cos(θ/2)|0⟩ + e^(iφ)sin(θ/2)|1⟩
```

**Where:**
- θ = Polar angle (0 ≤ θ ≤ π)
- φ = Azimuthal angle (0 ≤ φ < 2π)

---

**Geometric Interpretation:**

```
          |0⟩ (North Pole)
           ↑
           │
    ─────┼─────  Equator
         /│\
        / │ \ 
       /  │  \
      /   ↓   \
    |1⟩ (South Pole)
    
Sphere radius = 1
Any point = Valid qubit state
```

---

#### **Special Points on Bloch Sphere:**

**1. Computational Basis (Z-axis):**
```
|0⟩: θ = 0, φ = any
     (North pole)

|1⟩: θ = π, φ = any
     (South pole)
```

---

**2. X-Basis (X-axis):**
```
|+⟩ = (|0⟩ + |1⟩)/√2
     θ = π/2, φ = 0
     (Positive X-axis)

|−⟩ = (|0⟩ - |1⟩)/√2
     θ = π/2, φ = π
     (Negative X-axis)
```

---

**3. Y-Basis (Y-axis):**
```
|i+⟩ = (|0⟩ + i|1⟩)/√2
      θ = π/2, φ = π/2
      (Positive Y-axis)

|i−⟩ = (|0⟩ - i|1⟩)/√2
      θ = π/2, φ = 3π/2
      (Negative Y-axis)
```

---

#### **Bloch Vector:**

State |ψ⟩ ku corresponding 3D unit vector:
```
r⃗ = (x, y, z)

Where:
x = sin(θ)cos(φ)
y = sin(θ)sin(φ)
z = cos(θ)
```

**Magnitude:** |r⃗| = 1

---

**Example Calculations:**

**State:** |+⟩ = (|0⟩ + |1⟩)/√2
```
θ = π/2, φ = 0
x = sin(π/2)cos(0) = 1
y = sin(π/2)sin(0) = 0
z = cos(π/2) = 0
Bloch vector: (1, 0, 0)
```

**State:** |1⟩
```
θ = π, φ = 0
x = sin(π)cos(0) = 0
y = sin(π)sin(0) = 0
z = cos(π) = -1
Bloch vector: (0, 0, -1)
```

---

#### **Applications of Bloch Sphere:**

**1. Visualizing Quantum Gates:**

**Pauli-X (Bit Flip):**
```
Rotation by π around X-axis
|0⟩ → |1⟩ (North → South)
|1⟩ → |0⟩ (South → North)
```

**Pauli-Z (Phase Flip):**
```
Rotation by π around Z-axis
|+⟩ → |−⟩ (X-axis flip)
Equatorial plane rotation
```

**Hadamard Gate:**
```
π rotation around axis (X + Z)/√2
|0⟩ → |+⟩ (North → +X)
|1⟩ → |−⟩ (South → -X)
```

---

**2. Measurement Interpretation:**

**Z-basis Measurement:**
- Project onto Z-axis
- Probability ∝ z-component
- P(|0⟩) = (1 + z)/2
- P(|1⟩) = (1 - z)/2

**Example:**
```
State at equator (z = 0):
P(|0⟩) = P(|1⟩) = 1/2
Equal superposition
```

---

**3. State Distance:**

**Angle between states = Distinguishability**
```
|⟨ψ|φ⟩|² = cos²(θ/2)
```

Where θ = angle between Bloch vectors

**Orthogonal states:**
- Opposite points on sphere
- θ = π
- Perfectly distinguishable

---

#### **Pure vs Mixed States:**

**Pure State:**
- Surface of Bloch sphere
- |r⃗| = 1
- Complete information

**Mixed State (Classical Uncertainty):**
- Inside Bloch sphere
- |r⃗| < 1
- Statistical mixture
- NOT quantum superposition

---

#### **Limitations:**

**1. Single Qubit Only:**
- Multi-qubit states cannot represent
- Entanglement not visualizable

**2. Two Qubits:**
- Would need 7D space!
- (2⁴ - 2 normalization - 1 global phase = 7)

---

#### **Example: Custom State Representation**

**Problem:** Represent state on Bloch sphere
```
|ψ⟩ = (√3/2)|0⟩ + (1/2)|1⟩
```

**Solution:**
```
α = √3/2, β = 1/2 (both real)

cos(θ/2) = √3/2 → θ/2 = 30° → θ = 60°
sin(θ/2) = 1/2 (matches)

β real → φ = 0

Bloch coordinates:
θ = 60° = π/3
φ = 0

Bloch vector:
x = sin(60°)cos(0) = √3/2
y = 0
z = cos(60°) = 1/2

Point: Upper hemisphere, towards +X
```

---

**Summary:**
- Bloch sphere = 3D visualization tool
- θ, φ = 2 parameters for qubit
- Special points = basis states
- Gates = Rotations
- Surface = Pure states
- Measurement = Projection
- Single qubit only (limitation)

---

### 14A. Single-Qubit Gates (Pauli & Hadamard)

#### **Introduction to Quantum Gates:**

Quantum gates unitary operators - qubit states transform panrum, classical logic gates quantum equivalent.

**Key Properties:**
- Unitary (reversible)
- Linear (superposition preserve)
- Matrix representation
- Geometric interpretation (Bloch sphere)

---

#### **1. Pauli-X Gate (NOT Gate):**

**Matrix Representation:**
```
X = [0 1]
    [1 0]
```

**Action:**
```
X|0⟩ = |1⟩
X|1⟩ = |0⟩
```

**Verification:**
```
X|0⟩ = [0 1][1] = [0] = |1⟩
       [1 0][0]   [1]

X|1⟩ = [0 1][0] = [1] = |0⟩
       [1 0][1]   [0]
```

---

**Effect on Superposition:**
```
|ψ⟩ = α|0⟩ + β|1⟩

X|ψ⟩ = α·X|0⟩ + β·X|1⟩
     = α|1⟩ + β|0⟩
     = β|0⟩ + α|1⟩
     (Amplitudes swapped)
```

---

**Bloch Sphere Interpretation:**
```
Rotation by π (180°) around X-axis

     |0⟩
      ↓  
     |1⟩  (flip)

Equator states preserved:
|+⟩ → |+⟩
|−⟩ → |−⟩
```

---

**Properties:**
```
X² = I (Self-inverse)
X† = X (Hermitian)
Det(X) = -1
Eigenvalues: +1, -1
```

**Physical Significance:**
- Classical NOT gate quantum version
- Bit flip error model
- Spin flip operation

---

#### **2. Pauli-Y Gate:**

**Matrix:**
```
Y = [0 -i]
    [i  0]
```

**Action:**
```
Y|0⟩ = i|1⟩
Y|1⟩ = -i|0⟩
```

**Verification:**
```
Y|0⟩ = [0 -i][1] = [ 0] = 0|0⟩ + i|1⟩ = i|1⟩
       [i  0][0]   [i ]

Y|1⟩ = [0 -i][0] = [-i] = -i|0⟩ + 0|1⟩ = -i|0⟩
       [i  0][1]   [ 0]
```

---

**Effect on General State:**
```
|ψ⟩ = α|0⟩ + β|1⟩

Y|ψ⟩ = α(i|1⟩) + β(-i|0⟩)
     = -iβ|0⟩ + iα|1⟩
```

---

**Bloch Sphere:**
```
Rotation by π around Y-axis

Computational basis affected:
|0⟩ ↔ |1⟩ (with phase)

Y-axis eigenstates preserved:
|i+⟩ → |i+⟩
|i−⟩ → |i−⟩
```

---

**Properties:**
```
Y² = I
Y† = Y (Hermitian)
Y = iXZ (Combination)
```

**Physical Significance:**
- Combined bit + phase flip
- Pauli algebra: Y = iXZ

---

#### **3. Pauli-Z Gate (Phase Flip):**

**Matrix:**
```
Z = [1  0]
    [0 -1]
```

**Action:**
```
Z|0⟩ = |0⟩
Z|1⟩ = -|1⟩
```

**Verification:**
```
Z|0⟩ = [1  0][1] = [1] = |0⟩
       [0 -1][0]   [0]

Z|1⟩ = [1  0][0] = [ 0] = -|1⟩
       [0 -1][1]   [-1]
```

---

**Effect on Superposition:**
```
|ψ⟩ = α|0⟩ + β|1⟩

Z|ψ⟩ = α|0⟩ - β|1⟩
      (|1⟩ amplitude sign flipped)
```

**Example:**
```
|+⟩ = (|0⟩ + |1⟩)/√2

Z|+⟩ = (|0⟩ - |1⟩)/√2 = |−⟩
```

---

**Bloch Sphere:**
```
Rotation by π around Z-axis

Computational basis unchanged:
|0⟩ → |0⟩ (North pole)
|1⟩ → -|1⟩ (South pole, global phase)

Equatorial plane:
|+⟩ ↔ |−⟩ (phase flip)
```

---

**Properties:**
```
Z² = I
Z† = Z (Hermitian)
Z = diagonal (eigenstates |0⟩, |1⟩)
```

**Physical Significance:**
- Phase flip (no basis change)
- Phase kickback mechanism
- Controlled operations base

---

#### **4. Hadamard Gate:**

**Matrix:**
```
H = (1/√2)[1  1]
           [1 -1]
```

**Action:**
```
H|0⟩ = (|0⟩ + |1⟩)/√2 = |+⟩
H|1⟩ = (|0⟩ - |1⟩)/√2 = |−⟩
```

**Verification:**
```
H|0⟩ = (1/√2)[1  1][1] = (1/√2)[1] = (|0⟩+|1⟩)/√2
              [1 -1][0]          [1]

H|1⟩ = (1/√2)[1  1][0] = (1/√2)[ 1] = (|0⟩-|1⟩)/√2
              [1 -1][1]          [-1]
```

---

**Reverse Action:**
```
H|+⟩ = H·H|0⟩ = H²|0⟩ = |0⟩
H|−⟩ = H·H|1⟩ = H²|1⟩ = |1⟩

H² = I (Self-inverse)
```

---

**Effect on General State:**
```
|ψ⟩ = α|0⟩ + β|1⟩

H|ψ⟩ = α·H|0⟩ + β·H|1⟩
     = α(|0⟩+|1⟩)/√2 + β(|0⟩-|1⟩)/√2
     = ((α+β)|0⟩ + (α-β)|1⟩)/√2
```

---

**Bloch Sphere:**
```
Rotation by π around (X+Z)/√2 axis

Key transformations:
|0⟩ → |+⟩ (Z-basis → X-basis)
|+⟩ → |0⟩ (X-basis → Z-basis)

Geometric: 90° + reflection
```

---

**Properties:**
```
H² = I (Self-inverse)
H† = H (Hermitian & Unitary)
Eigenvalues: +1, -1
Eigenvectors: |0⟩±|1⟩
```

---

**Physical Significance:**

**1. Basis Change:**
```
Computational (Z) ↔ Hadamard (X) basis
```

**2. Superposition Creation:**
```
Definite state → Equal superposition
|0⟩ → 50-50 state |+⟩
```

**3. Quantum Algorithm Essential:**
- Deutsch algorithm
- Grover search
- QFT (Quantum Fourier Transform)

---

#### **Comparative Analysis:**

| Gate | Basis Affected | Type | Key Use |
|------|---------------|------|---------|
| **X** | Flips |0⟩↔|1⟩ | Bit flip | NOT operation |
| **Y** | Flips with phase | Bit+Phase | Combined error |
| **Z** | Phase only | Phase flip | Controlled ops |
| **H** | Basis change | Superpose | Algorithms |

---

**Combined Example:**

**Problem:** Apply H, then X, then H to |0⟩

**Solution:**
```
Step 1: H|0⟩ = |+⟩ = (|0⟩+|1⟩)/√2

Step 2: X|+⟩ = X(|0⟩+|1⟩)/√2
              = (|1⟩+|0⟩)/√2
              = |+⟩ (unchanged!)

Step 3: H|+⟩ = |0⟩

Result: H·X·H|0⟩ = |0⟩
```

**Interesting:** HXH = Z (conjugation)

---

**Gate Sequences:**

```
XZ = -ZX (Anti-commute)
HXH = Z (Basis conjugation)
HZH = X (Basis conjugation)
```

---

**Summary:**
- Pauli gates: Basic rotations (π)
- X: Bit flip (computational basis)
- Y: Bit + phase (combined)
- Z: Phase flip (relative phase)
- H: Superposition creator (basis change)
- All unitary, reversible, norm-preserving

---

### 14B. Two-Qubit States & Bell States

#### **Two-Qubit State Space:**

**Basis States:**
```
|00⟩, |01⟩, |10⟩, |11⟩
```

**Dimension:** 2² = 4

**General State:**
```
|ψ⟩ = α₀₀|00⟩ + α₀₁|01⟩ + α₁₀|10⟩ + α₁₁|11⟩
```

**Normalization:**
```
|α₀₀|² + |α₀₁|² + |α₁₀|² + |α₁₁|² = 1
```

---

#### **Separable vs Entangled States:**

**Separable (Product State):**
```
|ψ⟩ = |ψ₁⟩ ⊗ |ψ₂⟩
     = (α|0⟩ + β|1⟩) ⊗ (γ|0⟩ + δ|1⟩)
```

**Example:**
```
|ψ⟩ = |0⟩ ⊗ |+⟩ = |0⟩(|0⟩+|1⟩)/√2
     = (|00⟩ + |01⟩)/√2
```

**Properties:**
- Independent qubits
- Measure one, other unaffected
- Classical correlation

---

**Entangled State:**
Cannot write as product!

**Example:**
```
|Φ⁺⟩ = (|00⟩ + |11⟩)/√2
```

**Test for Product:**
Try |ψ⟩ = (α|0⟩+β|1⟩) ⊗ (γ|0⟩+δ|1⟩):
```
= αγ|00⟩ + αδ|01⟩ + βγ|10⟩ + βδ|11⟩
```

For |Φ⁺⟩:
- αγ = 1/√2 → α, γ ≠ 0
- αδ = 0 → α = 0 OR δ = 0 (Contradiction!)
- Cannot be product!

---

#### **Bell States (Maximally Entangled):**

**Four Bell States:**

**1. Phi-Plus (|Φ⁺⟩):**
```
|Φ⁺⟩ = (|00⟩ + |11⟩)/√2
```

**Properties:**
- Measure first qubit → second instantly determined
- |0⟩ → |0⟩ or |1⟩ → |1⟩
- Perfect correlation

---

**2. Phi-Minus (|Φ⁻⟩):**
```
|Φ⁻⟩ = (|00⟩ - |11⟩)/√2
```

**Properties:**
- Similar correlation, opposite phase
- |0⟩ → |0⟩ or |1⟩ → |1⟩
- Relative phase π

---

**3. Psi-Plus (|Ψ⁺⟩):**
```
|Ψ⁺⟩ = (|01⟩ + |10⟩)/√2
```

**Properties:**
- Anti-correlated
- |0⟩ → |1⟩ or |1⟩ → |0⟩
- Opposite outcomes

---

**4. Psi-Minus (|Ψ⁻⟩):**
```
|Ψ⁻⟩ = (|01⟩ - |10⟩)/√2
```

**Properties:**
- Anti-correlated with phase
- Singlet state
- Antisymmetric

---

#### **Properties of Bell States:**

**1. Orthonormal:**
```
⟨Φ⁺|Φ⁺⟩ = 1
⟨Φ⁺|Φ⁻⟩ = 0
⟨Φ⁺|Ψ⁺⟩ = 0
(All pairs orthogonal)
```

---

**2. Maximal Entanglement:**
- Cannot be written as product
- Strongest quantum correlation
- Entropy measure maximum

---

**3. Bell Basis:**
```
Complete orthonormal basis
Any two-qubit state-a Bell states combination-a express pannalam
```

---

**4. Symmetric/Antisymmetric:**
```
Φ⁺, Φ⁻, Ψ⁺: Symmetric
Ψ⁻: Antisymmetric (exchange qubits → minus sign)
```

---

#### **Creating Bell States:**

**Circuit for |Φ⁺⟩:**
```
|00⟩ → H ⊗ I → CNOT → (|00⟩+|11⟩)/√2

Steps:
1. Start: |00⟩
2. Hadamard on first: (|0⟩+|1⟩)/√2 ⊗ |0⟩ = (|00⟩+|10⟩)/√2
3. CNOT: (|00⟩+|11⟩)/√2 = |Φ⁺⟩
```

---

**Other Bell States:**
```
|Φ⁻⟩: Apply Z to first qubit of |Φ⁺⟩
|Ψ⁺⟩: Apply X to first qubit of |Φ⁺⟩
|Ψ⁻⟩: Apply ZX to first qubit of |Φ⁺⟩
```

---

#### **Measurement Properties:**

**Measure |Φ⁺⟩ in Computational Basis:**

**Before Measurement:**
- System in superposition
- Neither 00 nor 11

**Measure First Qubit:**
```
If result |0⟩:
- Second qubit automatically |0⟩
- Probability 1/2
- State collapses to |00⟩

If result |1⟩:
- Second qubit automatically |1⟩
- Probability 1/2
- State collapses to |11⟩
```

**Non-locality:**
- Instant correlation (faster than light?)
- No information transfer (random outcomes)
- Einstein "spooky action"

---

**Measure in Bell Basis:**
```
Measure |Φ⁺⟩ in Bell basis:
Result |Φ⁺⟩ with probability 1
(Deterministic in own basis)
```

---

#### **Applications:**

**1. Quantum Teleportation:**
```
Unknown state |ψ⟩ teleport panna
Bell state shared resource
Classical communication + entanglement
State transfer without physical travel
```

---

**2. Superdense Coding:**
```
2 classical bits send using 1 qubit
Entanglement pre-shared
Double classical capacity
```

---

**3. Quantum Cryptography (E91):**
```
Bell state violation classical bounds
Eavesdropping detectable
Secure key distribution
```

---

**4. Quantum Error Correction:**
```
Entanglement encode information
Redundancy create
Errors detect & correct
```

---

#### **Bell's Theorem:**

**Statement:**
No local hidden variable theory can reproduce quantum predictions.

**CHSH Inequality:**
Classical limit: |S| ≤ 2
Quantum mechanics: |S| ≤ 2√2

**Violation:**
```
Bell states: S = 2√2 ≈ 2.828
Clearly > 2 (classical limit)
Quantum mechanics confirmed
```

**Significance:**
- Quantum correlations non-classical
- Local realism violated
- Nature fundamentally quantum

---

**Summary:**
- Two qubits: 4D space
- Separable: Product form possible
- Entangled: Cannot factor
- Bell states: Maximally entangled
- Four orthonormal Bell states
- Quantum correlation stronger than classical
- Applications: Teleportation, cryptography
- Bell's theorem: Non-local nature confirmed

---

### 15A. Dirac Notation & Bra-Ket

#### **Introduction:**

Paul Dirac invent panna notation quantum states represent panna elegant-a use pannalam. "Bra-ket" notation-nu koopduvaanga (bracket-a split pannirukkaanga).

---

#### **Ket Vectors:**

**Definition:** Column vector representing quantum state.

**Notation:** |ψ⟩

**Example (Qubit):**
```
|0⟩ = [1]    |1⟩ = [0]
      [0]          [1]

|ψ⟩ = [α]  = α|0⟩ + β|1⟩
      [β]
```

---

**Properties:**
- State vectors
- Complex entries allowed
- Normalized: ⟨ψ|ψ⟩ = 1

---

#### **Bra Vectors:**

**Definition:** Row vector, ket-oda conjugate transpose.

**Notation:** ⟨ψ|

**Mathematical:**
```
If |ψ⟩ = [α]
         [β]

Then ⟨ψ| = [α* β*]
```

**Example:**
```
|ψ⟩ = (1+i)|0⟩ + 2i|1⟩

⟨ψ| = (1-i)⟨0| - 2i⟨1|
```

---

#### **Inner Product (Bra-ket):**

**Definition:**
```
⟨φ|ψ⟩ = φ₁*ψ₁ + φ₂*ψ₂ + ...
```

**Result:** Complex number (scalar)

---

**Example:**
```
|ψ⟩ = 3|0⟩ + 4i|1⟩
|φ⟩ = 1|0⟩ + 2|1⟩

⟨φ|ψ⟩ = (1*)(3) + (2*)(4i)
      = 3 + 8i

⟨ψ|φ⟩ = (3*)(1) + (-4i*)(2)
      = 3 - 8i
      = ⟨φ|ψ⟩* (Conjugate)
```

---

**Special Cases:**
```
⟨0|0⟩ = 1 (Normalized)
⟨1|1⟩ = 1
⟨0|1⟩ = 0 (Orthogonal)
⟨1|0⟩ = 0
```

---

#### **Outer Product:**

**Definition:**
```
|ψ⟩⟨φ| = Matrix
```

**Example:**
```
|0⟩⟨0| = [1][1 0] = [1 0]
         [0]        [0 0]

|1⟩⟨1| = [0][0 1] = [0 0]
         [1]        [0 1]

|0⟩⟨1| = [1][0 1] = [0 1]
         [0]        [0 0]
```

---

**Properties:**
```
(|ψ⟩⟨φ|)† = |φ⟩⟨ψ|
```

**Use:** Projection operators, density matrices

---

#### **Representing Quantum States:**

**1. Pure States:**
```
|ψ⟩ = α|0⟩ + β|1⟩

Components clear
Phase explicit
Normalization easy to check
```

---

**2. Multi-Qubit States:**
```
Two qubits:
|ψ⟩ = α|00⟩ + β|01⟩ + γ|10⟩ + δ|11⟩

Tensor product:
|ψ⟩ ⊗ |φ⟩ = |ψφ⟩

Example:
|0⟩ ⊗ |1⟩ = |01⟩
```

---

**3. Superposition:**
```
|+⟩ = (|0⟩ + |1⟩)/√2
|−⟩ = (|0⟩ - |1⟩)/√2

Clear combination
Coefficients explicit
```

---

**4. Entangled States:**
```
|Φ⁺⟩ = (|00⟩ + |11⟩)/√2

Cannot write as product
Correlation clear
```

---

#### **Operations in Dirac Notation:**

**1. Operator Action:**
```
A|ψ⟩ = |φ⟩

Example:
X|0⟩ = |1⟩
H|0⟩ = (|0⟩+|1⟩)/√2
```

---

**2. Expectation Value:**
```
⟨A⟩ = ⟨ψ|A|ψ⟩

Example:
⟨Z⟩ = ⟨ψ|Z|ψ⟩
    = (α*⟨0| + β*⟨1|)Z(α|0⟩ + β|1⟩)
    = |α|² - |β|²
```

---

**3. Probability:**
```
P(measurement = |φ⟩) = |⟨φ|ψ⟩|²

Example:
|ψ⟩ = (3|0⟩ + 4|1⟩)/5
P(0) = |⟨0|ψ⟩|² = |3/5|² = 9/25
```

---

**4. Projection:**
```
Project |ψ⟩ onto |φ⟩:
|φ⟩⟨φ|ψ⟩

Example:
|0⟩⟨0|ψ⟩ = |0⟩⟨0|(α|0⟩+β|1⟩)
          = α|0⟩
```

---

#### **Completeness Relation:**

**For basis {|φₙ⟩}:**
```
Σₙ |φₙ⟩⟨φₙ| = I

Example (computational basis):
|0⟩⟨0| + |1⟩⟨1| = I
```

**Use:** Identity decomposition

---

**Application:**
```
|ψ⟩ = I|ψ⟩
    = (|0⟩⟨0| + |1⟩⟨1|)|ψ⟩
    = |0⟩⟨0|ψ⟩ + |1⟩⟨1|ψ⟩
    = ⟨0|ψ⟩|0⟩ + ⟨1|ψ⟩|1⟩
    (Basis expansion)
```

---

#### **Advantages of Dirac Notation:**

**1. Compact:**
```
Instead of:  ψ = [α]
                 [β]
Write: |ψ⟩ = α|0⟩ + β|1⟩
```

---

**2. Basis Independent:**
```
|ψ⟩ same regardless of coordinate choice
Physical meaning clear
```

---

**3. Operations Intuitive:**
```
⟨φ|ψ⟩ = Inner product (automatic)
|ψ⟩⟨φ| = Outer product (clear)
A|ψ⟩ = Transformation (natural)
```

---

**4. Multi-Particle Easy:**
```
|ψ₁⟩|ψ₂⟩|ψ₃⟩ = |ψ₁ψ₂ψ₃⟩
Tensor products implicit
```

---

**Summary:**
- |ψ⟩ = Ket (state vector)
- ⟨ψ| = Bra (dual vector)
- ⟨φ|ψ⟩ = Inner product (scalar)
- |ψ⟩⟨φ| = Outer product (operator)
- Compact, elegant, physics-focused notation
- Standard quantum mechanics notation

---

###15B. Computational Basis & Orthonormal Properties

#### **Definition of Computational Basis:**

**Single Qubit:**
```
|0⟩ = [1]    |1⟩ = [0]
      [0]          [1]
```

**Standard basis quantum computing la**, classical bits quantum equivalent.

---

**Why "Computational":**
- Binary encoding natural
- Measurement outcomes classical bits
- Algorithm results easily interpret

---

#### **Multi-Qubit Computational Basis:**

**Two Qubits:**
```
|00⟩ = [1]    |01⟩ = [0]    |10⟩ = [0]    |11⟩ = [0]
       [0]           [1]           [0]           [0]
       [0]           [0]           [1]           [0]
       [0]           [0]           [0]           [1]
```

**Dimension:** 4

---

**Three Qubits:**
```
|000⟩, |001⟩, |010⟩, |011⟩,
|100⟩, |101⟩, |110⟩, |111⟩
```

**Dimension:** 8 = 2³

---

**n Qubits:**
- Basis states: 2ⁿ
- Dimension: 2ⁿ
- Tensor product structure

---

#### **Orthonormality Properties:**

**1. Normalization:**
```
⟨i|i⟩ = 1  for all basis states |i⟩
```

**Examples:**
```
⟨0|0⟩ = [1 0][1] = 1
              [0]

⟨1|1⟩ = [0 1][0] = 1
              [1]

⟨00|00⟩ = 1
⟨101|101⟩ = 1
```

**Physical Meaning:**
- Unit length vectors
- Probability interpretation
- Well-defined states

---

**2. Orthogonality:**
```
⟨i|j⟩ = 0  for i ≠ j
```

**Examples:**
```
⟨0|1⟩ = [1 0][0] = 0
              [1]

⟨1|0⟩ = [0 1][1] = 0
              [0]

⟨00|01⟩ = 0
⟨10|11⟩ = 0
⟨000|111⟩ = 0
```

**Physical Meaning:**
- Perfectly distinguishable
- Measurement la no ambiguity
- Exclusive outcomes

---

**3. Kronecker Delta:**
```
⟨i|j⟩ = δᵢⱼ = {1 if i = j
              {0 if i ≠ j
```

**Complete Orthonormal Relation**

---

#### **Why Orthonormal Basis Important:**

**1. Unique Expansion:**

Any state |ψ⟩-a basis la unique-a expand pannalam:
```
|ψ⟩ = Σᵢ cᵢ|i⟩
```

**Where:**
```
cᵢ = ⟨i|ψ⟩ (Projection)
```

**Example:**
```
|ψ⟩ = (3/5)|0⟩ + (4/5)|1⟩

c₀ = ⟨0|ψ⟩ = 3/5
c₁ = ⟨1|ψ⟩ = 4/5
```

---

**2. Probability Interpretation:**

**Born Rule:**
```
P(outcome i) = |⟨i|ψ⟩|² = |cᵢ|²
```

**Example:**
```
|ψ⟩ = (3/5)|0⟩ + (4/5)|1⟩

P(0) = |3/5|² = 9/25 = 36%
P(1) = |4/5|² = 16/25 = 64%
Total = 100% ✓
```

---

**3. Normalization Check:**

Orthonormal basis-la:
```
⟨ψ|ψ⟩ = Σᵢ |cᵢ|²
```

**Must equal 1** for valid quantum state.

**Example:**
```
|ψ⟩ = α|0⟩ + β|1⟩
⟨ψ|ψ⟩ = |α|² + |β|² = 1 (required)
```

---

**4. Easy Calculations:**

Inner product simple:
```
|ψ⟩ = Σᵢ aᵢ|i⟩
|φ⟩ = Σⱼ bⱼ|j⟩

⟨φ|ψ⟩ = Σᵢ aᵢ*bᵢ (direct sum, no cross terms)
```

---

#### **Computational Basis Measurements:**

**Measurement Operators:**
```
M₀ = |0⟩⟨0|  (Project onto |0⟩)
M₁ = |1⟩⟨1|  (Project onto |1⟩)
```

**Properties:**
```
M₀ + M₁ = I (Completeness)
M₀² = M₀ (Projection)
M₁² = M₁
M₀M₁ = 0 (Orthogonal)
```

---

**Measurement Process:**

**State before:** |ψ⟩ = α|0⟩ + β|1⟩

**Measure:**
```
Outcome |0⟩:
- Probability: |α|²
- Post-state: |0⟩

Outcome |1⟩:
- Probability: |β|²
- Post-state: |1⟩
```

---

#### **Completeness Relation:**

**Single Qubit:**
```
|0⟩⟨0| + |1⟩⟨1| = I

Verification:
[1 0] + [0 0] = [1 0] = I ✓
[0 0]   [0 1]   [0 1]
```

---

**Multi-Qubit:**
```
Σᵢ |i⟩⟨i| = I

Example (2 qubits):
|00⟩⟨00| + |01⟩⟨01| + |10⟩⟨10| + |11⟩⟨11| = I₄ₓ₄
```

---

**Use in Decomposition:**
```
|ψ⟩ = I|ψ⟩
    = (Σᵢ |i⟩⟨i|)|ψ⟩
    = Σᵢ |i⟩⟨i|ψ⟩
    = Σᵢ cᵢ|i⟩
```

---

#### **Other Bases (For Comparison):**

**Hadamard Basis (X-basis):**
```
|+⟩ = (|0⟩ + |1⟩)/√2
|−⟩ = (|0⟩ - |1⟩)/√2
```

**Check Orthonormality:**
```
⟨+|+⟩ = 1 ✓
⟨−|−⟩ = 1 ✓
⟨+|−⟩ = ((⟨0|+⟨1|)/√2)((|0⟩-|1⟩)/√2)
      = (1-1)/2 = 0 ✓
```

**Also orthonormal!**

---

**Y-Basis:**
```
|i+⟩ = (|0⟩ + i|1⟩)/√2
|i−⟩ = (|0⟩ - i|1⟩)/√2
```

**Orthonormal:** Yes ✓

---

**Any Unitary Transformation:**
If {|ψᵢ⟩} orthonormal, then U|ψᵢ⟩ also orthonormal.

---

#### **Applications:**

**1. Quantum Algorithms:**
```
Start: |00...0⟩ (Computational basis)
Apply gates
Measure: Computational basis
Result: Classical bitstring
```

---

**2. Error Detection:**
```
Error changes basis state
Syndrome measurement detects
Code space vs error space orthogonal
```

---

**3. State Tomography:**
```
Measure different bases
Reconstruct full state
Computational basis primary
```

---

**Summary:**
- Computational basis: Standard measurement basis
- |0⟩, |1⟩, |00⟩, ..., |11...1⟩
- Orthonormal: ⟨i|j⟩ = δᵢⱼ
- Normalization → probability conservation
- Orthogonality → distinguishability
- Completeness → any state expressible
- Foundation for quantum computing

---

## PART-C (20 MARKS)

### 16A. Inner & Outer Products in Vector Space

#### **Section 1: Inner Product - Detailed Analysis**

**Mathematical Definition:**

Vector space V la, inner product ⟨·|·⟩: V × V → ℂ function with properties:

**1. Linearity (Second Argument):**
```
⟨φ|(α|ψ₁⟩ + β|ψ₂⟩) = α⟨φ|ψ₁⟩ + β⟨φ|ψ₂⟩
```

**2. Conjugate Symmetry:**
```
⟨φ|ψ⟩ = ⟨ψ|φ⟩*
```

**3. Positive Definiteness:**
```
⟨ψ|ψ⟩ ≥ 0
⟨ψ|ψ⟩ = 0 ⟺ |ψ⟩ = 0
```

---

**Computation in Different Bases:**

**Computational Basis:**
```
|ψ⟩ = Σᵢ aᵢ|i⟩
|φ⟩ = Σⱼ bⱼ|j⟩

⟨φ|ψ⟩ = ΣᵢΣⱼ bⱼ*aᵢ⟨j|i⟩
      = ΣᵢΣⱼ bⱼ*aᵢδⱼᵢ
      = Σᵢ bᵢ*aᵢ
```

**Matrix Form:**
```
⟨φ|ψ⟩ = [b₁* b₂* ... bₙ*][a₁]
                          [a₂]
                          [⋮ ]
                          [aₙ]
       = Σᵢ bᵢ*aᵢ
```

---

**Example Calculations:**

**Example 1:**
```
|ψ⟩ = (1+i)|0⟩ + 2|1⟩
|φ⟩ = 3|0⟩ + (1-i)|1⟩

⟨φ|ψ⟩ = 3*(1+i) + (1-i)*·2
      = 3(1+i) + (1+i)·2
      = 3 + 3i + 2 + 2i
      = 5 + 5i

Verify conjugate symmetry:
⟨ψ|φ⟩ = (1-i)·3 + 2*·(1-i)
      = 3 - 3i + 2(1-i)
      = 3 - 3i + 2 - 2i
      = 5 - 5i
      = ⟨φ|ψ⟩* ✓
```

---

**Example 2: Multi-Qubit**
```
|ψ⟩ = (|00⟩ + |11⟩)/√2  (Bell state)
|φ⟩ = (|00⟩ - |11⟩)/√2  (Another Bell)

⟨φ|ψ⟩ = (⟨00| - ⟨11|)/√2 · (|00⟩ + |11⟩)/√2
      = (1/2)(⟨00|00⟩ + ⟨00|11⟩ - ⟨11|00⟩ - ⟨11|11⟩)
      = (1/2)(1 + 0 - 0 - 1)
      = 0

Orthogonal Bell states!
```

---

**Physical Interpretations:**

**1. Probability Amplitude:**
```
⟨φ|ψ⟩ = Amplitude for transition |ψ⟩ → |φ⟩
|⟨φ|ψ⟩|² = Probability
```

**Physical Meaning:**
- System state |ψ⟩-la irundhaa
- |φ⟩ measure panna probability = |⟨φ|ψ⟩|²

**Example:**
```
|ψ⟩ = (√3/2)|0⟩ + (1/2)|1⟩
Measure in |+⟩ state:

|+⟩ = (|0⟩+|1⟩)/√2
⟨+|ψ⟩ = (⟨0|+⟨1|)/√2 · (√3/2|0⟩ + 1/2|1⟩)
      = (1/√2)(√3/2 + 1/2)
      = (√3 + 1)/(2√2)

P(+) = |(√3+1)/(2√2)|²
     = (√3+1)²/8
     = (3 + 2√3 + 1)/8
     = (4 + 2√3)/8
     ≈ 0.933 (93.3%)
```

---

**2. State Overlap:**
```
|⟨φ|ψ⟩| = "Similarity" between states
```

Values:
- **0:** Orthogonal (completely different)
- **1:** Parallel (same/opposite direction)
- **0 < |⟨φ|ψ⟩| < 1:** Partially overlapping

**Example:**
```
|0⟩ and |+⟩:
⟨+|0⟩ = (⟨0|+⟨1|)/√2 · |0⟩
      = 1/√2
|⟨+|0⟩| = 1/√2 ≈ 0.707

45° angle, moderate similarity
```

---

**3. Expectation Values:**
```
⟨A⟩ψ = ⟨ψ|A|ψ⟩
```

**Physical Meaning:**
- Average measurement outcome
- Observable A-oda mean value
- State |ψ⟩-la irundhaa

**Example: Spin Measurement**
```
|ψ⟩ = cos(θ/2)|0⟩ + sin(θ/2)|1⟩
A = Z (Pauli-Z)

⟨Z⟩ = ⟨ψ|Z|ψ⟩
    = (cos(θ/2)⟨0| + sin(θ/2)⟨1|)Z(cos(θ/2)|0⟩ + sin(θ/2)|1⟩)
    = cos²(θ/2)⟨0|Z|0⟩ + sin²(θ/2)⟨1|Z|1⟩
    = cos²(θ/2)·1 + sin²(θ/2)·(-1)
    = cos(θ)

Interpretation: Average spin along Z-axis = cos(θ)
```

---

**4. Distance Metric:**

**Fidelity:**
```
F(ψ,φ) = |⟨φ|ψ⟩|²
```

Measures "closeness" of states:
- F = 1: Identical states
- F = 0: Orthogonal states

**Application:** Quantum state comparison, error analysis

---

**5. Causchy-Schwarz Inequality:**
```
|⟨φ|ψ⟩|² ≤ ⟨φ|φ⟩⟨ψ|ψ⟩

For normalized states:
|⟨φ|ψ⟩| ≤ 1
```

**Physical Meaning:**
Probability never exceed 1 (obvious but mathematically guaranteed).

---

#### **Section 2: Outer Product - Detailed Analysis**

**Mathematical Definition:**
```
|ψ⟩⟨φ|: V → V (Linear operator)
```

**Action:**
```
(|ψ⟩⟨φ|)|χ⟩ = |ψ⟩⟨φ|χ⟩
              = ⟨φ|χ⟩|ψ⟩  (scalar times ket)
```

---

**Matrix Representation:**

**Computational Basis:**
```
|ψ⟩ = [a₁]    ⟨φ| = [b₁* b₂* ... bₙ*]
      [a₂]
      [⋮ ]
      [aₙ]

|ψ⟩⟨φ| = [a₁]             [a₁b₁* a₁b₂* ... a₁bₙ*]
         [a₂][b₁* b₂* ...bₙ*] = [a₂b₁* a₂b₂* ... a₂bₙ*]
         [⋮ ]             [⋮     ⋮         ⋮    ]
         [aₙ]             [aₙb₁* aₙb₂* ... aₙbₙ*]
```

**Rank-1 matrix!**

---

**Example Calculations:**

**Example 1: Basic Outer Products**
```
|0⟩⟨0| = [1][1 0] = [1 0]
         [0]        [0 0]

|1⟩⟨1| = [0][0 1] = [0 0]
         [1]        [0 1]

|0⟩⟨1| = [1][0 1] = [0 1]
         [0]        [0 0]

|1⟩⟨0| = [0][1 0] = [0 0]
         [1]        [1 0]
```

---

**Example 2: Superposition States**
```
|+⟩⟨+| where |+⟩ = (|0⟩+|1⟩)/√2

|+⟩⟨+| = ((|0⟩+|1⟩)/√2)((⟨0|+⟨1|)/√2)
       = (1/2)(|0⟩⟨0| + |0⟩⟨1| + |1⟩⟨0| + |1⟩⟨1|)
       = (1/2)([1 0] + [0 1] + [0 0] + [0 0])
              ([0 0]   [0 0]   [1 0]   [0 1])
       = (1/2)[1 1]
              [1 1]
```

---

**Properties:**

**1. Hermitian Conjugate:**
```
(|ψ⟩⟨φ|)† = |φ⟩⟨ψ|
```

**Proof:**
```
((|ψ⟩⟨φ|)|χ⟩, |η⟩) = (⟨φ|χ⟩|ψ⟩, |η⟩)
                    = ⟨φ|χ⟩⟨η|ψ⟩
                    = ⟨χ|φ⟩*⟨η|ψ⟩
                    = (|χ⟩, ⟨ψ|η⟩|φ⟩)
                    = (|χ⟩, |φ⟩⟨ψ|η⟩)
```

---

**2. Composition:**
```
(|ψ⟩⟨φ|)(|χ⟩⟨η|) = |ψ⟩⟨φ|χ⟩⟨η|
                  = ⟨φ|χ⟩|ψ⟩⟨η|  (scalar factor)
```

---

**3. Trace:**
```
Tr(|ψ⟩⟨φ|) = ⟨φ|ψ⟩
```

---

#### **Physical Significance of Outer Product:**

**1. Projection Operators:**

**Definition:**
```
Pψ = |ψ⟩⟨ψ|  (if ⟨ψ|ψ⟩ = 1)
```

**Properties:**
```
Pψ² = (|ψ⟩⟨ψ|)(|ψ⟩⟨ψ|)
    = |ψ⟩⟨ψ|ψ⟩⟨ψ|
    = |ψ⟩·1·⟨ψ|
    = Pψ  (Idempotent)

Pψ† = Pψ  (Hermitian)

Tr(Pψ) = 1
```

---

**Physical Meaning:**
```
Pψ|φ⟩ = |ψ⟩⟨ψ|φ⟩
       = ⟨ψ|φ⟩|ψ⟩

Projects |φ⟩ onto direction |ψ⟩
Component of |φ⟩ along |ψ⟩
```

**Example:**
```
|φ⟩ = (3/5)|0⟩ + (4/5)|1⟩
Project onto |0⟩:

P₀|φ⟩ = |0⟩⟨0|φ⟩
      = |0⟩·(3/5)
      = (3/5)|0⟩

Component along |0⟩ direction
```

---

**Measurement Interpretation:**
```
Measure observable with eigenstates {|ψₙ⟩}:
- Outcome n: Eigenvalue λₙ
- Post-measurement state: Pₙ|ψ⟩/||Pₙ|ψ⟩||
- Probability: ||Pₙ|ψ⟩||² = |⟨ψₙ|ψ⟩|²
```

---

**2. Density Matrices:**

**Pure State:**
```
ρ = |ψ⟩⟨ψ|
```

**Properties:**
```
ρ² = ρ (Pure)
Tr(ρ) = 1
ρ† = ρ (Hermitian)
```

**Physical Meaning:**
- Complete description of quantum state
- Expectation: ⟨A⟩ = Tr(ρA)

---

**Mixed State:**
```
ρ = Σᵢ pᵢ|ψᵢ⟩⟨ψᵢ|  (Statistical mixture)
```

**Properties:**
```
ρ² ≠ ρ (Mixed)
Tr(ρ²) < 1 (Purity measure)
```

**Example:**
```
50-50 mixture of |0⟩ and |1⟩:
ρ = 0.5|0⟩⟨0| + 0.5|1⟩⟨1|
  = 0.5[1 0] + 0.5[0 0]
      [0 0]       [0 1]
  = [0.5  0 ]
    [ 0  0.5]

Not pure superposition!
Classical uncertainty, not quantum.
```

---

**3. Operator Decomposition:**

**Completeness Relation:**
```
Σₙ |ψₙ⟩⟨ψₙ| = I

For orthonormal basis {|ψₙ⟩}
```

**Any Operator:**
```
A = Σₙₘ aₙₘ|ψₙ⟩⟨ψₘ|

Where:
aₙₘ = ⟨ψₙ|A|ψₘ⟩
```

---

**Example: Pauli-X Decomposition**
```
X = |0⟩⟨1| + |1⟩⟨0|

Verification:
X|0⟩ = (|0⟩⟨1| + |1⟩⟨0|)|0⟩
     = |0⟩⟨1|0⟩ + |1⟩⟨0|0⟩
     = 0 + |1⟩·1
     = |1⟩ ✓

X|1⟩ = |0⟩ ✓
```

---

**4. Quantum Gates as Outer Products:**

**Hadamard:**
```
H = (|0⟩⟨+| + |1⟩⟨−|) + (|0⟩⟨−| + |1⟩⟨+|)

Or equivalently:
H = (|0⟩ + |1⟩)⟨0|/√2 + (|0⟩ - |1⟩)⟨1|/√2
  = |+⟩⟨0| + |−⟩⟨1|
```

---

**CNOT:**
```
CNOT = |0⟩⟨0| ⊗ I + |1⟩⟨1| ⊗ X
     = |00⟩⟨00| + |01⟩⟨01| + |10⟩⟨11| + |11⟩⟨10|

Control on first qubit
Target flips if control = 1
```

---

**5. Entanglement Creation:**

**Bell State from Product:**
```
Start: |00⟩
Apply: (H ⊗ I) then CNOT

H ⊗ I: |00⟩ → (|0⟩+|1⟩)/√2 ⊗ |0⟩ = (|00⟩+|10⟩)/√2

CNOT: (|00⟩+|10⟩)/√2 → (|00⟩+|11⟩)/√2 = |Φ⁺⟩

Outer product view:
CNOT = (|00⟩⟨00| + |01⟩⟨01| + |10⟩⟨11| + |11⟩⟨10|)
```

---

#### **Summary Table:**

| Aspect | Inner Product ⟨φ|ψ⟩ | Outer Product |ψ⟩⟨φ| |
|--------|-------------------|-------------------|
| **Type** | Scalar (ℂ) | Operator (Matrix) |
| **Dimension** | 1×1 | n×n |
| **Physics** | Amplitude/Probability | Projection/Gate |
| **Hermitian** | ⟨ψ|φ⟩* | |φ⟩⟨ψ| |
| **Use** | Measurement probability | State transformation |

---

**Final Summary:**
- **Inner product:** ⟨φ|ψ⟩ = scalar (probability amplitude)
- **Outer product:** |ψ⟩⟨φ| = operator (transformation)
- Inner: Measure similarity/overlap
- Outer: Create projections/gates
- Both essential quantum mechanics tools
- Dirac notation makes calculations elegant
- Physical interpretations profound

---

### 16B. Quantum Gates as Operators - Dirac Notation

*(Content for this will be similar depth to 16A, but focusing on gate representations)*

**[Due to length constraints, key points outlined:]**

**Section 1: Operator Representation Basics**
- Gates as unitary matrices
- Dirac notation advantages
- Basis-independent representation

**Section 2: Single-Qubit Gates**
- Pauli gates: X = |0⟩⟨1| + |1⟩⟨0|
- Hadamard: H = |+⟩⟨0| + |−⟩⟨1|
- Phase gates: S, T operators

**Section 3: Multi-Qubit Gates**
- CNOT decomposition
- Tensor product structure
- Controlled operations general form

**Section 4: Gate Composition**
- Sequential operations
- Conjugation relations
- Universal gate sets

**Section 5: Physical Implementation**
- Hamiltonian evolution
- Time evolution operator
- Pulse sequences

---

## QUICK REVISION SUMMARY

**Key Formulas:**
```
Uncertainty: ΔxΔp ≥ ℏ/2
Inner product: ⟨φ|ψ⟩ = Σᵢ φᵢ*ψᵢ
Normalization: ⟨ψ|ψ⟩ = 1
Probability: P = |⟨φ|ψ⟩|²
```

**Important Concepts:**
- Wave-particle duality
- Hermitian operators → real eigenvalues
- Unitary gates → reversible
- Entanglement → non-separable
- Measurement → collapse

**Gates:**
- X: Bit flip
- Z: Phase flip
- H: Superposition
- CNOT: Entangle

**Exam Tips:**
1. Draw Bloch sphere diagrams
2. Show all calculation steps
3. Use Dirac notation properly
4. Explain physical significance
5. Give quantum computing examples

**All the best! 🌟**
