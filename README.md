# Voltage Regulator Modules

A collection of four compact open-source voltage regulator PCB modules designed in EasyEDA .

This repository contains fixed-output 5V and 3.3V regulator boards made for embedded electronics, robotics, IoT jects, totyping, and small custom PCB designs.

Each board includes its schematic, PCB layout, BOM, and ject files. The Gerber files and EasyEDA ject files are available on each OSHWLab ject page.

## Included Boards

| Board         | Output Voltage | Max Output Current | Main Regulator | Type                   |
| ------------- | -------------: | -----------------: | -------------- | ---------------------- |
| 5V 1.5A    |             5V |               1.5A | L7805CV        | Linear regulator       |
| 5V 1A      |             5V |                 1A | AMS1117-5.0    | LDO / linear regulator |
| 3.3V 1A    |           3.3V |                 1A | AMS1117-3.3    | LDO / linear regulator |
| 3.3V 500mA |           3.3V |              500mA | RT9013-33GB-MS | LDO regulator          |

> Note: These boards are step-down regulator modules because they generate a lower fixed output voltage from a higher input voltage. The regulators used here are linear / LDO regulators, not switching buck converters.

## 5V 1.5A Step-Down Voltage Regulator

<img src="https://github.com/andreipopescufilimon/3.3V-5V-Voltage-Regulators/blob/0fc129d68f21643a803581ae65e8faeecc6290e5/5v-1.5a/5v-1.5a-pcb.png" width="400" />

The **5V 1.5A** module is a higher-current 5V regulator board based on the **L7805CV** linear regulator. It is designed for jects that need a stable 5V rail with more current than smaller LDO modules can vide.

This board can be used for microcontrollers, sensors, LED modules, small logic circuits, communication modules, and general 5V electronics.

