# General instructions

This repository contains all the hardware design files related to the underwater electronics being developed for smartboxes, positioning, and sonar applications.

## Kicad/
KiCad design files for the PCB.

- `FullDesign/` — Full KiCad project (schematic, PCB layout, project file). Includes automatic backups in `FullDesign-backups/`.
- `extraSymbols.kicad_sym` — Custom symbol library with components not available in the default KiCad libraries.

## Datasheets/
Datasheets for the custom components added to the `extraSymbols` library. Includes:

| File | Component |
|------|-----------|
| `622012fc.pdf` | 622012FC |
| `AD8031_8032.pdf` | AD8031 / AD8032 op-amps |
| `B130LAW.pdf` | B130LAW Schottky diode |
| `J109-D.PDF` | J109 JFET |
| `LSK170SeriesDSRevA22.pdf` | LSK170 JFET |
| `MAX14756-MAX14758.pdf` | MAX14756/57/58 analog switches |
| `MMBFJ270-D.PDF` | MMBFJ270 JFET |
| `PMEG6010CEH.pdf` | PMEG6010CEH Schottky diode |
| `SS26FL-D.PDF` | SS26FL Schottky diode |
| `ad5245.pdf` | AD5245 digital potentiometer |
| `adc121s101.pdf` | ADC121S101 ADC |
| `dac8411.pdf` | DAC8411 DAC |
| `lmz14201h.pdf` | LMZ14201H power module |
| `tps22918.pdf` | TPS22918 load switch |
| `tps62120.pdf` | TPS62120 buck converter |

All other datasheets are available from KiCad.

## LT simulations/
LTspice circuit simulations and the SPICE model libraries they depend on.

| File | Description |
|------|-------------|
| `Rx filter.asc` | Full receiver simulation including filters, preamplification, and amplification until the ADC |
| `Tx filter.asc` | Transmitter filter simulation |
| `LT Rx connection.cir` | Simulaation for the connection to Rx using transistors |
| `TX power.cir` | Simulation of the tx power amplification |
| `OPA551.LIB` | SPICE model for OPA551 op-amp |
| `OPA55x.LIB` | SPICE model for OPA552 op-amp |

## BOM.xlsx

Bill of Materials for all ICs in the full design. It contains, name, quantity, price, where is it use, and link to buy in mouser.