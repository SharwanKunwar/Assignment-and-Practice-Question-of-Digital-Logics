# Assignment-and-Practice-Question-of-Digital-Logics

# Unit-3: Combinational Logic Design

## 1. Logic Gates
**Definition**: Logic gates are the fundamental building blocks of digital circuits, used to perform logical operations on one or more binary inputs to produce a single output.

### Basic Logic Gates:
#### AND Gate
- **Logic Symbol**: A flat-ended shape with two or more inputs.
- **Logic Expression**: \( A \cdot B \)
- **Truth Table**:

| A | B | Output (A·B) |
|---|---|--------------|
| 0 | 0 | 0            |
| 0 | 1 | 0            |
| 1 | 0 | 0            |
| 1 | 1 | 1            |

- **Venn Diagram**: Represents the intersection of two sets.
- **Timing Diagram**: Shows the output for varying input changes over time.

#### OR Gate
- **Logic Symbol**: A curved shape with two or more inputs.
- **Logic Expression**: \( A + B \)
- **Truth Table**:

| A | B | Output (A + B) |
|---|---|----------------|
| 0 | 0 | 0              |
| 0 | 1 | 1              |
| 1 | 0 | 1              |
| 1 | 1 | 1              |

- **Venn Diagram**: Represents the union of two sets.
- **Timing Diagram**: Shows the output for varying input changes over time.

#### NOT Gate
- **Logic Symbol**: A triangle with a circle at the output.
- **Logic Expression**: \( \overline{A} \)
- **Truth Table**:

| A | Output (¬A) |
|---|-------------|
| 0 | 1           |
| 1 | 0           |

- **Venn Diagram**: Represents the complement of a set.
- **Timing Diagram**: Shows the output for varying input changes over time.

## 2. NAND and NOR Gates as Universal Gates
### NAND Gate:
- **Definition**: A NAND gate is the inverse of an AND gate, producing an output that is false only when all inputs are true.
- **Logic Symbol**: Same as AND gate but with a small circle at the output.
- **Logic Expression**: \( \overline{A \cdot B} \)
- **Truth Table**:

| A | B | Output (A NAND B) |
|---|---|-------------------|
| 0 | 0 | 1                 |
| 0 | 1 | 1                 |
| 1 | 0 | 1                 |
| 1 | 1 | 0                 |

- **Venn Diagram**: Represents the complement of the intersection of two sets.
- **Timing Diagram**: Shows the output for varying input changes over time.

### NOR Gate:
- **Definition**: A NOR gate is the inverse of an OR gate, producing an output that is true only when all inputs are false.
- **Logic Symbol**: Same as OR gate but with a small circle at the output.
- **Logic Expression**: \( \overline{A + B} \)
- **Truth Table**:

| A | B | Output (A NOR B) |
|---|---|------------------|
| 0 | 0 | 1                |
| 0 | 1 | 0                |
| 1 | 0 | 0                |
| 1 | 1 | 0                |

- **Venn Diagram**: Represents the complement of the union of two sets.
- **Timing Diagram**: Shows the output for varying input changes over time.

### Why called Universal Gates:
Both NAND and NOR gates can be used to construct any other logic gate (AND, OR, NOT), making them "universal."

## 3. Realize Basic Gates Using NAND and NOR Gates
- **AND Gate**: Implemented using a NAND gate followed by a NOT gate.
- **OR Gate**: Implemented using a NOR gate followed by a NOT gate.
- **NOT Gate**: Implemented by using a NAND gate with both inputs connected to the same variable.

## 4. XOR and XNOR Gates
### XOR Gate (Exclusive OR):
- **Logic Symbol**: OR gate symbol with an additional curved line on the input side.
- **Logic Expression**: \( A \oplus B \)
- **Truth Table**:

| A | B | Output (A XOR B) |
|---|---|------------------|
| 0 | 0 | 0                |
| 0 | 1 | 1                |
| 1 | 0 | 1                |
| 1 | 1 | 0                |

