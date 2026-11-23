# Tiger Moth CIX Mod (MSFS)

This is a mod to [Ant's Tiger Moth for MSFS](https://www.antsairplanes.com/msfstigermoth.html) to make some tweaks for CIX VFR Club:

- Pilot weight: 77 kg
- Passenger weight: 0 kg
- Fuel: 70%
- CIX Tigers liveries
- Weather presets
- Aerobatic smoke (red/white/blue)

The aerobatic smoke is based on (and should be used with) v1.4.1 of Ant's Tiger Moth.

This mod now includes the aerobatic smoke that used to be a separate add-on (Tiger Moth Aerobatic Smoke). If you have that installed, remove it before installing this one.

## Liveries

The CIX Tigers liveries are existing liveries with "Tiger" and the Tiger number added to both sides of the fuselage. Liveries flown by a regular club member also show that pilot's name and flag.

Livery  | Aircraft | Based on                                                                                        | Pilot                | Changes for CIX VFR Club
--------|----------|-------------------------------------------------------------------------------------------------|----------------------|---------------------------------------------------------------------------------------
TIGER-0 | ZK-BRC   | Ant's Airplanes (included with Ant's Tiger Moth)                                                |                      | "Tiger" and number added
TIGER-1 | A17-692  | Ant's Airplanes (included with Ant's Tiger Moth)                                                |                      | "Tiger" and number added
TIGER-2 | G-ANOD   | Jankees: [G-ANOD repaint](https://flightsim.to/file/51232/de-havilland-dh-82-tiger-moth-g-anod) |                      | "Tiger" and number added
TIGER-3 | T-6953   | Ant's Airplanes (included with Ant's Tiger Moth)                                                | Dave (UK)            | "Tiger", number, pilot name and flag added
TIGER-4 | A17-736  | Ant's Airplanes (included with Ant's Tiger Moth)                                                | Cristian (Romania)   | "Tiger", number, pilot name and flag added
TIGER-5 | N-6635   | Ant's Airplanes (included with Ant's Tiger Moth)                                                |                      | "Tiger" and number added
TIGER-6 | K-4259   | Ant's Airplanes (included with Ant's Tiger Moth)                                                | Tudux (Switzerland)  | "Tiger", number, pilot name and flag added; yellow bands on fuselage and wings changed to red
TIGER-7 | HB-UPM   | Jankees: [HB-UPM repaint](https://flightsim.to/file/41488/de-havilland-dh-82-tiger-moth-hb-upm) | John (UK)            | "Tiger", number, pilot name and flag added
TIGER-8 | VH-BVB   | Ant's Airplanes (included with Ant's Tiger Moth)                                                | Wentian (Australia)  | "Tiger", number, pilot name and flag added
TIGER-9 | A17-518  | Ant's Airplanes (included with Ant's Tiger Moth)                                                | Paul (UK)            | "Tiger", number, pilot name and flag added

Thanks to Ant's Airplanes for the aircraft and its original liveries, and to Jan Kees Blom (Jankees) for the G-ANOD and HB-UPM repaints.

Each livery has its own default setup of exterior details. These are applied every time the aircraft is loaded. You can change them for the current flight on the aircraft's tablet, and the tablet's reset button goes back to the livery's defaults.

All liveries share the following. The "Tablet setting" and "Default" columns use the names and values shown on the tablet's Exterior Preferences page:

Option                                              | Tablet setting         | Default
----------------------------------------------------|------------------------|----------------
Brass leading edge of propeller                     | Propeller edge         | On
Inner wheel covers                                  | Wheel cover inner      | Off
Outer wheel covers                                  | Wheel cover outer      | On
Small covers at the base of the struts and fuselage | *(not on the tablet)*  | Shown
Tail gear                                           | Tail gear              | Skid
Air intake                                          | Air intake             | Vintage
Oil tank                                            | Oil tank               | Straps
Windy airspeed gauge on left wing strut             | Windy Airspeed gauge   | Show
Prop spinner                                        | Propeller spinner      | On

The remaining details differ between liveries (tablet settings **Venturi** and **Pitot type**):

Livery  | Venturi    | Pitot type
--------|------------|-----------
TIGER-0 | Australian | Australian
TIGER-1 | English    | English
TIGER-2 | English    | English
TIGER-3 | English    | English
TIGER-4 | English    | English
TIGER-5 | English    | English
TIGER-6 | English    | English
TIGER-7 | Australian | English
TIGER-8 | Australian | Australian
TIGER-9 | Australian | Australian

The Australian venturi sits higher up on the right strut; the English one is lower down on the fuselage, mirroring the left side. The Australian pitot is straight; the English one bends down.

<details>
<summary>How the defaults are set</summary>

The defaults are stored as the last 11 characters of the `Title` in each livery's `aircraft.cfg`, for example `Title="Tiger Moth TIGER-0 01001100000"`. From left to right:

Position | Option                                              | Tablet setting        | 0                                     | 1
:-------:|-----------------------------------------------------|-----------------------|---------------------------------------|---------------------------------
1        | Brass leading edge of propeller                     | Propeller edge        | show                                  | hide
2        | Inner wheel covers                                  | Wheel cover inner     | show                                  | hide
3        | Outer wheel covers                                  | Wheel cover outer     | show                                  | hide
4        | Small covers at the base of the struts and fuselage | *(not on the tablet)* | show                                  | hide
5        | Tail gear                                           | Tail gear             | wheel                                 | skid
6        | Air intake                                          | Air intake            | modern (tear drop shaped)             | vintage (round)
7        | Oil tank                                            | Oil tank              | straps                                | no straps
8        | Venturi                                             | Venturi               | Australian (higher up on right strut) | English (lower down on fuselage)
9        | Pitot type                                          | Pitot type            | Australian (straight)                 | English (bends down)
10       | Windy airspeed gauge on left wing strut             | Windy Airspeed gauge  | show                                  | hide
11       | Prop spinner                                        | Propeller spinner     | show                                  | hide

</details>

## Aerobatic Smoke

Coloured display smoke (red/white/blue) can be set using the following controls (choose whatever key/joystick combinations as appropriate):

Effect                                 | Control Name               | Suggested Binding
---------------------------------------|----------------------------|-------------------------------------------
Toggle White Smoke (MSFS 2020/2024)    | `Smoke Toggle`             | <kbd>i</kbd>
Toggle White Smoke  (MSFS 2020 only *) | `Toggle Windshield Deice`  | <kbd>i</kbd>
Toggle Blue Smoke                      | `Toggle Engine 1 Anti Ice` | <kbd><kbd>Shift</kbd> + <kbd>i</kbd></kbd>
Toggle Red Smoke                       | `Toggle Plasma`            | <kbd><kbd>Ctrl</kbd> + <kbd>i</kbd></kbd>
Toggle Smoke Intensity                 | `Toggle G Limiter`         | <kbd><kbd>Alt</kbd> + <kbd>i</kbd></kbd>

(*) White smoke used to be controlled by `Toggle Windshield Deice`, but this didn't work in MSFS 2024 so has been changed to `Smoke Toggle`. For compatibility, `Toggle Windshield Deice` will continue to work in MSFS 2020 for the time being, but it should be considered deprecated and may be removed in a future version. Please update your mappings to use `Smoke Toggle` instead.

The smoke has two intensity levels. The default is "more intense". It can be switched to "less intense" with `Toggle G Limiter`.
