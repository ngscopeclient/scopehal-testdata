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

## Embedded

### 1-Wire.scopesession

Source: CSV import, original instrument unknown

Note: The device this waveform came from has a bug and the initial reset pulse is slightly too short. The decode
correctly flags this as a problem.

* 1-Wire
* Threshold

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
