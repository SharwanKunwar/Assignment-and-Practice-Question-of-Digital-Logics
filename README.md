# Unit-4: Counter and Registers

## 1. Distinguish between sequential and combinational logic with example

### Sequential Logic:
- In sequential logic, the output depends not only on the current inputs but also on the previous states (history).
- These circuits have memory elements, like flip-flops or latches, which store the previous states.
  
**Example:**  
A **D flip-flop** is a sequential logic element where the output depends on both the input and the clock signal.

### Combinational Logic:
- In combinational logic, the output depends solely on the current inputs, with no memory or dependence on previous states.
- These circuits perform operations like AND, OR, NOT, etc., to produce an output.

**Example:**  
A **2-input AND gate** is a combinational logic element where the output depends only on the current inputs.

---

## 2. Differentiate between latch and flip-flop

### Latch:
- A latch is a level-sensitive device that stores data when the enable signal is active.
- Latches can change states whenever the clock or control signal is active, leading to potential glitches.

### Flip-Flop:
- A flip-flop is an edge-triggered device that stores data only on the rising or falling edge of the clock signal.
- Flip-flops provide more stability and are less prone to glitches compared to latches.

---

## 3. What is clocked RS flip-flop? Explain with its logic diagram, truth table, and timing diagram. What are the drawbacks of clocked RS flip-flop?

### Clocked RS Flip-Flop:
A clocked RS flip-flop is a type of sequential circuit that uses a clock signal to control the setting and resetting of its outputs. The inputs are **Set (S)** and **Reset (R)**, and the output is **Q**.

### Logic Diagram:
  _______

### Truth Table:
| **S** | **R** | **Q** | **Q'** |
|:-----:|:-----:|:-----:|:------:|
|   0   |   0   |   Q   |   Q'   |
|   0   |   1   |   0   |   1    |
|   1   |   0   |   1   |   0    |
|   1   |   1   |   Invalid | Invalid |

### Timing Diagram:

### Drawbacks of Clocked RS Flip-Flop:
1. The **S = 1** and **R = 1** condition is invalid, leading to unpredictable outputs.
2. It may lead to a race condition in certain designs.

---

## 4. What is D flip-flop? Explain with its logic diagram, truth table, and timing diagram.

### D Flip-Flop:
A D flip-flop is a type of sequential logic circuit that captures the value of the input **D** at the edge of the clock signal and holds it until the next clock edge.

### Logic Diagram:
  _______

### Truth Table:
| **CLK** | **D** | **Q** | **Q'** |
|:------:|:-----:|:-----:|:------:|
|   ↑    |   0   |   0   |   1    |
|   ↑    |   1   |   1   |   0    |

### Timing Diagram:

---

## 5. Define sequential circuit. Draw a logic diagram, graphic symbol, characteristic table, and characteristic equation of clocked JK flip-flop.

### Sequential Circuit:
A sequential circuit is a type of circuit where the output depends on both the current input and the previous states. These circuits have memory elements, and the state of the system is updated at each clock cycle.

### Clocked JK Flip-Flop:
A JK flip-flop is a type of flip-flop that has two inputs, **J** and **K**, and it can toggle its state based on these inputs.

### Logic Diagram:

### Graphic Symbol:
   _______

### Characteristic Table:
| **J** | **K** | **Q** | **Q'** |
|:-----:|:-----:|:-----:|:------:|
|   0   |   0   |   Q   |   Q'   |
|   0   |   1   |   0   |   1    |
|   1   |   0   |   1   |   0    |
|   1   |   1   |   T   |   T    |

### Characteristic Equation:
The characteristic equation for a JK flip-flop is:
Where:
- **Q(t+1)** is the next state of the flip-flop.
- **J** and **K** are the inputs.
- **Q** is the current state of the flip-flop.
- **Q'** is the complement of Q.

### Truth Table:
| **T** | **Q(t)** | **Q(t+1)** |
|:-----:|:--------:|:----------:|
|   0   |    0     |     0      |
|   0   |    1     |     1      |
|   1   |    0     |     1      |
|   1   |    1     |     0      |