- **Venn Diagram**: Represents the symmetric difference of two sets.
- **Timing Diagram**: Shows the output for varying input changes over time.

### XNOR Gate (Exclusive NOR):
- **Logic Symbol**: XOR gate symbol with a small circle at the output.
- **Logic Expression**: \( A \odot B \)
- **Truth Table**:

| A | B | Output (A XNOR B) |
|---|---|-------------------|
| 0 | 0 | 1                 |
| 0 | 1 | 0                 |
| 1 | 0 | 0                 |
| 1 | 1 | 1                 |

- **Venn Diagram**: Represents the complement of the symmetric difference of two sets.
- **Timing Diagram**: Shows the output for varying input changes over time.

## 5. Boolean Terms
- **Boolean Variables**: Variables that take binary values (0 or 1).
- **Boolean Functions**: Functions that map Boolean variables to an output value (0 or 1).
- **Boolean Expressions**: Algebraic expressions involving Boolean variables, constants, and operations like AND, OR, NOT.
- **Boolean Algebra**: A mathematical structure used to model logical operations and simplify Boolean expressions.

## 6. Difference Between Boolean Algebra and Ordinary Algebra
- **Boolean Algebra**: Deals with binary values (0 and 1) and operations like AND, OR, and NOT. It is used for logic simplification and digital circuit design.
- **Ordinary Algebra**: Involves real numbers and operations like addition, subtraction, multiplication, and division, focusing on general mathematical functions.

## 7. Boolean Identities and Postulates

### Boolean Identities:
1. **Identity Law:**
   - \( A + 0 = A \)
   - \( A \cdot 1 = A \)
   
2. **Null Law:**
   - \( A + 1 = 1 \)
   - \( A \cdot 0 = 0 \)
   
