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
