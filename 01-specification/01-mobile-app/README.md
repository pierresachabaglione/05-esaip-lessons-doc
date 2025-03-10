<!--
SPDX-FileCopyrightText: 2025 Benoît Rolandeau <benoit.rolandeau@allcircuits.com>

SPDX-License-Identifier: MIT
-->

# Mobile application

## Table of contents <!-- omit from toc -->

- [Mobile application](#mobile-application)
  - [Presentation](#presentation)
  - [Needs](#needs)
    - [MUST have](#must-have)
    - [SHOULD have](#should-have)
    - [COULD have](#could-have)

## Presentation

This file contains **WHAT** your customer expects from the mobile application.

## Needs

### MUST have

- `NMA1`: the user must be able to see the list of its things.
- `NMA2`: the user must be able to filter the list of its things depending of their types.
- `NMA3`: the user must be able to see its things on a dedicated page.
- `NMA4`: the user must be able to see the `client` attributes from its things, without the
  ability to modify them.
- `NMA5`: the user must be able to see the `server` attributes from its things, with the ability
  to modify them.
- `NMA6`: the user must be able to see the telemetry data from its things.
- `NMA7`: the user must be able to set the refresh rate of the data displayed.
- `NMA8`: the user must be able to see the history of one telemetry element.
- `NMA9`: the user must be able to see its app in English or in French, depending of the
  language of the phone. If the language is not English or French, the app must be in English.
- `NMA10`: the user must be able to change its app in light or dark mode.
- `NMA11`: the user must be able to see the logo of the company as the app icon.
- `NMA12`: the user must be able to see the temperature of its temperature sensor in Celsius or
  Fahrenheit.
- `NMA13`: The user must be able to change the temperature unit in the settings of the app. This
  unit is saved as a `server` attribute of the temperature sensor.

### SHOULD have

- `NMA+1`: the user should be able to see the telemetry data in a graph.
- `NMA+3`: the user should be able to connect to the server by WebSocket. The user should be able to
  see the telemetry data in real-time.

### COULD have

- `NMA++1`: the user could be able to connect to the server with a login and a password. This
  implies to create a page to sign-up and sign-in to the server. The other pages must be only
  accessible if the user is connected.
- `NMA++2`: the user could be able to change its password and its login.
