
# Unit-2: Number Systems

## 1. Define number system. Explain the types of number system.

### Number System:
A number system is a method for representing numbers using digits or symbols in a consistent manner. It is essential for expressing quantities and performing arithmetic operations.

### Types of Number Systems:
- **Decimal (Base 10):** Uses digits 0-9.  
  Example: 456
- **Binary (Base 2):** Uses digits 0 and 1.  
  Example: 1011
- **Octal (Base 8):** Uses digits 0-7.  
  Example: 345
- **Hexadecimal (Base 16):** Uses digits 0-9 and letters A-F.  
  Example: 2F3

---

## 2. Convert the following numbers into binary number system:

- **(a) (8956.345)₁₀**  
  Integer: 8956₁₀ → 10001111001100₂  
  Fraction: 0.345₁₀ → 0.010110₂  
  **Result:** (10001111001100.010110)₂

- **(b) (456.237)₈**  
  Integer: 456₈ → 100101110₂  
  Fraction: 0.237₈ → 0.010011₂  
  **Result:** (100101110.010011)₂

- **(c) (BCA.50D)₁₆**  
  Integer: BCA₁₆ → 101111001010₂  
  Fraction: 0.50D₁₆ → 0.010100₂  
  **Result:** (101111001010.010100)₂

---

## 3. Convert the following numbers into octal number system:

- **(a) (10101011.001010)₂**  
  Integer: 10101011₂ → 253₈  
  Fraction: 0.001010₂ → 0.12₈  
  **Result:** (253.12)₈

- **(b) (8965.748)₁₀**  
  Integer: 8965₁₀ → 21145₈  
  Fraction: 0.748₁₀ → 0.57₈  
  **Result:** (21145.57)₈

- **(c) (2B5.CA)₁₆**  
  Integer: 2B5₁₆ → 5455₈  
  Fraction: 0.CA₁₆ → 0.62₈  
  **Result:** (5455.62)₈

---

## 4. Convert the following numbers into decimal number system:

- **(a) (1000101.0010101)₂**  
  Integer: 1000101₂ → 69₁₀  
  Fraction: 0.0010101₂ → 0.1640625₁₀  
  **Result:** (69.1640625)₁₀

- **(b) (4567.41)₈**  
  Integer: 4567₈ → 2399₁₀  
  Fraction: 0.41₈ → 0.53125₁₀  
  **Result:** (2399.53125)₁₀

- **(c) (D015.BE0)₁₆**  
  Integer: D015₁₆ → 53269₁₀  
  Fraction: 0.BE0₁₆ → 0.7421875₁₀  
  **Result:** (53269.7421875)₁₀

---

## 5. Convert the following numbers into hexadecimal number system:

- **(a) (10101011110011101.11011010)₂**  
  Integer: 10101011110011101₂ → 15CD₁₆  
  Fraction: 0.11011010₂ → 0.DA₁₆  
  **Result:** (15CD.DA)₁₆

- **(b) (7654.32)₈**  
  Integer: 7654₈ → 1F2C₁₆  
  Fraction: 0.32₈ → 0.69₁₆  
  **Result:** (1F2C.69)₁₆

- **(c) (9876.548)₁₀**  
  Integer: 9876₁₀ → 2694₁₆  
  Fraction: 0.548₁₀ → 0.8C₁₆  
  **Result:** (2694.8C)₁₆

---

## 6. Subtract using 1’s and 2’s complement method:

- **(a) (10110)₂ – (110010)₂**  
  Step 1: 1’s Complement of 110010: 001101  
  Step 2: Add 10110 + 001101 = 111011 (discard carry)  
  **Result:** –11101₂

- **(b) (110110)₂ – (100010)₂**  
  Step 1: 1’s Complement of 100010: 011101  
  Step 2: Add 110110 + 011101 = 1011011 (discard carry)  
  **Result:** 001011₂

---

## 7. Perform BCD Addition:

- **(a) 10000110 + 00010011**  
  **Result:** 10011001

- **(b) 010001010000 + 010000010111**  
  **Result:** 100001100111

- **(c) 456.23 + 128.78**  
  **Result:** 585.01 (in BCD)

---

## 8. Convert binary number into Grey code:

- **(a) 101101**  
  **Binary to Grey:** 111111

- **(b) 110101**  
  **Binary to Grey:** 101111

---

## 9. Convert Grey code into binary code:

- **(a) 11000110**  
  **Grey to Binary:** 10110101

- **(b) 10101111**  
  **Grey to Binary:** 11011100

---

## 10. Convert –176.375 into 32-bit floating point representation:

- Binary: –176.375₁₀ → ‑1010110.011₂  
- Normalize: ‑1.1010110011 x 2⁷  
- Sign: 1, Exponent: 127+7=134 (10000110), Mantissa: 10101100110000000000000  
- **Result:** 11100001101010110000000000000000

---

## 11. Convert 85.125 into IEEE 754 single and double precision representation:

- Binary: 85.125₁₀ → 1010101.001₂  
- Normalize: 1.010101001 x 2⁶

### Single Precision:
- Sign: 0, Exponent: 127+6=133 (10000101), Mantissa: 01010100100000000000000  
- **Result:** 01000010101010100100000000000000

### Double Precision:
- Exponent: 1023+6=1029 (10000000101), Mantissa: 0101010010000000000000000000000000000000000000000000  
- **Result:** 010000000101010101001000000000000000000000000000000000000000000000000000

---

## 12. What are error detecting & correcting codes? Explain with examples.

- **Error Detecting Codes:**  
  These codes identify errors during data transmission.  
  Example: **Parity bit.**

- **Error Correcting Codes:**  
  These codes detect and correct errors during transmission.  
  Example: **Hamming Code.**

### Hamming Code Example:
For 4-bit data "1010", add parity bits: 1010100.  
Use a parity check matrix to detect errors and correct single-bit errors during transmission.
