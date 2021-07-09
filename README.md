# Introduction

This repository contains a series of demo/test waveforms, acquired from a variety of oscilloscopes, for use with
glscopeclient and libscopehal.

Files are listed alphabetically below, along with a list of the features they demonstrate.

## Automotive

### CAN.scopesession

Source: Teledyne LeCroy HDO9204

* CAN
* Clock Recovery (PLL)
* Eye Pattern
* Subtract
* Threshold

## Aviation

### ARINC429.scopesession

Source: Agilent MSO-X 3024A

This is a placeholder dataset containing a waveform but no decodes as the ARINC 429 decode hasn't been written yet.

### MIL-STD-1553.scopesession

Source: Digilent ADP3450

* MIL-STD-1553

## Embedded

### 1-Wire.scopesession

Source: CSV import, original instrument unknown

Note: The device this dataset came from has a bug and the initial reset pulse is slightly too short. The decode
correctly flags this as a problem.

* 1-Wire
* Threshold

### I2CEEprom.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

* Threshold
* I2C
* I2C EEPROM

## Memory

### DDR1.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

Note: This dataset also contains analog signals for DQS and a single DQ line however DQ eye rendering isn't
quite fully debugged so that's not included.

* DDR1 Command Bus

### DDR3.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS, Teledyne LeCroy HDO9204

Note: This dataset was collected using the multi-scope sync feature from two different scopes.
The DUT is an embedded device that runs DDR3 in DLL-off mode at 250 MT/s (125 MHz clock).

* Threshold
* DDR3 Command Bus

### SDCard.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

* SD Card Command Bus
* SD Card Data Bus

## Miscellaneous

### FanPWM.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

* Duty Cycle
* Tachometer

### QuadratureEncoder.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

* Quadrature
* Threshold

## Mobile

### DSI.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

Note: Gated clock eye rendering removed due to bugs still being investigated

* MIPI D-PHY Symbol
* MIPI DSI Packet
* MIPI DSI Frame
* Subtract

## Networking

### 10Base-T.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

* 10Base-T
* IPv4
* Subtract

### 100Base-TX.scopesession

Source: Teledyne LeCroy SDA 816Zi

* 100Base-TX
* Clock Recovery (PLL)
* Eye Pattern
* IPv4
* Subtract

### 1000base-X.scopesession

Source: Teledyne LeCroy HDO9204

* 1000Base-X
* 8B/10B (IBM)
* Clock Recovery (PLL)
* Threshold
* Eye Pattern

### 10Gbase-R.scopesession

Source: Teledyne LeCroy SDA 816Zi

* 10Gbase-R
* 64b/66b
* Clock Recovery (PLL)
* Eye Pattern
* IPv4
* Threshold

### Autonegotiation.scopesession

Source: Teledyne LeCroy SDA 816Zi

* Ethernet Autonegotiation
* Subtract

### MDIO.scopesession

Source: Teledyne LeCroy HDO9204

* Threshold
* MDIO

## PC

### HDMI.scopesession

Source: Teledyne LeCroy DDA5005A

NOTE: There is currently no HDMI decode, and the TMDS decode chokes on HDMI guard bands.

* 8B/10B (TMDS)
* Clock Recovery (PLL)
* Threshold

### PCIe.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

* 1000Base-X
* 8B/10B (IBM)
* Clock Recovery (PLL)
* Emphasis Removal
* Eye Pattern
* IPv4
* PCIe Gen1/2 Logical
* PCIe Data Link
* PCIe Transport
* Threshold

## RF

### Filters.scopesession

Source: Teledyne LeCroy WaveRunner 8404M-MS

* FFT
* FIR Filter

### QPSK.scopesession

Source: Teledyne LeCroy WaveSurfer 3034

NOTE: The signal generator for this test is set up incorrectly, so one of the phases is 45 rather than 90 degrees
offset from the others.

* Downconvert
* FIR Filter
* Phase
