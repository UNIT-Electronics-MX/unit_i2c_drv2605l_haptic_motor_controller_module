# Hardware

<div align="center">
<a href="unit_sch_v_1_0_ue0065_DRV2605.pdf">
    <img src="resources/Schematics_icon.jpg" width="500px"><br/>Schematics
</a>
</div>


## Technical Specifications

- **Interface:** I2C
- **I2C Address:**  0x5A 
- **Input Voltage:** 3.3V-5V
- **Compatible With:** LRA (Linear Resonance Actuator) and ERM (Eccentric Rotating Mass)

## Recommended Operating Conditions

<div align=center>

| Symbol/Rail | Description                                          | Min  | Typ  | Max  | Unit |
|-------------|------------------------------------------------------|------|------|------|------|
|   V_IN      | Input Voltage                                        | 3    | -    | 5.25 | V    |
|   f_PWM     | PWM input frequency (INT Pin)                        | 10   | -    | 250  | kHz  |
|   Z_L       | Load Impedance (V_IN)                                | 8    | -    | -    | Ω    |
|   V_IL      | Digital low-level input voltage (EN, INT, SDA, SCL)  | -    | -    | 0.5  | V    |
|   V_IH      | Digital high-level input voltage (EN, INT, SDA, SCL) | 1.3  | -    | -    | V    |
|   f_LRA     | LRA Optimal Frequency Range                          | 125  | -    | 300  | Hz   |
|   I_IL      | Digital low-level input current (EN, INT, SDA, SCL)  | -    | -    | 1    | uA   |
|   I_IH      | Digital high-level input Current (EN, INT, SDA, SCL) | 1    | 3.0  | 3.5  | uA   |
|   f_o(PWM)  | PWM Output Frequency                                 | 19.5 | 20.5 | 21.5 | kHz  |

</div>

* For QWIIC compatibility the board <b>must</b> be powered at 3.3V. 

## Pinout

<div align="center">
<a href="./resources/unit_pinout_v_1_0_ue0065_DRV2605.jpg"> <img src="./resources/unit_pinout_v_1_0_ue0065_DRV2605.jpg" width="500x"><br/>Pinout</a>
</div>

### **Pinout Details**

<div align=center>

| Pin Label | Function         | Notes                             |
|-----------|------------------|-----------------------------------|
| +3V3      | Power Supply     | 3.3V Power Supply                 |
| GND       | Ground           | Common ground reference           |
| SCL       | I2C SCL          | Serial Clock Line                 |
| SDA       | I2C SDA          | Serial Data Line                  |
| INT       | Power Supply     | GPIO                              |
| OUT-      | Motor -          | Motor negative output             |
| OUT+      | Motor +          | Motor positive output             |


</div>

## Board Topology

<div align="center">
<a href="./resources/unit_topology_v_1_0_ue0065_DRV2605.png"><img src="./resources/unit_topology_v_1_0_ue0065_DRV2605.png" width="500px"><br/>Topology</a>


| Ref.  | Description                                                                 |
|-------|-----------------------------------------------------------------------------|
| IC1   | DRV2605 Haptic Motor Driver                                                 |
| L1    | Power On LED                                                                |
| J1    | 1mm JST Connector compatible with QWIIC and STEMMA QT Connector             |
| J2    | 1mm JST Connector compatible with QWIIC and STEMMA QT Connector Jack        |
| J3    | Output for haptic motor                                                     |
| JP1   | Header for Input Signals                                                    |

</div>

## Board Dimensions

<div align="center">
<a href="./resources/unit_dimension_v_1_0_ue0065_DRV2605.png"><img src="./resources/unit_dimension_v_1_0_ue0065_DRV2605.png" width="500px"><br/>Dimensions</a>
</div>
