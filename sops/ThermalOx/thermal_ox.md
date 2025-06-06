Standard Operating Procedure (SOP)  
Fort Lewis College  
Senior Seminar 2024-2025

**Author:** Natalia Lambos  
**Updated:** June 5, 2025

# Tube Furnace Oxidation Process Guide

---

### ⚠️ Safety Notice
- **Do not stand directly in front of the furnace during the process.**

---
## Unit Process SOP
1. **Preparation**

- Verify UHP oxygen and nitrogen tanks are full (>700 psi).
- Clean quartz boat with acetone, propanol, and methanol in the fume hood.
- Clean tube furnace and thermocouple with propanol using cleanroom wipes.
- Do not move the back thermal block.
- Place **Warning Furnace Sign** on Velcro at door.

2. **Wafer Loading**

- Load wafers into quartz boat, centered, regardless of count.
- Shiny side of wafers should face gas input (away from boat handle).
- Use **2 dummy wafers** to sandwich actual wafers, all facing shiny side toward gas input.
- Refer to Figure 1.

![Figure 1: Wafer orientation](sops/ThermalOx/Images/1.jpg)
3. **Boat Insertion**

- Insert quartz boat so wafers line up with furnace door latch (see _Figure 2.7_).
- Align thermal blocks with furnace insulation (see _Figure 2.8_).
- Slide the thermocouple through the metal blocks to ensure that it clears the wafers and does not hit them. 
- Close the lid on the furnace *SLOWLY*. If not, it can crush the tube. Secure latch. Put the metal grid from the oven on top of the furnace in preparation for the thermocouple.
- Put on metal cap cover and screw in on end of tube. 
image5.jpg, Picture, Picture

4. **Furnace Controller Setup**

- Turn **Main Power** switch to ON.
- Press button to display `C01` (current setting).
- Use directional buttons to adjust digits and set heating curve (see _Figure 2.9_).
- On oxidation day, after soaking, change `t06` from 400 to 1 to begin cooldown.


## Bubbler Setup

1. Go to outside closet and open UHP N2 and O2.
2. Dump out old water from bubbler, clean with Kimwipes.
3. Fill with **400 mL DI water** (~2/3 full).
4. Ensure all bubbler valves are **closed**:
   - Bypass (green)
   - Inlet (white)
   - Outlet (blue) — see _Figure 2.10_.
5. Confirm **butterfly valve** from bubbler to furnace is open (see _Figure 2.11_).

---

## Furnace Heating

1. Turn furnace Main Power ON.
2. Verify heating curve: `T06 = 1150°C` for DWD oxidation.
3. Set mass flow rates to **20 SCCM** for both N₂ and O₂.
4. Open nitrogen needle valve (2 turns counterclockwise).
5. Turn **N₂ butterfly valve** to ON.
6. Start run:
   - Hold controller button until “run” displays.
   - Hold green power button 2 seconds — red light should blink.

---

## Bubbler Heating (1 hr 45 min into ramp)

1. Tighten bubbler lid.
2. Turn ON bubbler power (under table).
3. Set to **102°C**, press and hold down arrow until it says “run”.

---

## Verify Furnace Temperature

1. After 2.5 hrs, plug thermocouple into **Omega Calibrator** (see _Figure 2.12_).
2. Use **high-temp gloves**.
3. Insert thermocouple until **scratches line up** with metal lid edge.
4. Wait 3 mins. Thermocouple will glow red.
5. Carefully remove and place on **metal grid**.

---

## Dry Oxidation Phase (45 min)

1. Open **O₂ needle valve** (2 turns counterclockwise).
2. Turn ON dry O₂ butterfly valve.
3. Turn OFF N₂ butterfly valve and close N₂ needle valve.
4. Set timer: **45 minutes**.

---

## Wet Oxidation Phase (2 hrs)

1. Confirm bubbler pressure ≥ **0.085 MPa**.
2. Open **bubbler bypass valve** (counterclockwise).
3. Open **bubbler outlet valve**.
4. Slowly turn ON **wet ox butterfly valve**.
5. Turn OFF **dry ox valve**.
6. Close **bubbler bypass**.
7. Slowly open **bubbler inlet**.
   - Water droplets in tube are **normal**.
8. Set timer: **120 minutes**.

---

## Post-Wet Oxidation (Cooldown Prep)

1. After 2 hrs:
   - Close bubbler **outlet** and **inlet** valves.
   - Open **dry ox butterfly valve**.
   - Close **wet ox valve**.
   - Turn OFF bubbler (power switch under table).
2. Set timer: **45 minutes**.

---

## Cooldown

1. After 45 min, set `t06 = 1` minute.
2. Reopen **N₂ needle valve** and turn ON **N₂ butterfly valve**.
3. Turn OFF **dry O₂ valve** and close O₂ needle valve.
4. Go outside and turn OFF **UHP O₂**.
5. Set timer: **3.5 hrs** for cooldown.

---

## End of Run

- When furnace <400°C, turn off Main Power.
- Close N₂ needle valve and butterfly valve.
- Turn OFF UHP nitrogen tank.

---

## Next Day Procedure

1. Remove wafers; place in individual wafer carriers **shiny side down**.
2. Cleave one wafer and measure oxide thickness via **SEM**.
3. Take remaining wafers to **Berndt Hall lab** for ellipsometry.
   - Follow procedure under “Ellipsometry Measurements”.

---
