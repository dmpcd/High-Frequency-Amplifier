# High Frequency Amplifier Project

## Introduction

This project involves the design and development of a high-frequency amplifier capable of driving an 8-ohm speaker without distortion. The amplifier operates within a frequency range of 20kHz to 100kHz and is composed of a two-stage design: a common emitter pre-amplifier for voltage amplification and a class AB power amplifier with voltage buffers for power amplification.

## Features

- **Frequency Range**: 20kHz to 100kHz
- **Load**: Drives an 8-ohm speaker without significant distortion
- **Stages**: Two-stage amplifier design
  - **Pre-Amplifier**: Common emitter configuration for voltage amplification
  - **Power Amplifier**: Class AB with voltage buffers for power amplification
- **Gain**: Open terminal voltage gain of 28.5 (theoretical), with a practical gain of 18.1 when driving a speaker
- **Efficiency**: Designed to minimize power dissipation while ensuring high performance

## Design Approach

The design of the amplifier involved several steps:

1. **Class A Amplifier Stage**: Provides full amplification of the input signal with a simple structure but is inefficient due to constant current flow.
2. **Class B Amplifier Stage**: Conducts only half of the input signal and uses a push-pull arrangement to combine outputs, reducing power loss but introducing zero crossing distortion.
3. **Class AB Amplifier Stage**: Combines the benefits of Class A and Class B stages to minimize distortion while maintaining efficiency.
4. **Voltage Buffer Stage**: Incorporates voltage buffers using the common collector configuration to isolate transistors and achieve high gain.

## Prototype Design

### Simulation

The amplifier circuit was initially simulated using Proteus software to validate the design and performance.

### Physical Prototype

A physical prototype was built and tested using the following steps:
- **Breadboard Implementation**: Initial testing and verification of circuit functionality
- **PCB Design**: The circuit was designed using Altium software, with components soldered onto the PCB after screen printing
- **Enclosure**: Designed using SolidWorks with a perforated cover for heat dissipation, made from PLA+ material for eco-friendliness

### Components and Equipment

#### Components

- 2N2222A NPN BJT transistor
- TIP 31C power transistors (2)
- TIP 32C power transistors (2)
- Capacitors: 1µF, 10µF, 100µF, 1000µF, 220µF
- Resistors: 1.2kΩ, 10kΩ, 2.2kΩ, 270Ω, 56Ω, 2.2kΩ
- Power resistors: 68Ω, 2.2Ω

#### Equipment

- Power Supply
- Digital multimeter
- Signal generator
- Digital Oscilloscope
- Breadboard
- 8Ω speaker

## Results

The amplifier was tested for various parameters, and the following results were obtained:

- **Open Circuit Gain**: 21
- **Gain with 8Ω Load**: 16.393
- **Bandwidth**: 700kHz
- **Input Resistance**: 2.188 kΩ
- **Output Resistance**: 8.0108 Ω
- **Power Dissipation**: 2.4 W

## Individual Contributions

- **Maduwantha L.H.H**: PCB design, Component selection
- **Dimagi D.H.P.**: Enclosure design, Breadboard implementation
- **Dissanayaka D.M.P.C.**: Enclosure design, Soldering PCB, Breadboard implementation
- **Dilshan N.L.**: Circuit design, Simulation in Proteus

## Conclusion

The project was successfully completed within the given timeframe. Despite some minor issues with the bandwidth and waveform distortion, the amplifier meets most of the design requirements and performs effectively for the intended application.

## Setup and Usage

### Prerequisites

- Basic knowledge of electronic components and circuits
- Tools for soldering and assembling the PCB
- Access to simulation software (Proteus) and design software (Altium, SolidWorks)

### Steps to Reproduce

1. **Clone the Repository**: 
    ```sh
    git clone https://github.com/dmpcd/high-frequency-amplifier.git
    cd high-frequency-amplifier
    ```

2. **Simulation**: 
   - Open the simulation files in Proteus and run the simulations to observe the amplifier's performance.

3. **PCB Design**: 
   - Use Altium to open the PCB design files and review the layout. Fabricate and assemble the PCB.

4. **Testing**: 
   - Use the listed components and equipment to build the physical prototype and verify the results as described.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## References

- [Amplifier Classes](https://www.electronics-tutorials.ws/amplifier/amplifier-classes.html)
- [2N2222A NPN Transistor Datasheet](https://pdf1.alldatasheet.com/datasheet-pdf/download/956542/FCI/2N2222A.html)
- [TIP31C Datasheet](https://www.st.com/resource/en/datasheet/tip31c.pdf)
- [TIP32C Datasheet](https://www.st.com/resource/en/datasheet/tip32c.pdf)
