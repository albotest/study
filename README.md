# QUANTUM COMPUTING - SHORT NOTES (THANGLISH)

---

## PART-A (2 MARKS)

### 1. Hermitian Operators - Importance

**Why Important:**
- Real eigenvalues (measurement results real numbers)
- Physical observables represent (energy, momentum, position)
- Orthogonal eigenvectors (states distinguish pannalam)

---

### 2. Wave Nature - Experimental Observation

**Double-slit experiment:** Light interference pattern form aagum (bright & dark fringes) - wave behavior prove panrum.

---

### 3. Heisenberg Uncertainty Principle

**Statement:** "Position and momentum simultaneously exact-a measure panna mudiyaadhu."

**Formula:** ΔxΔp ≥ ℏ/2

---

### 4. Inner Product

**Definition:** Two vectors ku scalar value calculate panra operation.

**Notation:** ⟨ψ|φ⟩ = ψ₁*φ₁ + ψ₂*φ₂

**Use:** Probability calculate, orthogonality check

---

### 5. Pauli Gates (Two)

1. **Pauli-X:** |0⟩ → |1⟩, |1⟩ → |0⟩ (NOT gate)
2. **Pauli-Z:** |0⟩ → |0⟩, |1⟩ → -|1⟩ (Phase flip)

---

### 6. Hadamard Gate Function

**Function:** Superposition create panrum

**Action:**
- H|0⟩ = (|0⟩ + |1⟩)/√2 = |+⟩
- H|1⟩ = (|0⟩ - |1⟩)/√2 = |−⟩

---

### 7. Entanglement

**Definition:** Two qubits strongly correlated - one measure pannaa mathadu instant-a affect aagum.

**Example:** |Φ⁺⟩ = (|00⟩ + |11⟩)/√2

---

### 8. Bell States

**Four maximally entangled states:**
1. |Φ⁺⟩ = (|00⟩ + |11⟩)/√2
2. |Φ⁻⟩ = (|00⟩ - |11⟩)/√2
3. |Ψ⁺⟩ = (|01⟩ + |10⟩)/√2
4. |Ψ⁻⟩ = (|01⟩ - |10⟩)/√2

---

### 9. Dirac Notation

**Definition:** Quantum states represent panra notation.

**Two parts:**
- **Ket:** |ψ⟩ (state vector)
- **Bra:** ⟨ψ| (conjugate)

---

### 10. Ket Vector

**Definition:** Column vector representing quantum state.

**Example:**
```
|0⟩ = [1]    |1⟩ = [0]
      [0]          [1]
```

---

## PART-B (13 MARKS)

### 11A. Wave-Particle Duality & Observation

#### **Wave-Particle Duality:**
Light both wave and particle properties show panrum.

**Wave Evidence - Double Slit:**
```
Two slits → Interference pattern
Bright & dark fringes
Wave behavior
```

**Particle Evidence - Photoelectric Effect:**
- Light frequency increase → electron energy increase
- Intensity → number of electrons
- Photon (particle) concept
- E = hf

---

#### **Observation Effect:**

**No Detector:**
- Interference pattern visible
- Wave behavior
- Both slits through pass

**With Detector:**
- Pattern disappear
- Two bands only
- Particle behavior
- Wave function collapse

**Why:** Measurement process quantum state disturb panrum - superposition collapse aagum.

**Significance:** Observer reality-a affect panrum (quantum mechanics fundamental property).

---

### 11B. Uncertainty Principle

#### **Statement & Formula:**
```
ΔxΔp ≥ ℏ/2
ΔEΔt ≥ ℏ/2
```

**Meaning:** Position accurate-a measure → momentum uncertain, vice versa.

---

#### **Physical Significance:**

**1. Fundamental Limit:**
- Nature property (not instrument limitation)
- Cannot improve by better technology

**2. Wave-Particle Connection:**
- Wave spread out → position uncertain
- Single wavelength → momentum certain but position uncertain

**3. Atom Stability:**
- Electron nucleus close → Δx small → Δp large → high energy
- Prevents collapse into nucleus

**4. Examples:**
- Ground state energy always positive (zero-point energy)
- Quantum tunneling possible

---

### 12A. Vector Spaces in Quantum

#### **Concept:**
Quantum states = Vectors in Hilbert space with operations (addition, scalar multiplication).

**Why Use:** Superposition naturally represent pannalam.

---

#### **Basis & Dimension:**

**Single Qubit:**
```
Basis: |0⟩, |1⟩
Dimension: 2
Any state: |ψ⟩ = α|0⟩ + β|1⟩
Normalization: |α|² + |β|² = 1
```

**Two Qubits:**
```
Basis: |00⟩, |01⟩, |10⟩, |11⟩
Dimension: 4
n qubits → 2ⁿ dimensions
```

---

#### **Different Bases:**

