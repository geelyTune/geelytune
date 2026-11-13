# Changelog

## 26-11-13.57

**Sensors**
- Fixed: “Range, forecast” no longer shows 0 with charge hold on

**Navigation**
- “Yandex Auto settings” are now called “Navigator settings”; the switches are “Remove 3D buildings” and “Remove 3D landmarks”

**Cameras**
- Reversing: “None” option — no reversing cameras, the front camera after reversing and on the button still works
- Fixed: on the instrument cluster, the turn camera no longer interrupts the front camera and the reversing cameras

**HUD**
- Front camera from a steering wheel button: the OK button switches between it and “Mirror cameras forward”, as after “R”; the chosen view is remembered
- Fixed: the HUD Speed window stays where its plate is in the layout and no longer shifts when cameras are shown
- Fixed: the speed next to the wide turn camera is cyan in “Snow mode”

**Instrument cluster**
- Fixed: “Автомобиль впереди начал движение” (“Vehicle ahead has started moving”) instead of the factory Russian text with a typo

**Controls**
- “Climate”: “Restore climate” — the climate, seat and steering wheel heating and ventilation, and window heating return to how they were left
- “Remote access”: an engine start by a security system (for example, StarLine) on a locked car is recognized at once; while the engine or climate it started is running, the power-off timer does not cut the warm-up
- “Remote access”: after the relay wakes the car, the status bar shows how many minutes are left until the car goes to sleep; the power-off timer counts from when the infotainment system started
- “Remote access”: climate now includes automatic heating of the driver and passenger seats and the seat and steering wheel heating time
- Fixed: “Remote access” — the screen no longer lights up on the locked vehicle when it switches off after a remote start
- Fixed: car wash mode no longer turns itself off if the car is on and locked from inside — for example, by itself when shifting to “D”

**Driver assistance**
- “Automatic emergency braking (AEB)” and “Forward collision warning (FCW)”; the choice is restored every time the car is switched on. As in the standard settings, AEB can only be turned off below 10 km/h

**Buttons**
- On firmware 2.2.0 and later — “Speed limiter”: holding any steering wheel button or a short press of the star button switches the cruise button between cruise control and the speed limiter
- On firmware 2.2.0 and later, a short press of the star button no longer offers the front camera and “Sport”: the standard button would also switch the speed limiter along with them

**Sound**
- “External speaker”: your voice through the speaker outside the car — for example, to warn a pedestrian. Talk by holding the button in the window or an assigned steering wheel button, or by tapping the status bar button (it turns off by itself after 30 seconds). The window also has volume with “Boost”, your own phrase up to 10 seconds, your own sound from a USB drive and a test with the “Space” melody. Volume needs the GeelyMediaBridge 26-11-12.5 system copy
- Volume of the speeding chime for the Navigator sign: “Quiet”, “Normal” or “Loud”; “Normal” is as loud as the assistant chime — the chime used to be half as loud
- “Amplifier restart” is now in Sound, as the last item; if the amplifier does not accept a restart, the window suggests opening the driver’s door
- “Experimental”: “Loudness” and, on hybrids, “Engine noise cancellation (EOC)” — hidden settings from the engineering menu
- Fixed: custom pedestrian warning sound on EX5 EV — plays forward and in reverse

**Status bar**
- “HDC” button: one tap turns hill descent control on or off; the button is orange while HDC is on

## 26-11-10.67

**Sensors**
- (EX5 EM-i) the car in the background takes the color from "Display" → "Vehicle color"

**Navigation**
- On firmware 2.2.0 GeelyTune works with the factory Yandex Navigator if Yandex Auto is not installed: the map on the HUD and instrument cluster, map settings; the Navigator icon in the app menu is "Yandex Maps"
- "Instrument cluster": the navigator for the cluster map — Yandex Auto or an Android Auto navigator (for example, Navitel)
- "Yandex Auto settings": without 3D buildings and landmarks the CPU load is about a quarter lower; "Don’t write navigation data to the log"; "No Yandex metrics" — up to 1.5 GB more free memory and faster startup

**Cameras**
- "Turn signals": "Show wide camera view" — on the HUD the camera takes half of the strip, with the speed next to it
- "Mirror cameras forward": after "R", the OK button on the steering wheel switches between the front camera and the mirror cameras aimed at the front wheels
- Fixed: on EX5 EV with early firmware the rear camera turns on in "R", the front one after reversing

**HUD**
- HUD Speed plate — size and transparency, warnings through the headrest speakers
- The magnet in the layout turns plate snapping on and off; while the map and route card are dragged, they move on the HUD right away
- Android Auto navigator map — maneuver hints and lanes, the route already driven
- Navigator speed limit sign has no fill
- Fixed: cameras, especially the side ones, are shown more smoothly
- Fixed: while the turn signal camera is at the side, speed limit signs and plates in the speed area are not shown
- Fixed: the outside temperature comes from the car sensor, no −1° after a restart
- Fixed (models with an engine): the petrol part of the range forecast was 2–2.5 times too low; fuel consumption "since last refuel" was too high — it is counted anew
- Fixed: without the permission to draw over other apps, a hint shows where to grant it
- Fixed: with driving assistants hidden, no piece of the lane line is left above the speed
- Fixed: the "Route" plate no longer jumps around