3. **Complement Law:**
   - \( A + A' = 1 \)
   - \( A \cdot A' = 0 \)
   
4. **Idempotent Law:**
   - \( A + A = A \)
   - \( A \cdot A = A \)
   
5. **Domination Law:**
   - \( A + 1 = 1 \)
   - \( A \cdot 0 = 0 \)
   
6. **Double Negation Law:**
   - \( (A')' = A \)
   
7. **Commutative Law:**
   - \( A + B = B + A \)
   - \( A \cdot B = B \cdot A \)
   
8. **Associative Law:**
   - \( A + (B + C) = (A + B) + C \)
   - \( A \cdot (B \cdot C) = (A \cdot B) \cdot C \)
   
9. **Distributive Law:**
   - \( A \cdot (B + C) = (A \cdot B) + (A \cdot C) \)
   - \( A + (B \cdot C) = (A + B) \cdot (A + C) \)
   
10. **Absorption Law:**
    - \( A + A \cdot B = A \)
    - \( A \cdot (A + B) = A \)

### Boolean Postulates:
1. \( A \cdot B = B \cdot A \) (Commutative Property)
2. \( A \cdot (B \cdot C) = (A \cdot B) \cdot C \) (Associative Property)
3. \( A + (B + C) = (A + B) + C \) (Associative Property)
4. \( A + B = B + A \) (Commutative Property)
5. \( A \cdot (B + C) = (A \cdot B) + (A \cdot C) \) (Distributive Property)

## 8. De-Morgan’s Theorem

### De-Morgan’s Theorem states:
1. \( (A \cdot B)' = A' + B' \)
2. \( (A + B)' = A' \cdot B' \)

### Proof:
1. For \( (A \cdot B)' = A' + B' \):
   - Let’s assume that \( A \cdot B = 1 \). Then \( (A \cdot B)' = 0 \).
   - Therefore, \( A' + B' = 0 \) holds true.
   - Hence, \( (A \cdot B)' = A' + B' \).

2. For \( (A + B)' = A' \cdot B' \):
   - Let’s assume that \( A + B = 1 \). Then \( (A + B)' = 0 \).
   - Therefore, \( A' \cdot B' = 0 \) holds true.
   - Hence, \( (A + B)' = A' \cdot B' \).

## 9. Principle of Duality

The principle of duality states that every Boolean expression has a dual, where:
- The operations \( + \) and \( \cdot \) are interchanged.
- The constants 0 and 1 are swapped.

### Example:
- The dual of \( A + B \cdot C \) is \( A \cdot B + C \).

## 10. Definitions

1. **Minterm:** A minterm is a product (AND operation) of all variables in the Boolean expression, each of which appears in true or complemented form. Example: \( A \cdot B' \cdot C \).
   
2. **Maxterm:** A maxterm is a sum (OR operation) of all variables, each of which appears in true or complemented form. Example: \( A + B' + C \).

3. **SOP (Sum of Products):** An expression that is the sum (OR) of several products (ANDs) of variables. Example: \( (A \cdot B) + (A' \cdot C) \).

4. **POS (Product of Sums):** An expression that is the product (AND) of several sums (ORs) of variables. Example: \( (A + B) \cdot (C + D) \).

## 11. Solving Boolean Expressions Using Formula Method

### a. Expression: \( xy + xy' \)
   - **Solution:** Factor out \( x \):
     \[
     xy + xy' = x(y + y') = x \cdot 1 = x
     \]

### b. Expression: \( (A + B)'(A' + B)' \)
   - **Solution:** Apply De-Morgan’s theorem:
     \[
     (A + B)'(A' + B)' = A'B' \cdot AB = 0
     \]

### c. Expression: \( ABC + A'B'C + A'BC + ABC' + A'B'C' \)
   - **Solution:** Simplify using combining terms:
     \[
     ABC + A'BC + A'B'C + ABC' + A'B'C' = BC + A'B'C + A'B'C' = BC + A'B'
     \]

### d. Expression: \( AC' + B'D + A'CD + ABCD \)
   - **Solution:** Simplify by combining terms:
     \[
     AC' + B'D + A'CD + ABCD = AC' + B'D + A'CD
     \]

### e. Expression: \( (A' + B' + D')(A + B' + C')(A' + B + D')(B + C' + D') \)
   - **Solution:** Simplify step by step using distribution and combining terms.

### f. Prove: \( A(A'C)(A'B + C)(A'BC + C') = 0 \)
   - **Solution:** Using the distributive property:
     \[
     A(A'C)(A'B + C)(A'BC + C') = 0
     \]

## 12. Converting Boolean Expressions into Standard POS Form

### a. Expression: \( (A + B')(B + C) \)
   - **Solution:** Apply distributive law to get the POS form:
     \[
     (A + B')(B + C) = (A + B' + C)(A + B' + B)
     \]

### b. Expression: \( (A + B' + C)(B' + C + D')(A + B' + C' + D) \)
   - **Solution:** Expand using distributive law:
     \[
     (A + B' + C)(B' + C + D')(A + B' + C' + D)
     \]

## 13. Convert Boolean Expressions into Standard SOP Form

### a. \( AB'C + A'B' + ABC'D \)
   - **Solution:**
     The given expression is already in SOP form:
     \[
     AB'C + A'B' + ABC'D
     \]

### b. \( WX'Y + X'YZ' + WXY' \)
   - **Solution:**
     The given expression is already in SOP form:
     \[
     WX'Y + X'YZ' + WXY'
     \]

## 14. Convert Between SOP and POS Forms

### a. \( F(x, y, z) = \sum(1, 3, 7) \)
   - **Solution:** Convert from SOP to POS:
     \[
     F(x, y, z) = (x + y' + z)(x' + y + z')(x' + y' + z')
     \]

### b. \( F(A, B, C, D) = \sum(0, 2, 6, 11, 13, 14) \)
   - **Solution:** Convert from SOP to POS:
     \[
     F(A, B, C, D) = (A + B + C + D)(A + B' + C' + D')(A' + B' + C + D)(A' + B + C' + D')
     \]

### c. \( F(x, y, z) = \pi(0, 3, 6, 7) \)
   - **Solution:** Convert from POS to SOP:
     \[
     F(x, y, z) = x' \cdot y' \cdot z + x \cdot y' \cdot z'
     \]

### d. \( F(A, B, C, D) = \pi(0, 1, 2, 3, 6, 12) \)
   - **Solution:** Convert from POS to SOP:
     \[
     F(A, B, C, D) = A'B'C'D' + A'B'C'D + AB'C'D + AB'CD'
     \]

## 15. K-Map: Pair, Quad, and Octet

### Definitions:
- **Pair:** A group of two adjacent 1s or 0s in a K-map.
- **Quad:** A group of four adjacent 1s or 0s in a K-map.
- **Octet:** A group of eight adjacent 1s or 0s in a K-map.

### Simplifying Boolean Expressions Using K-Map:

### a. \( F(w, x, y, z) = \sum(2, 3, 12, 13, 14, 15) \)
   - **Solution:** Simplify the expression using K-map.

### b. \( F(A, B, C, D) = \pi(0, 1, 2, 3, 4, 10, 11) \)
   - **Solution:** Simplify the expression using K-map.

### c. \( F(w, x, y, z) = \sum(1, 3, 7, 11, 15) \) with don’t care conditions: \( D(w, x, y, z) = \sum(0, 2, 5) \)
   - **Solution:** Simplify the expression using K-map with don’t care conditions.

### d. \( F(A, B, C, D) = \pi(2, 3, 4, 5, 7, 9, 10) \) with don’t care conditions: \( D(A, B, C, D) = \pi(0, 6, 11) \)
   - **Solution:** Simplify the expression using K-map with don’t care conditions.

## 16. Combinational Circuit

A **combinational circuit** is a type of digital circuit whose output depends solely on the current input values. There are no memory elements involved.

### Combinational Circuit Design Procedure:
1. **Define the problem:** Understand the required logic and functionality.
2. **Write the truth table:** Define the inputs and corresponding outputs.
3. **Simplify the Boolean expression:** Use Boolean algebra or K-map for simplification.
4. **Draw the circuit diagram:** Using logic gates (AND, OR, NOT, etc.).
5. **Verify the design:** Ensure the circuit meets the required specifications.

## 17. Half Adder and Full Adder Design

### Half Adder:
- **Truth Table:**
  | A | B | Sum | Carry |
  |---|---|-----|-------|
  | 0 | 0 |  0  |   0   |
  | 0 | 1 |  1  |   0   |
  | 1 | 0 |  1  |   0   |
  | 1 | 1 |  0  |   1   |

- **Boolean Expressions:**
  - Sum: \( A \oplus B \)
  - Carry: \( A \cdot B \)

- **Logic Diagram:**
  - Use XOR gate for Sum and AND gate for Carry.

### Full Adder:
- **Truth Table:**
  | A | B | Cin | Sum | Cout |
  |---|---|-----|-----|------|
  | 0 | 0 |  0  |  0  |   0  |
  | 0 | 1 |  0  |  1  |   0  |
  | 1 | 0 |  0  |  1  |   0  |
  | 1 | 1 |  0  |  0  |   1  |
  | 0 | 0 |  1  |  1  |   0  |
  | 0 | 1 |  1  |  0  |   1  |
  | 1 | 0 |  1  |  0  |   1  |
  | 1 | 1 |  1  |  1  |   1  |

- **Boolean Expressions:**
  - Sum: \( A \oplus B \oplus Cin \)
  - Carry: \( (A \cdot B) + (Cin \cdot (A \oplus B)) \)

- **Logic Diagram:**
  - Use XOR gates for Sum and AND/OR gates for Carry.

## 18. Half Subtractor and Full Subtractor Design

### Half Subtractor:
- **Truth Table:**
  | A | B | Difference | Borrow |
  |---|---|------------|--------|
  | 0 | 0 |     0      |    0   |
  | 0 | 1 |     1      |    1   |
  | 1 | 0 |     1      |    0   |
  | 1 | 1 |     0      |    0   |

- **Boolean Expressions:**
  - Difference: \( A \oplus B \)
  - Borrow: \( A' \cdot B \)

- **Logic Diagram:**
  - Use XOR gate for Difference and AND gate for Borrow.

### Full Subtractor:
- **Truth Table:**
  | A | B | Bin | Difference | Borrow |
  |---|---|-----|------------|--------|
  | 0 | 0 |  0  |     0      |    0   |
  | 0 | 1 |  0  |     1      |    1   |
  | 1 | 0 |  0  |     1      |    0   |
  | 1 | 1 |  0  |     0      |    0   |
  | 0 | 0 |  1  |     1      |    1   |
  | 0 | 1 |  1  |     0      |    1   |
  | 1 | 0 |  1  |     0      |    0   |
  | 1 | 1 |  1  |     1      |    1   |

- **Boolean Expressions:**
  - Difference: \( A \oplus B \oplus Bin \)
  - Borrow: \( (A' \cdot B) + (Bin \cdot (A' + B)) \)

- **Logic Diagram:**
  - Use XOR gates for Difference and AND/OR gates for Borrow.

## 19. Decoder Design

### 2:4 Decoder:
- **Block Diagram:**
  A decoder with 2 input lines and 4 output lines.

- **Truth Table:**
  | A | B | Y0 | Y1 | Y2 | Y3 |
  |---|---|----|----|----|----|
  | 0 | 0 |  1 |  0 |  0 |  0 |
  | 0 | 1 |  0 |  1 |  0 |  0 |
  | 1 | 0 |  0 |  0 |  1 |  0 |
  | 1 | 1 |  0 |  0 |  0 |  1 |

- **Mathematical Expression:**
  \[
  Y0 = A'B', Y1 = A'B, Y2 = AB', Y3 = AB
  \]

### Circuit Diagram:
- Use AND gates for each output and connect the inputs accordingly.

### 20. Design a 3:8 Line Decoder, 4:2 Encoder, Priority Encoder, and more
(Continue similar pattern for each of the remaining designs...)






## 21. BCD to Decimal Decoder Design

### Block Diagram:
A **BCD to Decimal Decoder** takes a 4-bit Binary Coded Decimal (BCD) input and converts it into a 10-line output corresponding to the decimal digits 0-9.

### Truth Table:

| BCD Input (A, B, C, D) | Decimal Output (Y0 to Y9) |
|------------------------|---------------------------|
| 0000                   | 0000000001                |
| 0001                   | 0000000010                |
| 0010                   | 0000000100                |
| 0011                   | 0000001000                |
| 0100                   | 0000010000                |
| 0101                   | 0000100000                |
| 0110                   | 0001000000                |
| 0111                   | 0010000000                |
| 1000                   | 0100000000                |
| 1001                   | 1000000000                |

### Circuit Diagram:
The decoder uses AND gates to select one of the 10 outputs based on the 4-bit input.

### Mathematical Expression:
\[
Y_0 = A'B'C'D', Y_1 = A'B'C'D, Y_2 = A'B'CD', \dots, Y_9 = ABCD
\]

## 22. 4:16 Line Decoder (Binary to Hexadecimal Converter)

### Block Diagram:
A **4:16 Decoder** converts a 4-bit binary input to one of 16 output lines.

### Truth Table:

| A | B | C | D | Output (Y0 to Y15) |
|---|---|---|---|--------------------|
| 0 | 0 | 0 | 0 | 0000000000000001    |
| 0 | 0 | 0 | 1 | 0000000000000010    |
| 0 | 0 | 1 | 0 | 0000000000000100    |
| 0 | 0 | 1 | 1 | 0000000000001000    |
| 0 | 1 | 0 | 0 | 0000000000010000    |
| 0 | 1 | 0 | 1 | 0000000000100000    |
| 0 | 1 | 1 | 0 | 0000000001000000    |
| 0 | 1 | 1 | 1 | 0000000010000000    |
| 1 | 0 | 0 | 0 | 0000000100000000    |
| 1 | 0 | 0 | 1 | 0000001000000000    |
| 1 | 0 | 1 | 0 | 0000010000000000    |
| 1 | 0 | 1 | 1 | 0000100000000000    |
| 1 | 1 | 0 | 0 | 0001000000000000    |
| 1 | 1 | 0 | 1 | 0010000000000000    |
| 1 | 1 | 1 | 0 | 0100000000000000    |
| 1 | 1 | 1 | 1 | 1000000000000000    |

### Circuit Diagram:
Use 16 AND gates for each output line and select the corresponding line based on the input combination.

### Mathematical Expression:
\[
Y_0 = A'B'C'D', Y_1 = A'B'C'D, Y_2 = A'B'CD', \dots, Y_{15} = ABCD
\]

## 23. Encoder Definition and Design (4:2 Encoder)

### Definition:
An **Encoder** is a combinational circuit that converts an active input line into a binary code.

### Block Diagram:
A **4:2 Encoder** has 4 input lines and 2 output lines.

### Truth Table:

| Input | Output |
|-------|--------|
| 0001  | 00     |
| 0010  | 01     |
| 0100  | 10     |
| 1000  | 11     |

### Circuit Diagram:
The circuit consists of OR gates that combine the appropriate inputs to generate the binary output.

### Mathematical Expression:
\[
Y_0 = A + B, \quad Y_1 = C + D
\]

## 24. 8:3 Encoder (Octal to Binary Converter)

### Block Diagram:
An **8:3 Encoder** has 8 input lines and 3 output lines.

### Truth Table:

| Input | Output |
|-------|--------|
| 00000001 | 000 |
| 00000010 | 001 |
| 00000100 | 010 |
| 00001000 | 011 |
| 00010000 | 100 |
| 00100000 | 101 |
| 01000000 | 110 |
| 10000000 | 111 |

### Circuit Diagram:
Use OR gates to generate the binary output corresponding to the highest active input line.

### Mathematical Expression:
\[
Y_0 = A + B + C, \quad Y_1 = D + E + F, \quad Y_2 = G + H
\]

## 25. Priority Encoder Definition and Design (4:2 Priority Encoder)

### Definition:
A **Priority Encoder** is an encoder that gives the highest-priority active input as the output.

### Block Diagram:
A **4:2 Priority Encoder** has 4 input lines and 2 output lines, with priority given to the highest input.

### Truth Table:

| Input | Output |
|-------|--------|
| 0001  | 00     |
| 0010  | 01     |
| 0100  | 10     |
| 1000  | 11     |
| 1111  | 11     |

### Circuit Diagram:
Use OR gates to combine inputs with priority logic.

### Mathematical Expression:
\[
Y_0 = A + B, \quad Y_1 = C + D
\]

## 26. 8:3 Priority Encoder Design

### Block Diagram:
An **8:3 Priority Encoder** has 8 input lines and 3 output lines, with priority given to the highest active input.

### Truth Table:

| Input | Output |
|-------|--------|
| 00000001 | 000 |
| 00000010 | 001 |
| 00000100 | 010 |
| 00001000 | 011 |
| 00010000 | 100 |
| 00100000 | 101 |
| 01000000 | 110 |
| 10000000 | 111 |

### Circuit Diagram:
The circuit uses priority logic to select the highest input and generate the corresponding binary output.

### Mathematical Expression:
\[
Y_0 = A + B + C, \quad Y_1 = D + E + F, \quad Y_2 = G + H
\]

## 27. Multiplexor Definition and Design (4:1 Multiplexor)

### Definition:
A **Multiplexor (MUX)** is a combinational circuit that selects one of many inputs and forwards it to a single output line based on a set of control signals.

### Block Diagram:
A **4:1 Multiplexor** has 4 input lines, 1 output line, and 2 control (select) lines.

### Truth Table:

| Select Lines | Input | Output |
|---------------|-------|--------|
| S1 | S0 | I0 | I1 | I2 | I3 | Y |
|  0  |  0  |  X  |  0  |  0  |  0  | I0 |
|  0  |  1  |  0  |  X  |  0  |  0  | I1 |
|  1  |  0  |  0  |  0  |  X  |  0  | I2 |
|  1  |  1  |  0  |  0  |  0  |  X  | I3 |

### Circuit Diagram:
A 4:1 MUX can be constructed using 2:1 MUX blocks, with logic gates to control the selection.

### Mathematical Expression:
\[
Y = S_1'S_0'I_0 + S_1'S_0I_1 + S_1S_0'I_2 + S_1S_0I_3
\]

---

## 28. De-multiplexor Definition and Design (1:4 De-multiplexor)

### Definition:
A **De-multiplexor (DEMUX)** is a combinational circuit that takes a single input and channels it to one of many output lines based on the control signals.

### Block Diagram:
A **1:4 De-multiplexor** has 1 input line, 4 output lines, and 2 control (select) lines.

### Truth Table:

| Select Lines | Input | Output |
|---------------|-------|--------|
| S1 | S0 | I | O0 | O1 | O2 | O3 |
|  0  |  0  |  X  |  X  |  0  |  0  |  0  |
|  0  |  1  |  X  |  0  |  X  |  0  |  0  |
|  1  |  0  |  X  |  0  |  0  |  X  |  0  |
|  1  |  1  |  X  |  0  |  0  |  0  |  X  |

### Circuit Diagram:
The DEMUX uses AND gates to direct the input signal to the appropriate output line based on the control signals.

### Mathematical Expression:
\[
O_0 = S_1'S_0'I, \quad O_1 = S_1'S_0I, \quad O_2 = S_1S_0'I, \quad O_3 = S_1S_0I
\]

---

## 29. Design 4:1 MUX Using 2:1 MUX

### Design Steps:
To design a **4:1 MUX** using **2:1 MUX**:
- Use two 2:1 MUX for the first level of selection.
- Then, use another 2:1 MUX to combine the outputs from the first level.

### Block Diagram:

      +-----+



### Mathematical Expression:
\[
Y = S_1'S_0'I_0 + S_1'S_0I_1 + S_1S_0'I_2 + S_1S_0I_3
\]

---

## 30. Design 8:1 MUX Using 4:1 MUX and OR Gate

### Design Steps:
To design an **8:1 MUX** using **4:1 MUX** and an OR gate:
- Use two 4:1 MUX blocks to handle the first level of inputs.
- Use a 2:1 MUX for the final selection.
- Combine the outputs of the 4:1 MUX blocks with an OR gate.

### Block Diagram:
  +-----+       +-----+



### Mathematical Expression:
\[
Y = (S_2'S_1'S_0I_0 + S_2'S_1S_0I_1 + S_2S_1'S_0I_2 + S_2S_1S_0I_3) \, \text{OR} \, (S_2'S_1'S_0I_4 + S_2'S_1S_0I_5 + S_2S_1'S_0I_6 + S_2S_1S_0I_7)
\]

---

## 31. Design 4:16 Line Decoder Using Five 2:4 Line Decoders with Enable

### Design Steps:
To design a **4:16 Line Decoder** using **five 2:4 line decoders** with enable:
- Use four 2:4 line decoders to generate the first 16 outputs.
- Use an additional 2:4 line decoder to control the enabling of the outputs based on the input lines.

### Block Diagram:
      +-----+



### Truth Table:
The output will be enabled for the corresponding line based on the input combination, with control signals determining which 2:4 decoder is active.

### Mathematical Expression:
\[
Y_0 = S_3'S_2'S_1'S_0, \quad Y_1 = S_3'S_2'S_1S_0, \dots, Y_{15} = S_3S_2S_1S_0
\]




