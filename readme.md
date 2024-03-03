# Variable Lighting System for FPGA Boards

## Project Description

This project aims to design a variable lighting system using LEDs on FPGA boards, employing the Pulse Width Modulation (PWM) technique to vary the light intensity. The system features several modes of operation, catering to different requirements and scenarios:

### Modes of Operation

1. **Manual Mode**: In this mode, the luminous intensity of the LEDs is directly controlled through switches on the FPGA board. The intensity value is supplied in an 8-bit format, allowing for precise manual control over each LED's brightness.

2. **Test Mode**: Designed for testing each LED's functionality, this mode automatically cycles the light intensity of the LEDs from their minimum to maximum values in a specific time interval unique to each LED. The intervals increase progressively from 1 second for led0 to 8 seconds for led7, creating an approximate saw wave pattern for the intensity variation.

3. **Automatic Mode**: In this mode, the luminous intensity of the LEDs automatically cycles from the minimum to the maximum value and then back to the minimum. This cycle creates an approximate triangle waveform, with the cycle's duration (measured in seconds) provided as an input to the system. This mode is useful for demonstrations or when a dynamic light display is required without manual adjustment.

### Display and Control

- The current operating mode, the light intensity of the LEDs, and the period for the current waveform are displayed on the 7-segment displays of the FPGA board. This feature provides real-time feedback and makes it easier to monitor and adjust the system's settings.

### Documentation and References

- For detailed information on working with the FPGA board and implementing PWM for light intensity variation, refer to the FPGA board reference manual available at [Digilent's official website](www.digilentinc.com).

### Implementation Notes

- The implementation relies on the PWM technique to adjust the LEDs' luminous intensity. This approach allows for fine-tuned control over the lighting, making the system versatile for various applications, from visual alerts to ambient lighting effects.

- The choice of modes and the use of a manual input system ensure that the lighting system can be adapted to a wide range of scenarios, providing both functionality and educational value in understanding PWM and FPGA board capabilities.

This project provides a comprehensive platform for exploring variable lighting systems, PWM techniques, and FPGA board functionalities.