You can find the Gerber files and EasyEDA ject files on the OSHWLab ject page:
[5V 1.5A on OSHWLab](https://oshwlab.com/bicicleta11/5v-1.5a-step-down-voltage-regula)

### Features

* Fixed 5V output
* Up to 1.5A output current
* Based on the L7805CV regulator
* Simple 3-pin input / output module
* Suitable for embedded systems, robotics, and totyping
* Through-hole header for easy connection

### Main Components

| Designator | Component    | Part Number | Package      |
| ---------- | ------------ | ----------- | ------------ |
| U1         | 5V regulator | L7805CV     | TO-220-3     |
| C1, C2     | Capacitors   | 10uF        | 0805         |
| H1         | 3-pin header | 2.54mm      | Through-hole |

### BOM

| ID | Name            | Designator | Footprint                   | Quantity | Manufacturer Part | Supplier Part |
| -- | --------------- | ---------- | --------------------------- | -------: | ----------------- | ------------- |
| 1  | L7805CV         | U1         | TO-220-3_L10.0-W4.5-P2.54-L |        1 | L7805CV           | C6430948      |
| 2  | 10uF            | C1, C2     | C0805                       |        2 | CL21B106KPQNNNE   | C32635        |
| 3  | HDR-F_2.54_1x3P | H1         | HDR-TH_3P-P2.54-V-F         |        1 | -                 | -             |

## 5V 1A Step-Down Voltage Regulator

<img src="https://github.com/andreipopescufilimon/3.3V-5V-Voltage-Regulators/blob/0fc129d68f21643a803581ae65e8faeecc6290e5/5v-1a/5v-1a-pcb.png" width="400" />

The **5V 1A** module is a compact 5V regulator board based on the **AMS1117-5.0**. It is suitable for small embedded systems that need a reliable 5V output from a higher input voltage.

It can be used to power microcontrollers, sensor modules, small servos, logic circuits, LEDs, and other low-power 5V devices.

You can find the Gerber files and EasyEDA ject files on the OSHWLab ject page:
[5V 1A on OSHWLab](https://oshwlab.com/bicicleta11/5v-1a-step-down-voltage-reg)

### Features

* Fixed 5V output
* Up to 1A output current
* Based on the AMS1117-5.0 regulator
* Compact PCB size
* Simple input, output, and ground connection
* Good for DIY electronics, robotics, and embedded systems

### Main Components

| Designator | Component        | Part Number | Package      |
| ---------- | ---------------- | ----------- | ------------ |
| U1         | 5V LDO regulator | AMS1117-5.0 | SOT-223      |
| C1         | Capacitor        | 22uF        | 0805         |
| C2         | Capacitor        | 10uF        | 0805         |
| H1         | 3-pin header     | 2.54mm      | Through-hole |

### BOM

| ID | Name              | Designator | Footprint                            | Quantity | Manufacturer Part | Supplier Part |
| -- | ----------------- | ---------- | ------------------------------------ | -------: | ----------------- | ------------- |
| 1  | AMS1117-5.0(XBLW) | U1         | SOT-223-3_L6.5-W3.4-P2.30-LS7.0-BR-1 |        1 | AMS1117-5.0(XBLW) | C18723570     |
| 2  | 22uF              | C1         | C0805                                |        1 | CL21A226MAYNNNE   | C602037       |
| 3  | 10uF              | C2         | C0805                                |        1 | CL21B106KPQNNNE   | C32635        |
| 4  | HDR-F_2.54_1x3P   | H1         | HDR-TH_3P-P2.54-V-F                  |        1 | -                 | -             |

## 3.3V 1A Step-Down Voltage Regulator

<img src="https://github.com/andreipopescufilimon/3.3V-5V-Voltage-Regulators/blob/0fc129d68f21643a803581ae65e8faeecc6290e5/3.3v-1a/3.3v-1a-pcb.png" width="400" />

The **3.3V 1A** module vides a fixed 3.3V output using the **AMS1117-3.3** regulator. It is made for modern low-voltage electronics such as ESP32 boards, sensors, logic ICs, communication modules, and embedded systems.

This board is useful when a ject has a higher input voltage available but requires a stable 3.3V power rail.

You can find the Gerber files and EasyEDA ject files on the OSHWLab ject page:
[3.3V 1A on OSHWLab](https://oshwlab.com/bicicleta11/3.3v-1a-step-down-voltage-regula)

### Features

* Fixed 3.3V output
* Up to 1A output current
* Based on the AMS1117-3.3 regulator
* Suitable for ESP32, sensors, and 3.3V logic
* Compact and easy to integrate
* Designed for robotics, IoT, and custom PCB jects

### Main Components

| Designator | Component          | Part Number | Package      |
| ---------- | ------------------ | ----------- | ------------ |
| U1         | 3.3V LDO regulator | AMS1117-3.3 | SOT-223      |
| C1         | Capacitor          | 10uF        | 0805         |
| C2         | Capacitor          | 22uF        | 0805         |
| H1         | 3-pin header       | 2.54mm      | Through-hole |

### BOM

| ID | Name            | Designator | Footprint                          | Quantity | Manufacturer Part | Supplier Part |
| -- | --------------- | ---------- | ---------------------------------- | -------: | ----------------- | ------------- |
| 1  | 10uF            | C1         | C0805                              |        1 | CL21B106KPQNNNE   | C32635        |
| 2  | HDR-F_2.54_1x3P | H1         | HDR-TH_3P-P2.54-V-F                |        1 | -                 | -             |
| 3  | AMS1117-3.3     | U1         | SOT-223-4_L6.5-W3.5-P2.30-LS7.0-BR |        1 | AMS1117-3.3       | C347222       |
| 4  | 22uF            | C2         | C0805                              |        1 | CL21A226MAYNNNE   | C602037       |

## 3.3V 500mA Step-Down Voltage Regulator

<img src="https://github.com/andreipopescufilimon/3.3V-5V-Voltage-Regulators/blob/0fc129d68f21643a803581ae65e8faeecc6290e5/3.3v-500ma/3.3v-500ma-pcb.png" width="400" />

The **3.3V 500mA** module is a small 3.3V regulator board based on the **RT9013-33GB-MS** LDO regulator. It is intended for lower-power electronics where a compact and efficient 3.3V rail is needed.

It is a good choice for sensors, small microcontrollers, communication modules, logic circuits, IoT devices, and lightweight embedded systems.

You can find the Gerber files and EasyEDA ject files on the OSHWLab ject page:
[3.3V 500mA on OSHWLab](https://oshwlab.com/bicicleta11/3.3v-500ma-step-down-voltage-reg)

### Features

* Fixed 3.3V output
* Up to 500mA output current
* Based on the RT9013-33GB-MS LDO regulator
* Very compact design
* Suitable for sensors and small 3.3V modules
* Good for IoT, robotics, and low-power PCB jects

### Main Components

| Designator | Component          | Part Number    | Package      |
| ---------- | ------------------ | -------------- | ------------ |
| U1         | 3.3V LDO regulator | RT9013-33GB-MS | SOT-23-5     |
| C1, C2     | Capacitors         | 10uF           | 0805         |
| H1         | 3-pin header       | 2.54mm         | Through-hole |

### BOM

| ID | Name            | Designator | Footprint                         | Quantity | Manufacturer Part | Supplier Part |
| -- | --------------- | ---------- | --------------------------------- | -------: | ----------------- | ------------- |
| 1  | RT9013-33GB-MS  | U1         | SOT-23-5_L2.9-W1.6-P0.95-LS2.8-BR |        1 | RT9013-33GB-MS    | C7434207      |
| 2  | 10uF            | C1, C2     | C0805                             |        2 | CL21B106KPQNNNE   | C32635        |
| 3  | HDR-F_2.54_1x3P | H1         | HDR-TH_3P-P2.54-V-F               |        1 | -                 | -             |

## Pinout

Each board uses a simple 3-pin header.

| Pin  | Function                 |
| ---- | ------------------------ |
| VIN  | Input voltage            |
| GND  | Ground                   |
| VOUT | Regulated output voltage |

Always check the schematic and PCB silkscreen before powering the board.

## Usage

1. Connect the input voltage to `VIN`.
2. Connect ground to `GND`.
3. Connect your load to `VOUT`.
4. Make sure the input voltage is higher than the required output voltage.
5. Do not exceed the current rating of the selected regulator board.
6. Check the regulator temperature during testing, especially with higher input voltages or higher loads.

## Thermal Considerations

These modules use linear / LDO regulators, so the regulator must dissipate the voltage difference between input and output as heat.

Power dissipation can be estimated with:

```text
P = (VIN - VOUT) × IOUT
```

Example:

```text
VIN = 12V
VOUT = 5V
IOUT = 1A

P = (12V - 5V) × 1A
P = 7W
```

In this example, the regulator would need to dissipate 7W as heat, which is too much for a small regulator board without per thermal management.

For large voltage drops or high current loads, a switching buck converter is usually a better choice.

## Recommended Use Cases

* Microcontroller power rails
* ESP32 / Arduino jects
* Sensor modules
* Logic circuits
* Small robotics jects
* IoT devices
* PCB totypes
* Educational electronics jects
* Testing and bench jects
* Custom board power sections

## Manufacturing

The boards were designed in **EasyEDA ** and can be manufactured using services such as **JLCPCB**.

Each board should include:

* Schematic
* PCB layout
* BOM
* Gerber files
* EasyEDA ject file
* PCB preview images

The Gerber files and EasyEDA ject files are available through the OSHWLab links listed in each board section.
