# Digital Logic ASIC Design

## How it works

This project implements four fundamental combinational logic gates: AND, OR, XOR, and NAND. Each gate operates independently using two binary inputs and produces one binary output.

The circuit uses all eight input pins and four output pins.

| Logic Gate | Inputs | Output | Operation |
|---|---|---|---|
| AND | IN0, IN1 | OUT0 | HIGH when both inputs are HIGH |
| OR | IN2, IN3 | OUT1 | HIGH when at least one input is HIGH |
| XOR | IN4, IN5 | OUT2 | HIGH when the inputs are different |
| NAND | IN6, IN7 | OUT3 | LOW only when both inputs are HIGH |

The circuit is purely combinational and does not require a clock signal or internal memory.

## How to test

1. Connect the eight input pins to digital switches.
2. Connect the four output pins to LEDs or a logic analyzer.
3. Apply different binary combinations (0 or 1) to each pair of inputs.
4. Observe the corresponding outputs.
5. Compare the results with the expected truth table.

### Expected Truth Table

| Input A | Input B | AND | OR | XOR | NAND |
|---|---|---|---|---|---|
| 0 | 0 | 0 | 0 | 0 | 1 |
| 0 | 1 | 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 1 | 1 | 1 |
| 1 | 1 | 1 | 1 | 0 | 0 |

Each gate should be tested independently using its corresponding input pins.

The design can also be tested in Wokwi using the input switches and the seven-segment display connected to the outputs.

## External hardware

No additional external hardware is required for the internal logic functionality.

For testing and visualization, the following components can be used:

- Eight digital input switches
- A seven-segment LED display or individual LEDs
- A compatible Tiny Tapeout test