### Timing Diagram:

---

## 7. Design a Master-slave flip-flop by using JK flip-flop along with its circuit diagram and truth table.

### Master-Slave JK Flip-Flop:
A master-slave flip-flop is created by connecting two JK flip-flops in series. The master flip-flop is triggered on the clock’s leading edge, and the slave flip-flop is triggered on the trailing edge. This arrangement ensures that the output of the slave flip-flop is stable and does not change during the clock pulse.

### Circuit Diagram:

### Truth Table:
| **J** | **K** | **Q (Master)** | **Q (Slave)** |
|:-----:|:-----:|:--------------:|:-------------:|
|   0   |   0   |       Q        |       Q       |
|   0   |   1   |       0        |       0       |
|   1   |   0   |       1        |       1       |
|   1   |   1   |    Toggle      |    Toggle     |

---

## 8. Discuss race condition in JK flip-flop and methods to overcome it.

### Race Condition in JK Flip-Flop:
A race condition occurs in a JK flip-flop when both **J** and **K** inputs are high at the same time. This causes the output to toggle rapidly, leading to unpredictable behavior.

### Methods to Overcome Race Condition:
1. **Master-Slave Flip-Flop**: Using a master-slave configuration, where the flip-flop changes state only on the trailing edge of the clock signal, helps avoid the race condition.
2. **Edge-Triggered Flip-Flop**: Use of edge-triggered flip-flops (like D flip-flops) can also eliminate race conditions by changing state only on a clock edge.

---

## 9. Write down the difference between asynchronous and synchronous counter.

### Asynchronous Counter:
- In an asynchronous counter, the flip-flops are not all triggered simultaneously. The clock input of each flip-flop is connected to the output of the previous flip-flop.
- The flip-flops change states at different times, which can lead to propagation delay.

### Synchronous Counter:
- In a synchronous counter, all flip-flops are triggered by the same clock signal. The state of all flip-flops changes simultaneously.
- Synchronous counters are faster and more reliable as they avoid the propagation delay of asynchronous counters.

---

## 10. Design a 3-bit asynchronous binary UP counter.

### 3-Bit Asynchronous Binary UP Counter:
- A 3-bit counter has 3 flip-flops (typically T flip-flops) connected in series.
- The output of each flip-flop represents a bit of the binary count.

### Circuit Diagram:

### Operation:
- The first flip-flop toggles with every clock pulse, and each subsequent flip-flop toggles when the previous flip-flop transitions from 1 to 0.

---

## 11. Design a 4-bit synchronous binary DOWN counter

### 4-Bit Synchronous Binary DOWN Counter:
- A 4-bit down counter counts down from 15 to 0 in binary.
- All flip-flops are connected to the same clock signal, and the counting sequence is controlled by the logic inputs of the flip-flops.

### Circuit Diagram:


## 6. What is T flip-flop? Explain with its logic diagram, truth table, and timing diagram.

### T Flip-Flop:
A T flip-flop is a type of flip-flop that toggles its output on each clock pulse when the input **T** is high. When **T** is low, the output remains unchanged.

### Logic Diagram:


### Operation:
- The flip-flops change states simultaneously, and the logic inputs determine whether the counter counts down or up.

---

## 12. Design a 3-bit asynchronous UP/DOWN counter.

### 3-Bit Asynchronous UP/DOWN Counter:
- A 3-bit counter that can count both upwards and downwards based on a control input (Up/Down).
- When the control input is high, the counter counts up; when low, it counts down.

### Circuit Diagram:

### Operation:
- The counter’s direction is controlled by the Up/Down input. The flip-flops toggle in sequence based on the control input.

---

## 13. Explain the Ring counter with Circuit, State, and Timing Diagram.

### Ring Counter:
A ring counter is a type of shift register where the output of the last flip-flop is connected to the input of the first flip-flop. It generates a sequence of states where only one flip-flop is high at any time.