**HUD and instrument cluster**
- With the Navigator sign, "Allowed excess speed" and a speed limit warning: the sign flashes, with sound if selected
- Cameras fade in and out smoothly
- Fixed: the map is not drawn under the camera — lower load
- Fixed: the map shows the car position right away, even if the Navigator is not open

**Instrument cluster**
- Fixed: after parking, the add-ons come back by themselves when the car is switched on, without opening GeelyTune
- Fixed: the add-ons no longer stay off after "Service mode" if the instrument cluster did not respond when the mode was turned off
- Fixed: the turn signal camera appears right after the car wakes up
- Fixed: no black screen instead of the map when the Navigator is not running; the speed limit sign no longer starts an unloaded Navigator
- Fixed: for third-party players the track time keeps running after pauses and seeking, and the artwork appears right away
- Fixed: "Battery status" no longer shifts up; on EX5 EV the battery percentage is correct right after startup
- Fixed: on firmware 2.2.0 the RPM in place of the second speed no longer flickers while driving; there is no "Second speed" plate in "Layout" — this cluster version does not have it

**Battery**
- Fixed: on the hybrid the "Actual consumption" range forecast no longer overstates the electric range; the electric forecast goes down to 25% charge, as in the factory one
- Fixed: EX5 EV with firmware 253612 — the energy left in the battery and the range forecast are calculated from the charge level

**Controls**
- "Remote access": while the locked car is woken remotely (for example, by an installed device) — ADB over Wi-Fi, headlights and screens off, the selected climate on, power off after 5, 10, 20 or 30 minutes; everything returns when the car is disarmed
- "Connection": "USB port" — "Debugging" or "Storage", the selected mode is set at every start; the port is open for debugging from the first seconds of boot
- "Apps": remove and restore the built-in Spotify; on firmware 2.2.0 — turn the built-in Yandex Auto off and on
- "Safety": what failure protection does, and a switch for it
- "Reset to factory settings": everything GeelyTune has changed in the car and on the instrument cluster, each marked "Modified" or "Factory", and a "Reset" button
- Fixed: "Connection" → "ADB over Wi-Fi" — with a network selected, the port opens right after the car starts
- Fixed: during boot the USB port is in debugging mode right away — the computer sees the car over the cable from the first seconds

**Lights**
- Fixed: after turning the headlights off with a button, the approach light no longer goes off the moment the car unlocks; the central lock button in the cabin no longer changes the headlights while you are in the car

**Buttons**
- The "Screen saver" hold function
- Fixed: on firmware 2.2.0 a short press of the selector with "Drive mode" chosen opens the drive mode switch, not the wallpaper
- Fixed: steering wheel buttons switch tracks in the "Volny Zvuka" player

**Sound**
- "Virtual venue": studio, concert hall, opera, vocal concert
- "Headrest speakers": each profile has its own mode
- "Lock sound": "Standard" or "Custom" with volume, "Off"; on EX5 EM-r — through the external speaker instead of the horn
- Fixed: the factory "Virtual venue" screen no longer restarts car services

**Display**
- "Vehicle color": new green, closer to the real one; on EX5 EV — "White" on the instrument cluster

**Status bar**
- "Heated steering wheel" button
- "Headlights" outside "P" work like the steering wheel button: up to 20 km/h the headlights switch to position lights and back
- Fixed: screenshots report "Screenshot saved" or "Could not take a screenshot"; the "CPU" plate updates at least every 10 seconds; the GeelyTune icon opens GeelyTune

**Bottom bar**
- Fixed: the button in the fuel door position no longer disappears when the theme changes

**Update**
- A section of its own; "Components": the version of each part, "Reinstall", "Remove" and "Install" — including GeelyMediaBridge missing from the car and the factory Yandex Navigator on firmware 2.2.0
- Firmware 2.2.0: the factory Yandex Navigator, bottom bar and audio service missing from the car are downloaded from the update server — including after a factory reset
- Fixed: "Update available" names what will actually be updated; if GeelyMediaBridge cannot install an update, GeelyTune installs it itself; right after the car is switched on, it waits for the instrument cluster to boot
- Fixed: GeelyMediaBridge without system rights (after a firmware update or unlock) — a window with an "Install" button when GeelyTune opens; the media bridge installs into the system on firmware without a separate write layer too

**Maintenance**
- "Language" — Russian, English, Chinese, Thai
- "Grant missing permissions"; with some permissions missing, a window with a "Grant" button appears at start in "P"
- The bottom bar installs on EX5 EV with firmware 264133
- Fixed: "Save settings to USB drive" — shade tiles are saved too

**Other**
- Search in the app: pull the menu down from the very top
- Fixed: GeelyTune starts faster; occasionally, after the car was switched on, some functions did not start until a reboot
