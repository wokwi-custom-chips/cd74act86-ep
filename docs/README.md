# Wokwi cd74act86-ep Chip

This is a custom chip for [Wokwi](https://wokwi.com/). It implements the cd74act86-ep IC.

## Description

The cd74act86-ep contain four independent 2-input Exclusive-OR gates. Each gate performs the Boolean function
of Y = (A ⊕ B) in positive logic.

## Truth Table (1 for each gate)

| INPUT A | INPUT B |  OUTPUT |
|---------|---------|---------|
|    L    |    L    |    L    |
|    H    |    L    |    H    |
|    L    |    H    |    H    |
|    H    |    H    |    L    |

## Pin names

| Name | Description             |
| ---- | ----------------------- |
|  1A  | Gate 1 Input signal  A  |
|  1B  | Gate 1 Input signal  B  |
|  1Y  | Gate 1 Output signal    |
|  2A  | Gate 2 Input signal  A  |
|  2B  | Gate 2 Input signal  B  |
|  2Y  | Gate 2 Output signal    |
|  3A  | Gate 3 Input signal  A  |
|  3B  | Gate 3 Input signal  B  |
|  3Y  | Gate 3 Output signal    |
|  4A  | Gate 4 Input signal  A  |
|  4B  | Gate 4 Input signal  B  |
|  4Y  | Gate 4 Output signal    |
| GND  | Ground                  |
| VCC  | Supply voltage          |


## Usage

To use this chip in your project, include it as a dependency in your `diagram.json` file:

```json
  "dependencies": {
    "chip-cd74act86-ep": "github:wokwi-custom-chips/cd74act86-ep@0.1.0"
  }
```

Then, add the chip to your circuit by adding a `chip-cd74act86-ep` item to the `parts` section of diagram.json:

```json
  "parts": {
    ...,
    { "type": "chip-cd74act86-ep", "id": "chip1" }
  },
```

For a complete example, see [The cd74act86-ep chip test project](https://wokwi.com/projects/398973311191185409).