**Computational (Z-basis):**
```
|0⟩, |1⟩
```

**Hadamard (X-basis):**
```
|+⟩ = (|0⟩+|1⟩)/√2
|−⟩ = (|0⟩-|1⟩)/√2
```

**Example:** Spin-½ particle, qutrit (3-level system)

---

### 12B. Inner Product Role

#### **Definition:**
```
⟨φ|ψ⟩ = φ₁*ψ₁ + φ₂*ψ₂
```

---

#### **Three Main Roles:**

**1. Probabilities (Born Rule):**
```
P(measure |φ⟩) = |⟨φ|ψ⟩|²

Example:
|ψ⟩ = (3/5)|0⟩ + (4/5)|1⟩
P(0) = |⟨0|ψ⟩|² = |3/5|² = 9/25
```

**2. Normalization:**
```
⟨ψ|ψ⟩ = 1 required
Total probability = 1
```

**3. Orthogonality:**
```
⟨φ|ψ⟩ = 0 → orthogonal
Distinguishable states
```

---

### 13A. Postulates of Quantum Computing

#### **Postulate 1: State Space**
Any quantum system 2ⁿ dimensional Hilbert space. State |ψ⟩ unit vector.

**Single qubit:** |ψ⟩ = α|0⟩ + β|1⟩

---

#### **Postulate 2: Evolution**
Evolution unitary: |ψ(t₂)⟩ = U|ψ(t₁)⟩

**Properties:**
- U†U = I (unitary)
- Reversible
- Norm preserving

**Example:** H|0⟩ = |+⟩, H² = I

---

#### **Postulate 3: Measurement**
Measurement operators {Mₘ}, probability: p(m) = ⟨ψ|Mₘ†Mₘ|ψ⟩

**Computational basis:**
```
P(0) = |α|²
P(1) = |β|²
Post-measurement: collapse to |0⟩ or |1⟩
```

---

#### **Postulate 4: Composite Systems**
Two systems tensor product: H₁ ⊗ H₂

**Example:**
```
|ψ⟩ ⊗ |φ⟩ = (α|0⟩+β|1⟩) ⊗ (γ|0⟩+δ|1⟩)
         = αγ|00⟩ + αδ|01⟩ + βγ|10⟩ + βδ|11⟩
```

**Entanglement:** Cannot write as product.

---

### 13B. Bloch Sphere

#### **Representation:**
```
|ψ⟩ = cos(θ/2)|0⟩ + e^(iφ)sin(θ/2)|1⟩
```

**Parameters:** θ (polar), φ (azimuthal)

---

#### **Special Points:**
```
|0⟩: North pole (θ=0)
|1⟩: South pole (θ=π)
|+⟩: +X axis (θ=π/2, φ=0)
|−⟩: -X axis (θ=π/2, φ=π)
```

---

#### **Gate Actions:**
- **X:** π rotation around X-axis
- **Z:** π rotation around Z-axis
- **H:** π rotation around (X+Z)/√2 axis

**Use:** Visualize single qubit states & operations.

---

### 14A. Single-Qubit Gates

#### **Pauli-X (NOT):**
```
X = [0 1]    X|0⟩ = |1⟩
    [1 0]    X|1⟩ = |0⟩
```

#### **Pauli-Z (Phase):**
```
Z = [1  0]   Z|0⟩ = |0⟩
    [0 -1]   Z|1⟩ = -|1⟩
```

#### **Hadamard:**
```
H = (1/√2)[1  1]
           [1 -1]

H|0⟩ = |+⟩
H|1⟩ = |−⟩
H² = I (self-inverse)
```

**Use:** X (bit flip), Z (phase flip), H (superposition)

---

### 14B. Bell States

#### **Two-Qubit States:**
General: |ψ⟩ = α₀₀|00⟩ + α₀₁|01⟩ + α₁₀|10⟩ + α₁₁|11⟩

**Separable:** Can write as |ψ₁⟩ ⊗ |ψ₂⟩  
**Entangled:** Cannot separate

---

#### **Bell States (Maximally Entangled):**
```
|Φ⁺⟩ = (|00⟩ + |11⟩)/√2  (correlated)
|Φ⁻⟩ = (|00⟩ - |11⟩)/√2  (phase)
|Ψ⁺⟩ = (|01⟩ + |10⟩)/√2  (anti-correlated)
|Ψ⁻⟩ = (|01⟩ - |10⟩)/√2  (singlet)
```

---

#### **Properties:**
- Orthonormal basis
- Maximal entanglement
- Measure one → other determined instantly

**Applications:**
- Quantum teleportation
- Cryptography (BB84)
- Bell's theorem violation

---

### 15A. Dirac Notation

#### **Bra-Ket:**
```
|ψ⟩ = ket (column vector)
⟨ψ| = bra (row vector, conjugate)
```

---

#### **Operations:**

