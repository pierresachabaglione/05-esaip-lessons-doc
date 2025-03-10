<!--
SPDX-FileCopyrightText: 2025 Benoît Rolandeau <benoit.rolandeau@allcircuits.com>

SPDX-License-Identifier: MIT
-->

# Temperature sensor

## Table of contents <!-- omit from toc -->

- [Temperature sensor](#temperature-sensor)
  - [Presentation](#presentation)
  - [Needs](#needs)
    - [MUST have](#must-have)
    - [SHOULD have](#should-have)

## Presentation

This file contains **WHAT** your customer expects from the temperature sensor.

## Needs

### MUST have

- `NTS1`: the temperature sensor must be able to send temperature data to the server. This is
  telemetry data.
- `NTS2`: the temperature data must be sent every 10 seconds in active mode and every 20 seconds in
  sleep mode.
- `NTS3`: the temperature data must be fakeable and configurable by the user through a gui
  interface. The user must be able to set the temperature value with a precision of 0.1°C.
- `NTS4`: the temperature data sent to the server must always be in Celsius degrees.
- `NTS5`: the gui interface of the temperature sensor must show the current temperature unit set in
  the `server` attributes of the temperature sensor.
- `NTS6`: the temperature sensor must be able to send humidity data to the server. This is telemetry
  data.
- `NTS7`: the humidity data must be sent every 20 seconds in active mode and every 50 seconds in
  sleep mode.
- `NTS8`: the humidity data must be fakeable and configurable by the user through a gui interface.
  The user must be able to set the humidity value with a precision of 1%.
- `NTS9`: the humidity data sent to the server must always be in percentage.
- `NTS10`: the gui interface of the temperature sensor must contain a button to switch between the
  active and the sleep mode.
- `NTS11`: the temperature sensor must poll the server every 10 seconds in active mode and every 20
  seconds in sleep mode to get the `server` attributes of the temperature sensor.

### SHOULD have

- `NTS+1`: the temperature sensor should be able to connect to the server by WebSocket. The
  temperature sensor should be able to receive the `server` attributes in real-time. The temperature
  sensor should be able to switch between the HTTP and the WebSocket connection. In the WebSocket
  mode, the `client` attributes and the telemetry data should be sent through the WebSocket. The
  frequency of sending should be the same as in the HTTP mode.
