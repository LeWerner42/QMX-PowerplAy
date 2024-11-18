# USB-C PD adapter for QMX + 50W PA

The QMX-PowerplAy is designed to power the [QRP Labs QMX](https://qrp-labs.com/qmx.html) as well as the [50W PA](https://qrp-labs.com/50wpa.html) off a USB PD Powerbank.
Designed for ultimate portability for SOTA / POTA activations, the board can negotiate `15V` or `20V` with `3A` or `5A` for the PA.
A `12V, 5A` switching regulator powers the QMX. Power Negotiation can be selected with simple Jumpers.

## Hardware
### Schematic
The main component is the [AP33771C](https://www.mouser.ch/ProductDetail/Diodes-Incorporated/AP33771CFBZ-13-FA01?qs=2wMNvWM5ZX7JpCFGcPz6nw%3D%3D) which takes care of USB PD negotiations.
Output Voltage and Current can be set through Jumpers `JP1` and `JP2`.
[The Barrel Jack](https://www.mouser.ch/ProductDetail/Wurth-Elektronik/694106301002?qs=a9WhcLg8qCwOEkcI62k5mA%3D%3D) J2 (5.5mm) directly connects to the negotiated power from USB.
J3 (5.5mm) is connected to the stepped-down 12V for supplying the QMX
![schematic](./powerplay/schematic.png "Board Schematic")

### Manufacturing
PCBs can be ordered with the gerbers in [fabrication](./powerplay/fabrication).  
The [Component BOM](https://lewerner42.github.io/QMX-PowerplAy/powerplay/bom/ibom.html) [`powerplay/bom/ibom.html`] lists all neccessary components for soldering.
Be aware of Capacitor Voltage ratings (>= 20V) for capacitors connected to USB power.
![rendering](./powerplay/powerplay.png "Board Render")

## Case

## Usage