**Inner Product (scalar):**
```
⟨φ|ψ⟩ = φ₁*ψ₁ + φ₂*ψ₂
```

**Outer Product (operator):**
```
|ψ⟩⟨φ| = matrix

Example:
|0⟩⟨0| = [1 0]
         [0 0]
```

---

#### **Uses:**

**Expectation Value:**
```
⟨A⟩ = ⟨ψ|A|ψ⟩
```

**Probability:**
```
P = |⟨φ|ψ⟩|²
```

**Projection:**
```
|ψ⟩⟨ψ| = projection operator
```

---

### 15B. Computational Basis

#### **Definition:**
```
|0⟩ = [1]    |1⟩ = [0]
      [0]          [1]
```

**Multi-qubit:** |00⟩, |01⟩, |10⟩, |11⟩ (2ⁿ basis states)

---

#### **Orthonormal Properties:**

**Normalization:**
```
⟨0|0⟩ = 1
⟨1|1⟩ = 1
```

**Orthogonality:**
```
⟨0|1⟩ = 0
⟨1|0⟩ = 0
```

**Kronecker Delta:** ⟨i|j⟩ = δᵢⱼ

---

#### **Completeness:**
```
|0⟩⟨0| + |1⟩⟨1| = I

Any state:
|ψ⟩ = ⟨0|ψ⟩|0⟩ + ⟨1|ψ⟩|1⟩
```

**Importance:**
- Standard measurement basis
- Probability = |⟨i|ψ⟩|²
- Unique state expansion

---

## PART-C (20 MARKS)

### 16A. Inner & Outer Products

#### **INNER PRODUCT:**

**Definition:** ⟨φ|ψ⟩ = Σᵢ φᵢ*ψᵢ (complex scalar)

**Properties:**
1. Linearity: ⟨φ|(α|ψ₁⟩+β|ψ₂⟩) = α⟨φ|ψ₁⟩ + β⟨φ|ψ₂⟩
2. Conjugate symmetry: ⟨φ|ψ⟩ = ⟨ψ|φ⟩*
3. Positive: ⟨ψ|ψ⟩ ≥ 0

---

#### **Physical Significance:**

**1. Probability Amplitude:**
```
P(measure |φ⟩) = |⟨φ|ψ⟩|²

Example:
|ψ⟩ = (√3/2)|0⟩ + (1/2)|1⟩
|+⟩ = (|0⟩+|1⟩)/√2

⟨+|ψ⟩ = (1/√2)(√3/2 + 1/2) = (√3+1)/(2√2)
P(+) = (4+2√3)/8 ≈ 0.93
```

---

**2. State Overlap:**
- |⟨φ|ψ⟩| = similarity
- 0 = orthogonal (different)
- 1 = parallel (same)

---

**3. Expectation Value:**
```
⟨A⟩ = ⟨ψ|A|ψ⟩

Example (Pauli-Z):
|ψ⟩ = cos(θ/2)|0⟩ + sin(θ/2)|1⟩
⟨Z⟩ = cos²(θ/2) - sin²(θ/2) = cos(θ)
```

---

#### **OUTER PRODUCT:**

**Definition:** |ψ⟩⟨φ|: V → V (linear operator, matrix)

**Action:** (|ψ⟩⟨φ|)|χ⟩ = ⟨φ|χ⟩|ψ⟩

---

**Matrix Form:**
```
|0⟩⟨0| = [1 0]    |1⟩⟨1| = [0 0]
         [0 0]              [0 1]

|0⟩⟨1| = [0 1]    |1⟩⟨0| = [0 0]
         [0 0]              [1 0]
```

---

#### **Physical Significance:**

**1. Projection Operators:**
```
Pψ = |ψ⟩⟨ψ|
Pψ² = Pψ (idempotent)

Projects |φ⟩ onto |ψ⟩:
Pψ|φ⟩ = |ψ⟩⟨ψ|φ⟩ = ⟨ψ|φ⟩|ψ⟩
```

**Use in Measurement:**
- Measurement outcome probability: ||Pₙ|ψ⟩||²
- Post-measurement state: Pₙ|ψ⟩/||Pₙ|ψ⟩||

---

**2. Density Matrices:**
```
Pure state: ρ = |ψ⟩⟨ψ|
Mixed state: ρ = Σᵢ pᵢ|ψᵢ⟩⟨ψᵢ|

Properties:
ρ² = ρ (pure)
Tr(ρ) = 1
⟨A⟩ = Tr(ρA)
```

---

**3. Operator Decomposition:**
```
Completeness: Σₙ |ψₙ⟩⟨ψₙ| = I

Any operator:
A = Σₙₘ aₙₘ|ψₙ⟩⟨ψₘ|
where aₙₘ = ⟨ψₙ|A|ψₘ⟩
```