### Circuit Diagram:

### State Diagram:
| State | Q1 | Q2 | Q3 | Q4 |
|:-----:|:--:|:--:|:--:|:--:|
|   1   |  1 |  0 |  0 |  0 |
|   2   |  0 |  1 |  0 |  0 |
|   3   |  0 |  0 |  1 |  0 |
|   4   |  0 |  0 |  0 |  1 |

### Timing Diagram:

---

## 14. Define register. Explain different types of registers with block diagram.

### Register:
A register is a storage device used to store binary data temporarily. Registers are commonly used in digital circuits to hold intermediate data during computation.

### Types of Registers:
1. **Shift Register**: A register where data can be shifted left or right.
2. **Serial-In-Parallel-Out (SIPO) Register**: Data is input serially and output in parallel.
3. **Parallel-In-Parallel-Out (PIPO) Register**: Data is input and output in parallel.

---

## 15. Define register. Explain the working principle of Serial In Serial Out (SISO) register.

### Serial-In-Serial-Out (SISO) Register:
A SISO register is a type of shift register where data is input serially and output serially. Each bit of data is shifted through the register with each clock pulse.

### Working Principle:
- Data enters the register one bit at a time and shifts through each flip-flop on each clock pulse.
- The last bit in the register is shifted out serially.

### Block Diagram:

---

## 16. Design a 4-bit Serial-In Parallel-Out Shift Register with Timing Diagram

### 4-Bit Serial-In Parallel-Out (SIPO) Shift Register:
A **Serial-In Parallel-Out (SIPO)** shift register allows data to be entered serially (one bit at a time) and output in parallel (all bits at once). Each clock pulse shifts the data into the next flip-flop in the register, and after four clock pulses, all four bits of data are stored and available as parallel output.

### Circuit Diagram:
The circuit consists of four flip-flops connected in series, with the output of each flip-flop connected to the input of the next flip-flop. The serial input is provided to the first flip-flop, and the parallel outputs are taken from each flip-flop.


- **FF1, FF2, FF3, FF4** are the flip-flops (typically D or JK flip-flops).
- **Serial Input**: The bit-by-bit data is shifted in.
- **Parallel Output**: The stored data is available as Q1, Q2, Q3, and Q4 (parallel output).

### Operation:
1. On each clock pulse, a bit is shifted into the first flip-flop (FF1).
2. The bits then propagate through the shift register, one bit at a time, with each clock pulse.
3. After 4 clock pulses, all 4 bits are stored, and the data is available at the parallel outputs (Q1 to Q4).

### Timing Diagram:

| Clock Pulse | Serial Input (S) | Q1 | Q2 | Q3 | Q4 |
|-------------|------------------|----|----|----|----|
| 0           | 0                | 0  | 0  | 0  | 0  |
| 1           | 1                | 1  | 0  | 0  | 0  |
| 2           | 0                | 1  | 1  | 0  | 0  |
| 3           | 1                | 1  | 0  | 1  | 0  |
| 4           | 0                | 1  | 1  | 0  | 1  |

- **Clock Pulse 0**: Initially, all flip-flops are reset to 0.
- **Clock Pulse 1**: The first bit "1" is shifted into FF1, and the output of FF1 becomes "1."
- **Clock Pulse 2**: The second bit "0" is shifted into FF1, and the output of FF2 becomes "1."
- **Clock Pulse 3**: The third bit "1" is shifted into FF1, and the output of FF3 becomes "1."
- **Clock Pulse 4**: The fourth bit "0" is shifted into FF1, and the output of FF4 becomes "1."

After 4 clock pulses, the register holds the bits "1010" at the parallel outputs.

### Summary:
- The **SIPO shift register** allows data to be input serially and output in parallel.
- The data is shifted through the register on each clock pulse, and after 4 clock pulses, the data is available as parallel output.
- The timing diagram shows the shift of bits into the register and the final parallel output after 4 clock cycles.

