**Hexadecimal to 7-Segment Display Converter**
This project implements a converter that takes a **hexadecimal digit (0–F)** as input and outputs the corresponding **7-segment display pattern**.

**What It Does**
- Takes a 4-bit binary/hexadecimal input (0x0 to 0xF)
- Outputs a 7-bit signal to drive a common-cathode 7-segment display
- Displays numbers 0–9 and letters A–F on the display

**How a 7-Segment Display Works**

A 7-segment display consists of 7 LEDs labeled as follows:(a-g)
Each segment (a–g) is controlled by one output bit. A binary **`1`** lights up the segment (for active high displays).

**Inputs and Outputs**

**Inputs**

- Hexadecimal digit (4-bit input): `0000` to `1111` (i.e., 0 to F)

**Outputs**

- 7-bit output: `{a, b, c, d, e, f, g}` pattern for the display

Example Mappings

| Hex | Segments (abcdefg) | Display |
|-----|--------------------|---------|
| 0   | 1111110            | `0`     |
| 1   | 0110000            | `1`     |
| 2   | 1101101            | `2`     |
| 3   | 1111001            | `3`     |
| 4   | 0110011            | `4`     |
| 5   | 1011011            | `5`     |
| 6   | 1011111            | `6`     |
| 7   | 1110000            | `7`     |
| 8   | 1111111            | `8`     |
| 9   | 1111011            | `9`     |
| A   | 1110111            | `A`     |
| B   | 0011111            | `b`     |
| C   | 1001110            | `C`     |
| D   | 0111101            | `d`     |
| E   | 1001111            | `E`     |
| F   | 1000111            | `F`     |



 Technologies Used

- Can be implemented in:
  - Verilog / VHDL (FPGA/ASIC)
  - FPGA kit
