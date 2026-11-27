# M487 Dual Master Module · Summing

Ward-Beck Systems M487, 1981|14. Wiki page: [M487 on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M487.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 65 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 6 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 5 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 161 |
| [PHOTOS/](PHOTOS/) | photographs of the module | 5 |
| [SOFTWARE/](SOFTWARE/) | program listings, firmware, the plugin | 1 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 17 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 43 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

**On the WBSps forum (2006|39 - 2014|47):** [8 topics](FORUM.md): what owners and technicians said about it.

## Specifications

From the technical data sheet: [1982 - M487 - Dual Master Module.pdf](MANUALS/1982%20-%20M487%20-%20Dual%20Master%20Module.pdf) page 2 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Gain** | 38 dB t/ -0.5 dB (bridging gain) |
| **Frequency response** | 0/-0.5 dB from 20 Hz to 20 kHz. (tailored frequency response) |
| **Noise** | 72 dB below +8 dBm output level (20 Hz to 20 kHz) |
| **Harmonic distortion** | Less than 0.257 THD from 30 Hz to 20 kHz at +24 dBm output or less. Less than 0.1% at kHz at +24 dBm outpul |
| **Source impedances** |  |
| &nbsp;&nbsp;Summing | External 30,000 ohms, balanced _ 600 ohms max imur, balanced. |
| **Input impedances** |  |
| &nbsp;&nbsp;Summing external | Less than ohms. 600 ohms, balanced. |
| &nbsp;&nbsp;Input level | External 48 dBm nominal, +24 dBm Maximum. |
| **Output impedances** | Out #1: Out #2: vu/Monitor Out: 600 ohms, balanced. 600 ohms, balanced 600 ohms, balanced. |
| **Load impedances** | Out #1: Out #2: VU/Monitor Out: 600 ohms, balanced 600 ohms, balanced Bridging, balanced (5000 ohms minimum) |
| **Output level** | Out #1: Out #2: VU/Monitor Out: +8 dBm nominal +24 dBm maximum. +8 dBm nominal, +24 dBm maximum. +8 dBrr nominal, +24 dBm maximum. |

## Circuit description

From [1982 - M487 - Dual Master Module.pdf](MANUALS/1982%20-%20M487%20-%20Dual%20Master%20Module.pdf) pages 4-8 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

The M487 Dual Master Module accommodates IWo seperale signal channels Tt is designed to receive the mixer feeds irom the summing buses of an audio mixing console The [wo sections of the unit process and amplify their signals to standard Line levels. The outputs of the M487 supply the main outputs of the mixing console. Both channels operate in similar manner. The follow ing description refers specifically Lo SECTION Lout The signal originating from the external summing bus enters the module at Pins and of the connector and i5 applied to the sumi ing nodes af U1 and U2. An external 600 ohm input is also provided and appears at pins and of the module connector. The nominal level of this external input 15 +8 dBm while the summing input operates 4[ -15 dBm from 30k ohm current source U1 through u3 with their associated components provide actively balanced inputs 45 wel as balanced output. The outpul of the preamplifier operates at nominal Level of -10 dBm and appears at pins 10 and of the module connector Attenuator Insert The balanced INSERT point, provided between pins 10 &amp; Land 11 &amp; M of the connector permits the insertion of an external altenuator and the reference oscillator slating selector. Output The 8-109C output amplifier operates with gain of 39 dB Tt recovers the signal loss of the attenuator and provides additional gain to produce nominal output level of +8 dBm at the module outputs. The output from the 8-109C is divides Tnto three por(5. The first (PGM 1) is an actively balanced 600 ohm output prov 'ding the direct master output. The second (PGM 2) is low impedance output routed to the T12024 output line selector, while the third provides an Isolated monitoring and metering output.

WAAD-BECK Bystems LTD; CIRcuiT DESCRIPTION

Power SuPply DecoUpl ing An active power supply decoup | ing network consisting of 01 through 06 provides isolation between the module and the +/ -25 volts power supply Transistors 03 and 06 monitor the supply current. In the event of excessive power supply demands, such 45 from component failure or amplifier overdrive, the current flow ing through 01 and 04 will be Vimited_ CRI and CR2 guard against inadvertent application of reverse power supply voltages

PARTS LiST

**C1 C2 C3 C4 C5**

Capacitor 330 uF/6 Kemet

**1390F 337MOO6AS**

47 pF Philips 2222-638-70479 C6 C7 C8 c9 C10 47 pF 4.7 pF 2222-638-09478 C1I C12 C13) C1b) C15 82 pF 2222-638-70829 delete Capacitor 47 pF 2222-638-70479

**C16 C17 C18 C19 C20**

6800 pF Aselco cQ92 MC-682m 6.8 pF 2222-638-09688

**C21 C22 C23 C24 C25**

68 uF/10 Kemnet

**22 UF/25**

Philips

**CRI CRZ CR3 CR4**

Diode Motorola

**IN403**

01 02 Transistor Tex. Inst. National

**TIP29B PN3569**

PARTS LiST

**MFG PART NUMBER**

03 04 05 06 Transistor National Tex. Inst. National PN3569 TiP30B PN3645

**RI R2 R3 R4 RS**

Resistor I/4w 5% 220k 220k 220k 220k 15k Philips R6 R7 R8 R9 R10 15k 15k 15k 15k 15k

**RII R12 RIJ R14 R15**

15k 15k 620 620 12K

Trim Pot

Piher PT 1Ov (2.5) 2k

Resistor 1/4w 59 11K Philips

Trim Pot

Piher PT 10v (2.5) 2k

**R20 R21 R22 R23 R24**

Resistor '/4w 5% 11k 470k 470K 18K 18K Philips

**R25 R26 R27 R28 R29**

15k 15k 620 620 15k

</details>

<!-- /module data -->

## Photos

_Photographs of the module itself: front, back, inside, racked._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYTVwRzBOS3JxMGc/view?resourcekey=0-UEzP7u3w0CPT5UOJZ6SGLw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYTVwRzBOS3JxMGc&resourcekey=0-UEzP7u3w0CPT5UOJZ6SGLw" width="240" alt="1982 - M487 - Mixer Slot.jpg"></a><br><sub>1982|15 · Mixer Slot</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTkZmRzdHajA3Ymc/view?resourcekey=0-lP_cZ_HNEGaCj48HRpt6Zg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTkZmRzdHajA3Ymc&resourcekey=0-lP_cZ_HNEGaCj48HRpt6Zg" width="240" alt="1982 - M487 - Preamp.jpg"></a><br><sub>1982|15 · Preamp</sub></td></tr>
</table>

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSWQ4LWo2N01MRW8/view?resourcekey=0-HONMjFQUNiYS3FNM5KZfNw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSWQ4LWo2N01MRW8&resourcekey=0-HONMjFQUNiYS3FNM5KZfNw" width="240" alt="19xx - M487 - DOC - 1202-04-007 - OSCILLATOR CUE-SOLO RE-ENTRY AND AUX LEVEL SCHEMATIC.jpg"></a><br><sub>19xx - M487 - DOC - 1202-04-007 - OSCILLATOR CUE-SOLO RE-ENTRY AND AUX LEVEL SCHEMATIC · <a href="MECHANICAL/19xx%20-%20M487%20-%20DOC%20-%201202-04-007%20-%20OSCILLATOR%20CUE-SOLO%20RE-ENTRY%20AND%20AUX%20LEVEL%20SCHEMATIC%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKT094Yk5yM0dZcUk/view?resourcekey=0-2rQcc7ZpKYk8r1g3eBNYxQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKT094Yk5yM0dZcUk&resourcekey=0-2rQcc7ZpKYk8r1g3eBNYxQ" width="240" alt="1982 - M487 - 487-01-001 - DUAL MASTER MODULE FUNCTIONAL DIAGRAM.jpg"></a><br><sub>1982|15 · 487-01-001 - DUAL MASTER MODULE FUNCTIONAL DIAGRAM · <a href="SCHEMATICS/1982%20-%20M487%20-%20487-01-001%20-%20DUAL%20MASTER%20MODULE%20FUNCTIONAL%20DIAGRAM%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbzJEVEhKRHB5bTg/view?resourcekey=0-9kuTeSQ8YEC1o8HeKdQkEg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbzJEVEhKRHB5bTg&resourcekey=0-9kuTeSQ8YEC1o8HeKdQkEg" width="240" alt="1982 - M487 - 487-02-001 - DUAL MASTER MODULE SCHEMATIC.jpg"></a><br><sub>1982|15 · 487-02-001 - DUAL MASTER MODULE SCHEMATIC · <a href="SCHEMATICS/1982%20-%20M487%20-%20487-02-001%20-%20DUAL%20MASTER%20MODULE%20SCHEMATIC%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeFNPend1em9EZG8/view?resourcekey=0-aZddMPRsjhbo1SiFzqgO7w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeFNPend1em9EZG8&resourcekey=0-aZddMPRsjhbo1SiFzqgO7w" width="240" alt="1982 - M487 - 487-02-001 - OLHG DUAL MASTER MODULE.jpg"></a><br><sub>1982|15 · 487-02-001 - OLHG DUAL MASTER MODULE · <a href="SCHEMATICS/1982%20-%20M487%20-%20487-02-001%20-%20OLHG%20DUAL%20MASTER%20MODULE%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOElBbVl1Q21ORk0/view?resourcekey=0-4JLXScj_XZlcNSZzCIL0Qg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOElBbVl1Q21ORk0&resourcekey=0-4JLXScj_XZlcNSZzCIL0Qg" width="240" alt="1982 - M487 - 487-06-001 - DUAL MASTER MODULE COMPONENT LAYOUT ENG.jpg"></a><br><sub>1982|15 · 487-06-001 - DUAL MASTER MODULE COMPONENT LAYOUT ENG · <a href="SCHEMATICS/1982%20-%20M487%20-%20487-06-001%20-%20DUAL%20MASTER%20MODULE%20COMPONENT%20LAYOUT%20ENG%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNEJoNnNod0kxVWM/view?resourcekey=0-mvadPXpdDNU_dq6qzEfmLg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNEJoNnNod0kxVWM&resourcekey=0-mvadPXpdDNU_dq6qzEfmLg" width="240" alt="1982 - M487 - 487-06-001.jpg"></a><br><sub>1982|15 · 487-06-001 · <a href="SCHEMATICS/1982%20-%20M487%20-%20487-06-001%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKa1NCQWhjXzFVYUE/view?resourcekey=0-1K_WDhKSYmrIQW2rURMZSQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKa1NCQWhjXzFVYUE&resourcekey=0-1K_WDhKSYmrIQW2rURMZSQ" width="240" alt="1982 - M487 - 8-109-02-004.jpg"></a><br><sub>1982|15 · 8-109-02-004 · <a href="SCHEMATICS/1982%20-%20M487%20-%208-109-02-004%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTjdCT2Q5WU56MXc/view?resourcekey=0-Z5m1Z34X3Z2A1oNV7C13YQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTjdCT2Q5WU56MXc&resourcekey=0-Z5m1Z34X3Z2A1oNV7C13YQ" width="240" alt="1982 - M487 - 8-109-06-004 - BOOSTER AMPLIFIER COMPONENT LAYOUT.jpg"></a><br><sub>1982|15 · 8-109-06-004 - BOOSTER AMPLIFIER COMPONENT LAYOUT · <a href="SCHEMATICS/1982%20-%20M487%20-%208-109-06-004%20-%20BOOSTER%20AMPLIFIER%20COMPONENT%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKd214S080ZkxQbDA/view?resourcekey=0-ZdE_XEF3vVJwwYYnKqCRvg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKd214S080ZkxQbDA&resourcekey=0-ZdE_XEF3vVJwwYYnKqCRvg" width="240" alt="1982 - M487 - 8-109-06-004 - BOOSTER AMPLIFIER.jpg"></a><br><sub>1982|15 · 8-109-06-004 - BOOSTER AMPLIFIER · <a href="SCHEMATICS/1982%20-%20M487%20-%208-109-06-004%20-%20BOOSTER%20AMPLIFIER%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKY3Z5VDB6ZC1KcE0/view?resourcekey=0-FOXGYaXjCh5kQRDk-YQE1Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKY3Z5VDB6ZC1KcE0&resourcekey=0-FOXGYaXjCh5kQRDk-YQE1Q" width="240" alt="1982 - M487 - B 487-01-001 - M487 - DUAL MASTER MODULE - FUNCTIONAL DIAGRAM.jpg"></a><br><sub>1982|15 · B 487-01-001 - M487 - DUAL MASTER MODULE - FUNCTIONAL DIAGRAM · <a href="SCHEMATICS/1982%20-%20M487%20-%20B%20487-01-001%20-%20M487%20-%20DUAL%20MASTER%20MODULE%20-%20FUNCTIONAL%20DIAGRAM%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdUlSMm9QV3hlVjg/view?resourcekey=0-5WSKSoM4AlodWTdCBiZJ7w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdUlSMm9QV3hlVjg&resourcekey=0-5WSKSoM4AlodWTdCBiZJ7w" width="240" alt="1982 - M487 - BOOSTER AMPLIFIER SCHEMATIC.jpg"></a><br><sub>1982|15 · BOOSTER AMPLIFIER SCHEMATIC · <a href="SCHEMATICS/1982%20-%20M487%20-%20BOOSTER%20AMPLIFIER%20SCHEMATIC%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSzVWcnpkTEFZTm8/view?resourcekey=0-FJF7HDRRrq82yig-wShWHg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSzVWcnpkTEFZTm8&resourcekey=0-FJF7HDRRrq82yig-wShWHg" width="240" alt="19xx - M487 - DOC - 1202-02-012 - OOP SHE-DS.jpg"></a><br><sub>19xx - M487 - DOC - 1202-02-012 - OOP SHE-DS · <a href="SCHEMATICS/19xx%20-%20M487%20-%20DOC%20-%201202-02-012%20-%20OOP%20SHE-DS%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSW9DVDFJUjhHNDA/view?resourcekey=0-LsRL7zmoNnMRkR9JkF5V2A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSW9DVDFJUjhHNDA&resourcekey=0-LsRL7zmoNnMRkR9JkF5V2A" width="240" alt="19xx - M487 - DOC - 1202-02-017 - POSTS CHASSIS GROUND.jpg"></a><br><sub>19xx - M487 - DOC - 1202-02-017 - POSTS CHASSIS GROUND · <a href="SCHEMATICS/19xx%20-%20M487%20-%20DOC%20-%201202-02-017%20-%20POSTS%20CHASSIS%20GROUND%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/1P-iAWGc4d_YV1wYgzhOOBKaQ3Hc77147/view" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=1P-iAWGc4d_YV1wYgzhOOBKaQ3Hc77147" width="240" alt="19xx - M487 - DOC - 481-02-002 - CUE OSC RE-ENTRY MODULE SCHEMATIC.jpg"></a><br><sub>19xx - M487 - DOC - 481-02-002 - CUE OSC RE-ENTRY MODULE SCHEMATIC · <a href="SCHEMATICS/19xx%20-%20M487%20-%20DOC%20-%20481-02-002%20-%20CUE%20OSC%20RE-ENTRY%20MODULE%20SCHEMATIC%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/13RkYzR0ht6lU4gY8G4s33nh-AMUfGvvg/view" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=13RkYzR0ht6lU4gY8G4s33nh-AMUfGvvg" width="240" alt="19xx - M487 - DOC - 487-02-001 - DUAL MASTER MODULE SCHEMATIC.jpg"></a><br><sub>19xx - M487 - DOC - 487-02-001 - DUAL MASTER MODULE SCHEMATIC · <a href="SCHEMATICS/19xx%20-%20M487%20-%20DOC%20-%20487-02-001%20-%20DUAL%20MASTER%20MODULE%20SCHEMATIC%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

Not on Google Drive yet: `1981 - 487-02-001 - DUAL MASTER MODULE SCHEMATIC - DRN P. Mahoney - ENG MRW - ISS 3.jpg`, `19xx - 487-01-001 - DUAL MASTER MODULE FUNCTIONAL DIAGRAM - DRN P. Mahoney - ENG RKB - ISS 1 (2).jpg`

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

Not on Google Drive yet: `M487 - RTO-144 Connections.pdf`

## RTO-144 pinout

RTO-144 edge connector. Every contact, with where it was read: [`RTO.json`](RTO.json).

| Pin | Signal | Kind | Pair | Confidence |
|---|---|---|---|---|

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKajBqekNaYkFHZWc/view?resourcekey=0-EYaCXm2HN2tGhoOt4gQZiA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKajBqekNaYkFHZWc&resourcekey=0-EYaCXm2HN2tGhoOt4gQZiA" width="240" alt="1982 - M487 - Dual Master Module (2).pdf"></a><br><sub>1982|15 · Dual Master Module (2)</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWTdHcmduQ3J5b0k/view?resourcekey=0-eg6s-1b5p5ftmkMXbR14qg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWTdHcmduQ3J5b0k&resourcekey=0-eg6s-1b5p5ftmkMXbR14qg" width="240" alt="1982 - M487 - Dual Master Module.pdf"></a><br><sub>1982|15 · Dual Master Module</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUndKbFozTEhvckk/view?resourcekey=0-vT21jv4kxtRjimQAbOXo7A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUndKbFozTEhvckk&resourcekey=0-vT21jv4kxtRjimQAbOXo7A" width="240" alt="1982 - M487 - P01 - TOC.jpg"></a><br><sub>1982|15 · P01 - TOC</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKX3RwYjdYX2hXYlE/view?resourcekey=0-wbf9AOFZu4wsuOQj5SsfLA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKX3RwYjdYX2hXYlE&resourcekey=0-wbf9AOFZu4wsuOQj5SsfLA" width="240" alt="1982 - M487 - P02 - 1-1.jpg"></a><br><sub>1982|15 · P02 - 1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWDJsVEc3QlozT2M/view?resourcekey=0-uEG5rh4PxPfMzDL5VN2Nug" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWDJsVEc3QlozT2M&resourcekey=0-uEG5rh4PxPfMzDL5VN2Nug" width="240" alt="1982 - M487 - P03 - 1-2.jpg"></a><br><sub>1982|15 · P03 - 1-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbzhsOXRWY2huQ28/view?resourcekey=0-4ur_zZgEreFJCYPvx60G0g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbzhsOXRWY2huQ28&resourcekey=0-4ur_zZgEreFJCYPvx60G0g" width="240" alt="1982 - M487 - P04 - 2-1.jpg"></a><br><sub>1982|15 · P04 - 2-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUmJWalRuNFJ4Ums/view?resourcekey=0-ZILoUt0dBzo33i2tgZhFXw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUmJWalRuNFJ4Ums&resourcekey=0-ZILoUt0dBzo33i2tgZhFXw" width="240" alt="1982 - M487 - P05 - 2-2.jpg"></a><br><sub>1982|15 · P05 - 2-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKamplVEJYalllQkE/view?resourcekey=0-trl4KNvqHiQCrog7lxPyiA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKamplVEJYalllQkE&resourcekey=0-trl4KNvqHiQCrog7lxPyiA" width="240" alt="1982 - M487 - P06 - 3-1.jpg"></a><br><sub>1982|15 · P06 - 3-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMUNxcjlJcGFtbW8/view?resourcekey=0-9V76f-CZ2i4f0vg87gajDA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMUNxcjlJcGFtbW8&resourcekey=0-9V76f-CZ2i4f0vg87gajDA" width="240" alt="1982 - M487 - P07 - 3-2.jpg"></a><br><sub>1982|15 · P07 - 3-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWVpLRk9EQkNsTDQ/view?resourcekey=0-9wpXTRZM0qtUmUnFWQhfdw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWVpLRk9EQkNsTDQ&resourcekey=0-9wpXTRZM0qtUmUnFWQhfdw" width="240" alt="1982 - M487 - P08 - 3-3.jpg"></a><br><sub>1982|15 · P08 - 3-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSVEwSlpDQWZTalU/view?resourcekey=0-2frPOyPycD2xu_wxtQDBcw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSVEwSlpDQWZTalU&resourcekey=0-2frPOyPycD2xu_wxtQDBcw" width="240" alt="1982 - M487 - P09 - 3-4.jpg"></a><br><sub>1982|15 · P09 - 3-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaW9xNzBic3A1b2M/view?resourcekey=0-XaHeMPbj_AK38dt-sLnURg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaW9xNzBic3A1b2M&resourcekey=0-XaHeMPbj_AK38dt-sLnURg" width="240" alt="1982 - M487 - P10 - 4-1.jpg"></a><br><sub>1982|15 · P10 - 4-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTmhsSEVDZ2V4MWs/view?resourcekey=0-BvT5Xg1vhpQPKIREd2KEng" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTmhsSEVDZ2V4MWs&resourcekey=0-BvT5Xg1vhpQPKIREd2KEng" width="240" alt="1982 - M487 - P11.jpg"></a><br><sub>1982|15 · P11</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZHFKSkQ4a1FZZjQ/view?resourcekey=0-zuBJJkO1AeC3n-x4Z1_pcA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZHFKSkQ4a1FZZjQ&resourcekey=0-zuBJJkO1AeC3n-x4Z1_pcA" width="240" alt="1982 - M487 - P12 - 8-109-1-1.jpg"></a><br><sub>1982|15 · P12 - 8-109-1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZF9PVUdjTFViSVk/view?resourcekey=0-JJLYYDxic4NAciVyCzHwaQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZF9PVUdjTFViSVk&resourcekey=0-JJLYYDxic4NAciVyCzHwaQ" width="240" alt="1982 - M487 - P13 - 8-109-1-2.jpg"></a><br><sub>1982|15 · P13 - 8-109-1-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdmplY3liSko5a2c/view?resourcekey=0-PuuzlkbC1k95w0nVOnPbFQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdmplY3liSko5a2c&resourcekey=0-PuuzlkbC1k95w0nVOnPbFQ" width="240" alt="1982 - M487 - P14 - 8-109-2-1.jpg"></a><br><sub>1982|15 · P14 - 8-109-2-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZC1IZ2p6Qnl6Q0E/view?resourcekey=0-PbYlKzmTenLXpWu8Gy_34Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZC1IZ2p6Qnl6Q0E&resourcekey=0-PbYlKzmTenLXpWu8Gy_34Q" width="240" alt="1982 - M487 - P15 - 8-109-2-2.jpg"></a><br><sub>1982|15 · P15 - 8-109-2-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUGdjQWc0MnZVWWs/view?resourcekey=0-8xOMglRmt6rtKaEkyS8zAw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUGdjQWc0MnZVWWs&resourcekey=0-8xOMglRmt6rtKaEkyS8zAw" width="240" alt="1982 - M487 - P16 - 8-109-2-3.jpg"></a><br><sub>1982|15 · P16 - 8-109-2-3</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOVpKcVd5SVhvY0k/view?resourcekey=0-UNdeNf3B4jwH_VRzhOGHDw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOVpKcVd5SVhvY0k&resourcekey=0-UNdeNf3B4jwH_VRzhOGHDw" width="240" alt="1982 - M487 - P17 - 8-109-2-4.jpg"></a><br><sub>1982|15 · P17 - 8-109-2-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNnp0cFpaT21BSWc/view?resourcekey=0-U1oh9PIlSNk0kWR2rInFDg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNnp0cFpaT21BSWc&resourcekey=0-U1oh9PIlSNk0kWR2rInFDg" width="240" alt="1982 - M487 - P18 - 8-109-2-5.jpg"></a><br><sub>1982|15 · P18 - 8-109-2-5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMi1rcjZwbXMyOUE/view?resourcekey=0-V82wewC7Mz-xGA5v3tieXg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMi1rcjZwbXMyOUE&resourcekey=0-V82wewC7Mz-xGA5v3tieXg" width="240" alt="19xx - M487 - DOC - L1202A - P12 - 1-9.jpg"></a><br><sub>19xx - M487 - DOC - L1202A - P12 - 1-9</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRGVVUmx1MlN1ek0/view?resourcekey=0-vJM2sfewluMBwXhSfCFOAg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRGVVUmx1MlN1ek0&resourcekey=0-vJM2sfewluMBwXhSfCFOAg" width="240" alt="19xx - M487 - DOC - L1202A - P25 - IV-1.jpg"></a><br><sub>19xx - M487 - DOC - L1202A - P25 - IV-1</sub></td></tr>
</table>

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [1981 - 487-02-001 - DUAL MASTER MODULE SCHEMATIC - DRN P. Mahoney - ENG MRW - ISS 3.kicad_sch](KICAD/1981%20-%20487-02-001%20-%20DUAL%20MASTER%20MODULE%20SCHEMATIC%20-%20DRN%20P.%20Mahoney%20-%20ENG%20MRW%20-%20ISS%203.kicad_sch)
- [1982 - M487 - 487-01-001 - DUAL MASTER MODULE FUNCTIONAL DIAGRAM.kicad_sch](KICAD/1982%20-%20M487%20-%20487-01-001%20-%20DUAL%20MASTER%20MODULE%20FUNCTIONAL%20DIAGRAM.kicad_sch)
- [1982 - M487 - 487-02-001 - DUAL MASTER MODULE SCHEMATIC.kicad_sch](KICAD/1982%20-%20M487%20-%20487-02-001%20-%20DUAL%20MASTER%20MODULE%20SCHEMATIC.kicad_sch)
- [1982 - M487 - 487-02-001 - OLHG DUAL MASTER MODULE.kicad_sch](KICAD/1982%20-%20M487%20-%20487-02-001%20-%20OLHG%20DUAL%20MASTER%20MODULE.kicad_sch)
- [1982 - M487 - 8-109-02-004.kicad_sch](KICAD/1982%20-%20M487%20-%208-109-02-004.kicad_sch)
- [1982 - M487 - B 487-01-001 - M487 - DUAL MASTER MODULE - FUNCTIONAL DIAGRAM.kicad_sch](KICAD/1982%20-%20M487%20-%20B%20487-01-001%20-%20M487%20-%20DUAL%20MASTER%20MODULE%20-%20FUNCTIONAL%20DIAGRAM.kicad_sch)
- [1982 - M487 - BOOSTER AMPLIFIER SCHEMATIC.kicad_sch](KICAD/1982%20-%20M487%20-%20BOOSTER%20AMPLIFIER%20SCHEMATIC.kicad_sch)
- [1982 - M487 - Dual Master Module p19.kicad_sch](KICAD/1982%20-%20M487%20-%20Dual%20Master%20Module%20p19.kicad_sch)
- [1982 - M487 - Dual Master Module p20.kicad_sch](KICAD/1982%20-%20M487%20-%20Dual%20Master%20Module%20p20.kicad_sch)
- [1982 - M487 - Dual Master Module p22.kicad_sch](KICAD/1982%20-%20M487%20-%20Dual%20Master%20Module%20p22.kicad_sch)
- [19xx - 487-01-001 - DUAL MASTER MODULE FUNCTIONAL DIAGRAM - DRN P. Mahoney - ENG RKB - ISS 1 (2).kicad_sch](KICAD/19xx%20-%20487-01-001%20-%20DUAL%20MASTER%20MODULE%20FUNCTIONAL%20DIAGRAM%20-%20DRN%20P.%20Mahoney%20-%20ENG%20RKB%20-%20ISS%201%20(2).kicad_sch)
- [19xx - M487 - DOC - 1202-02-012 - OOP SHE-DS.kicad_sch](KICAD/19xx%20-%20M487%20-%20DOC%20-%201202-02-012%20-%20OOP%20SHE-DS.kicad_sch)
- [19xx - M487 - DOC - 1202-02-017 - POSTS CHASSIS GROUND.kicad_sch](KICAD/19xx%20-%20M487%20-%20DOC%20-%201202-02-017%20-%20POSTS%20CHASSIS%20GROUND.kicad_sch)
- [19xx - M487 - DOC - 481-02-002 - CUE OSC RE-ENTRY MODULE SCHEMATIC.kicad_sch](KICAD/19xx%20-%20M487%20-%20DOC%20-%20481-02-002%20-%20CUE%20OSC%20RE-ENTRY%20MODULE%20SCHEMATIC.kicad_sch)
- [19xx - M487 - DOC - 487-02-001 - DUAL MASTER MODULE SCHEMATIC.kicad_sch](KICAD/19xx%20-%20M487%20-%20DOC%20-%20487-02-001%20-%20DUAL%20MASTER%20MODULE%20SCHEMATIC.kicad_sch)
- [M487.kicad_sym](KICAD/M487.kicad_sym)
- [index.html](KICAD/index.html)

## Software

- [index.html](SOFTWARE/index.html)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