**Example:**
```
X = |0⟩⟨1| + |1⟩⟨0|
Z = |0⟩⟨0| - |1⟩⟨1|
H = |+⟩⟨0| + |−⟩⟨1|
```

---

**4. Gate Construction:**
```
CNOT = |0⟩⟨0| ⊗ I + |1⟩⟨1| ⊗ X
     = |00⟩⟨00| + |01⟩⟨01| + |10⟩⟨11| + |11⟩⟨10|

Controlled-U = |0⟩⟨0| ⊗ I + |1⟩⟨1| ⊗ U
```

---

#### **Summary Table:**

| Aspect | Inner ⟨φ|ψ⟩ | Outer |ψ⟩⟨φ| |
|--------|------------|------------|
| Type | Scalar | Operator |
| Dimension | 1×1 | n×n |
| Physics | Amplitude | Transformation |
| Use | Probability | Projection/Gates |

---

### 16B. Quantum Gates as Operators (Dirac Form)

#### **Single-Qubit Gates:**

**Pauli Gates:**
```
X = |0⟩⟨1| + |1⟩⟨0|  (swap)
Y = i(|1⟩⟨0| - |0⟩⟨1|)  (complex swap)
Z = |0⟩⟨0| - |1⟩⟨1|  (phase)
```

**Verification:**
```
X|0⟩ = (|0⟩⟨1| + |1⟩⟨0|)|0⟩
     = |0⟩⟨1|0⟩ + |1⟩⟨0|0⟩
     = 0 + |1⟩·1 = |1⟩ ✓
```

---

**Hadamard:**
```
H = (|0⟩ + |1⟩)⟨0|/√2 + (|0⟩ - |1⟩)⟨1|/√2
  = |+⟩⟨0| + |−⟩⟨1|

Or:
H = (|0⟩⟨0| + |0⟩⟨1| + |1⟩⟨0| - |1⟩⟨1|)/√2
```

---

**Phase Gates:**
```
S = |0⟩⟨0| + i|1⟩⟨1|  (π/2 phase)
T = |0⟩⟨0| + e^(iπ/4)|1⟩⟨1|  (π/4 phase)
```

---

#### **Two-Qubit Gates:**

**CNOT:**
```
CNOT = |00⟩⟨00| + |01⟩⟨01| + |10⟩⟨11| + |11⟩⟨10|
     = |0⟩⟨0| ⊗ I + |1⟩⟨1| ⊗ X

Control = |0⟩: target unchanged
Control = |1⟩: target flipped
```

---

**SWAP:**
```
SWAP = |00⟩⟨00| + |01⟩⟨10| + |10⟩⟨01| + |11⟩⟨11|
```

---

**Controlled-U:**
```
C-U = |0⟩⟨0| ⊗ I + |1⟩⟨1| ⊗ U

General form for controlled operations
```

---

#### **Gate Composition:**

**Sequential:**
```
BA|ψ⟩ (apply A first, then B)

Example: HXH
HXH = H(|0⟩⟨1| + |1⟩⟨0|)H
    = ... = Z (basis conjugation)
```

---

**Tensor Product:**
```
H ⊗ X applied to |ψ⟩ ⊗ |φ⟩
= H|ψ⟩ ⊗ X|φ⟩
```

---

#### **Universal Gate Set:**
```
{H, T, CNOT} = universal
Any unitary can be approximated

Or: {H, S, CNOT, T}
```

---

#### **Physical Implementation:**

**Time Evolution:**
```
U(t) = e^(-iHt/ℏ)

Example: Single qubit rotation
Rx(θ) = e^(-iθX/2) = cos(θ/2)I - i sin(θ/2)X
```

---

**Hamiltonian Engineering:**
Design H such that U(t) = desired gate at specific time.

**Example:**
```
H = (ℏω/2)X → Rx(ωt) rotation
```

---

#### **Gate Relations:**
```
XZ = -ZX (anti-commute)
HXH = Z
HZH = X
XYZ = iI
```

---

## QUICK REVISION

**Key Formulas:**
```
Uncertainty: ΔxΔp ≥ ℏ/2
Probability: P = |⟨φ|ψ⟩|²
Normalization: ⟨ψ|ψ⟩ = 1
Inner: ⟨φ|ψ⟩ (scalar)
Outer: |ψ⟩⟨φ| (operator)
```

**Gates:**
```
X: |0⟩⟨1| + |1⟩⟨0|
Z: |0⟩⟨0| - |1⟩⟨1|
H: |+⟩⟨0| + |−⟩⟨1|
```

**Postulates:**
1. State = Hilbert space vector
2. Evolution = Unitary
3. Measurement = Collapse
4. Composite = Tensor product

**Exam Tips:**
1. Bloch sphere diagram draw
2. Mathematical steps show
3. Physical meaning explain
4. Examples mandatory
5. Dirac notation properly use

**All the best! 🌟**
