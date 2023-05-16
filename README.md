
# RFM9x Breakout Board

<img width="400px" src="https://user-images.githubusercontent.com/15846193/63650613-b8009a80-c74c-11e9-89e6-29d23c01b0fb.JPG"></br>

<img width="400px" src="https://user-images.githubusercontent.com/15846193/63650674-7de3c880-c74d-11e9-94c1-2ace51b7b5a7.png">

### Description

The RFM9x Breakout Board is a breadboard friendly PCB, converting the 2mm pitch connectors on the HopeRF modules to a more user friendly 2.54mm (0.100″) pitch footprint, used in standard breadboards. Using the breadboard, the developers can easily create IoT modules with 430MHz, 868MHz or 905MHz in their projects and add LoRaWAN capabilities to them.

### Features

- small size
- breadboard friendly (pin spacing 2.54mm)
- the board includes combined footprint for SMA edge as well as SMD u.Fl antenna connector, so both connectors can be applied separately or together depends on what is needed
- optional circuit for power indication
- optional pullup resistor to keep high voltage level on NCC pin in case the RFM95W/96W/98W module is connected to MCU that requires programming via FTDI

### Schematic

_schematic_<br />
<img width="900px" src="https://user-images.githubusercontent.com/15846193/67626541-ee41bf80-f84c-11e9-84ca-e3ff10501ca9.png">

Nothing special on the schematic. The components R1, R2 and D1 are optional and can be omitted if not needed. R1 is used as pullup to keep high voltage level on the NCC pin. This allows programming the RFM95W/96W/98W module in case the board is interfaced to external microcontroller and ISP is used as a programming interface. R2 and D1 are used as power indication.

### Boards

#### Revision 1b:

Updates in revision 1b include:
- added support for SMD u.Fl antenna connector
- added open source hardware logo to the layout of the board

_top side_<br />
<img width="200px" src="https://user-images.githubusercontent.com/15846193/67626468-06650f00-f84c-11e9-9a32-1fd6ca4eea67.png">

_bottom side_<br />
<img width="200px" src="https://user-images.githubusercontent.com/15846193/67626477-21378380-f84c-11e9-9949-5bb277921c48.png">

#### Revision 1:

Initial revision, obsolete.

_top side_<br />
<img width="200px" src="https://user-images.githubusercontent.com/15846193/67624759-3b199c00-f835-11e9-97bf-f37639b97d7c.png">

_bottom side_<br />
<img width="200px" src="https://user-images.githubusercontent.com/15846193/67624768-54224d00-f835-11e9-90ae-d462c66fc7b4.png">

### BOM

All components are 0805 sized and you can buy them everywhere.

| id | designator | value     | description        | quantity | datasheet             | supplier | note     |
|----|------------|-----------|--------------------|----------|-----------------------|----------|----------|
| 1  | R1         | 10k       | Resistor SMD 0805  | 1        |                       |          | optional |
| 2  | R2         | 330       | Resistor SMD 0805  | 1        |                       |          | optional |
| 3  | C1         | 10uF      | Capacitor SMD 0805 | 1        |                       |          | required |
| 4  | D1         | LED       | LED 0805           | 1        |                       |          | optional |
| 5  | J1         | Connector | SMD Edge Connector | 1        |                       |          | optional |
| 6  | J1         | Connector | SMA u.Fl Connector | 1        |                       |          | optional |
| 7  | U1         | RFM9xW    | RFM9xW module      | 1        | [datasheet][a173d720] | HopeRF   | required |

[a173d720]:https://www.hoperf.com/data/upload/portal/20190801/RFM95W-V2.0.pdf "RFM95x"

### Project status

The most recent version (rev. 1b) is tested and works fine. Previous version (rev. 1) is still valid but obsolete, therefore it is not available for purchase.

### Purchase

The board can be purchased from the [AISLER.net](https://aisler.net/) web store by clicking on thes [link](https://aisler.net/p/BNYBJOFL). You can also try to purchase it from 
the [PCBs.io](https://PCBs.io/share/4QJV1) web store. If you do so, PCBs.io gives me a small reward that helps when I purchase some newly created boards.

## License

<img width="100px" src="https://user-images.githubusercontent.com/15846193/42368218-bf6374f6-8106-11e8-91b4-e5df463580d6.jpg" /><br />

Copyright © 2019 Boyan Nedkov. All rights reserved.<br />
Licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License][1]. For permissions beyond the scope of this license please [contact me][2] so we can arrange a simple agreement.

[1]: http://creativecommons.org/licenses/by-nc/4.0/
[2]: mailto:attexx@gmx.com
