Standard Operating Procedure (SOP)
Fort Lewis College
Senior Seminar 2024-2025

**Author:** Lincoln Scheer
**Updated:** April 20, 2025

---

## Adapted From

PSR Photolithography Unit Process SOP.

---

## Notes

This SOP outlines the photolithography unit process, providing a standardized procedure for wafer preparation, photoresist application, patterning, and development. The goal is to ensure process consistency, repeatability, and safety. This document is actively developed and refined; modifications may be made as improvements are identified. Users must refer to the Karl Suss MBJ3 Contact Aligner section under Equipment and Materials to familiarize themselves with the machine before operation.

## Safety
This SOP is intended and may be use by students at Fort Lewis College trained in the FLC Nano Lab. You must read and fully understand the Material Safety Data Sheets (MSDS) for all chemicals and materials used in this SOP. You must also be trained on the equipment and processes before attempting to use them. If you have any questions or concerns, please consult Dr. Jeff Jessing. This SOP uses BOE (Buffered Oxide Etch) and AZ® 910 Remover, which are hazardous materials. Always wear appropriate personal protective equipment (PPE), including gloves, goggles, and lab coats. **BOE Etch contains hydrofluoric acid (HF)**, which is highly corrosive and can cause severe burns. You must be **trained in the use of HF to Dr. Jeff Jessing's satisfaction** before using this SOP. Don't use this SOP when you are tired, distracted, or otherwise unfit to work safely.

---

## Table of Contents

1. [Unit Process Overview](#unit-process-overview)
2. [Quick Reference Tables](#quick-reference-tables)
3. [Unit Process SOP](#unit-process-sop)
4. [Mask Etch Procedures](#mask-1--2--3-etch-procedures)
   1. [Mask 1 - Active (Positive Tone)](#mask-1---active-positive-tone)
   2. [Mask 2 - Gate Ox (Negative Tone)](#mask-2---gate-ox-negative-tone)
   3. [Mask 3 - Contact Opening (Negative Tone)](#mask-3---contact-opening-negative-tone)
   4. [Mask 4 - Metal Etch (Positive Tone)](#mask-4---metal-etch-positive-tone)
5. [Equipment and Materials](#equipment-and-materials)
   1. [Karl Suss MBJ3 Contact Aligner](#karl-suss-mbj3-contact-aligner)
6. [Startup Procedures](#startup-procedures)
7. [Shutdown Procedures](#shutdown-procedures)
---

## Unit Process Overview

The standard photolithography workflow consists of these key steps:

1. **Wafer Cleaning** - Prepare substrate surface
2. **Spin Coating** - Apply photoresist uniformly
3. **Soft Bake** - Evaporate solvents and stabilize film
4. **Exposure** - Transfer mask pattern to photoresist
5. **Post-Exposure Bake** (for negative resists) - Stabilize exposed areas
6. **Development** - Remove unwanted photoresist
7. **Hard Bake** (for positive resists) - Increase adhesion
8. **Processing** - Etching oxide or metal
9. **Stripping** - Remove remaining photoresist

## Quick Reference Tables

### Photoresist Parameters


| Parameter            | AZ® 1512 (Positive)        | AZ® nLOF™ 2020 (Negative) |
| ---------------------- | ----------------------------- | ----------------------------- |
| Spin Speed (RPM)     | 3000                          | 3000                          |
| Spin Time (s)        | 30                            | 30                            |
| Accel (s)         | 3                             | 3                             |
| Decel (s)         | 0.5                           | 0.5                           |
| Soft Bake (°C)      | 110                           | 110                           |
| Soft Bake (s)       | 60                            | 60                            |
| Exposure (mJ/cm²)   | 120                           | 73                            |
| Post Exposure Bake (°C) | N/A                           | 110                           |
| Post Exposure Bake (s)  | N/A                           | 60                            |
| Developer Type    | AZ® 300 MIF                  | AZ® 300 MIF                  |
| Developer (s)       | 45                            | 60                            |
| Hard Bake (°C)      | 110                           | N/A                           |
| Hard Bake (s)       | 300                           | N/A                           |
| Strip Type        | AZ® 910 Remover              | AZ® 910 Remover
| Stripping (°C) | 50-60                         | 50-60                         |
| Stripping (m) | 15                            | 15                            |

### Mask Summary

| Mask | Purpose         | Photoresist      | Tone     | 
| ------ | ----------------- | ------------------ | ---------- |
| 1    | Active          | AZ® 1512        | Positive |
| 2    | Gate Ox         | AZ® nLOF™ 2020 | Negative |
| 3    | Contact Opening | AZ® nLOF™ 2020 | Negative |
| 4    | Metal Etch      | AZ® 1512        | Positive |

---

## Unit Process SOP

This standardized process can be used for all mask steps with appropriate parameters.

1. **Spin Coating**

   Recommended setup orientation for spin coating, soft bake, and hardbake.
   ![alt text](sops/image-4.png)

   Steps 3-6 are performed immediately in sequence, no break between steps.
   
   1. Startup spin coater and hot plate, clean the spin coater "dropper window" with acetone.

      `Temp: 110°C`

      `Spin Speed: 3000 RPM`

      `Spin Time: 30 s`

      `Acceleration: 3 s`

      `Deceleration: 0.5 s`
   3. Place wafer on spin coater chuck with tweezers.
   2. Center wafer on chuck with tweezers and chuck tool.
   3. Do a test spin to ensure the wafer is centered, if not, re-center and test again.
   3. Apply adhesion promoter (unless metal substrate, mask 4) to the center of the wafer

      `HMDS: 7 drops`
   4. Spin HMDS (unless metal substrate, mask 4)
   5. Apply photoresist to the center of the wafer

      `Amount: 1-2 mL (full dropper)`

      `Type (Mask 1, 4): AZ® 1512`

      `Type (Mask 2, 3): AZ® nLOF™ 2020`
   6. Spin photoresist
2. **Soft Bake**

   1. Transfer wafer to hot plate 

      `Temperature: 110°C`

      `Time: 60 s`
   2. Remove wafer and let cool to room temperature
   3. If not exposed immediately, wrap in foil and store in yellow nitrogen box
3. **Exposure**

   1. Measure UV intensity using light meter

      `Intensity: X mW/cm²`
   2. Calculate exposure time based on required dose

      `Formula: Exposure Time [s] = Required Dose [mJ/cm²] ÷ Measured Intensity [mW/cm²]`

      `Dose (AZ® 1512): 120 mJ/cm²`

      `Dose (AZ® nLOF™ 2020): 73 mJ/cm²`
   3. Unscrew mask holder from stage
   4. Slide mask holder from stage and place mask holder on cleanroom wipe.
   5. Place appropriate mask (brown/chrome side up) on mask holder.
   6. Press "Vacuum Mask" button to apply vacuum to the mask holder. Verify that the mask is held securely.
      **Note:** Do not let the mask's brown/chrome side contact any surface.
   7. Carefully slide the mask holder back into the stage and clamp it down using the knurled knobs. Again, do not let the mask's brown/chrome side contact any surface.
   8. Load wafer onto chuck, covering all vacuum holes, ensuring the wafer is not in contact with the chuck o-ring.
   9. Move the transport slide so that the wafer is under the mask.
      **Note:** The transport slide is labeled 32.
   10. Alignment and Exposure
       1. Rotate the contact lever 80% of the wafer just before contact. The contact indicator should NOT be lit.
       2. Using the microscope, align the mask and wafer using X-Y and theta micromanipulators.
       3. Once in "coarse" contact, put into "fine" contact by rotating the contact lever 180° counterclockwise. The contact indicator should light.
       4. Rotate the separation lever fully clockwise to separate the mask and wafer. The contact indicator should go out and the separation indicator should light.
       5. Use the microscope to align features at high magnification if needed.
       6. Return to contact and verify alignment at contact and no shifting. At this state, the contact indicator should be lit, the separation unlit.
       7. Press the "Vacuum Holder" button to apply vacuum to the wafer against the mask.
       8. Press the "HP | SP" button to switch to high-pressure contact. The red "HP" portion of the button should be lit.
       9. Set the exposure timer based on your calculation above.
       10. Press "EXPOSURE" (never look directly at the UV light).
   11. Move the contact lever back 180° clockwise to release the wafer from the mask. The contact indicator should go out.
   12. Pull the transport slide and remove the wafer from the chuck.
4. **Post Exposure Bake** (AZ® nLOF™ 2020 ONLY)

   1. Transfer to hot plate.

      `Temperature: 110°C`

      `Time: 60 s`
   2. Remove wafer and let cool to room temperature.

5. **Development**

   1. Prepare AZ® 300 MIF developer in a fume hood along with two beakers of DI water.
   2. Immerse wafer in AZ® 300 MIF for prescribed time 

      `Time (AZ® 1512): 45 s`
      
      `Time (AZ® nLOF™ 2020): 60 s`
   3. Rinse in DI water for 30 s in each of two beakers

      `First Rinse: 30 s`
      
      `Second Rinse: 30 s`
   4. Rinse under flowing DI water for 30 s
   5. Dry with nitrogen gun
   3. Inspect wafer for development completion, if undeveloped, repeat development process for 1-5s and inspect again.

      `Overdeveloped: Rounded Edges`
      
      `Properly Developed: Sharp Edges`
      
      `Undeveloped: Rainbow Residue`
6. **Hard Bake** (AZ® 1512 ONLY)

   1. Place wafer on hot plate at 110°C
   
      `Temperature: 110°C`
      
      `Time: 300 s (5 min)`
   2. Remove wafer and let cool to room temperature
7. **Etch Process**

   1. Perform required process according to specific mask step.
8. **Stripping**

   1. Heat AZ® 910 Remover to 50-60°C
   
      `Temperature: 50-60°C`
      
      `Time: 900 s (15 min)`
   2. Immerse wafer for 15 min (900 s)
   3. Rinse in DI water for 5 min (300 s)
   
      `DI Water Rinse: 300 s (5 min)`
   4. Perform solvent cleaning with acetone, IPA, and methanol
   5. Dry with nitrogen gun

---

## Mask (1 & 2 & 3) Etch Procedures

   1. **Prepare Etch Station**
      1. Notify HF process supervisor (Dr. Jessing) before starting the etch process.
      2. You must be trained in the use of HF to Dr. Jessing's satisfaction before using this SOP.
      3. You must have a trained buddy present during the etch process.
      4. Wear appropriate PPE: goggles, 2x pairs nitrile gloves, 1x pair shoulder-length gloves, lab coat, and face shield, shoe covers, and a fume hood.
      5. Ensure the fume hood is functioning properly and the sash is at the minimum height you can work with.
      6. Ensure you know the location of the nearest emergency shower and eyewash station.
      7. Ensure you know the location of the nearest calcium gluconate station and calcium gluconate gel.
      8. Ensure you know the location of the nearest HF neutralization kit.
      9. If 1-8 are new to you, please ask Dr. Jessing for a refresher before proceeding.
      10. Setup a PTFE BOE Etch amd BOE Quench beaker in the fume hood.
      11. Fill the BOE Etch beaker with BOE and the BOE Quench beaker with DI water.

### Mask 1 - Active (Positive Tone)

1. **Prepare BOE Etch**
2. **Prepare BOE Quench**
3. **Prepare DI Water Rinse**
4. **Etch** 
   Dip the wafer in the BOE etch. Every 30s check the etch progress by lifting it out of the bath and watching weather the lapped surface appears hydrophobic or hydrophilic. The lapped surface should appear hydrophobic when the etch is complete. Then record this time and etch the wafer for an additional 20% of that time. This time is approximately 17mins for a 11000Å oxide layer of DWD.
5. **Quench**
   Dip the wafer in the BOE Quench for 30s.
6. **Rinse**
   Rinse the wafer in DI water for 1 minute.
7. **Dry**
   Dry the wafer with a nitrogen gun.

### Mask 2 - Gate Ox (Negative Tone)

1. **Prepare BOE Etch**
2. **Prepare BOE Quench**
3. **Prepare DI Water Rinse**
4. **Measure FOX Thickness**
   Measure the thickness of the FOX layer using the SEM, it is etched from the SOD removal process. Use the etch rate calculated from the previous etch to determine the etch time required to remove the remaining FOX layer. The etch time is 20% longer than calculated if above 4000Å, or 15% longer if below 4000Å.
5. **Etch**
      Dip the wafer in the BOE etch. Etch for the calculated time in step 4.
6. **Quench**
   Dip the wafer in the BOE Quench for 30s.
7. **Rinse**
   Rinse the wafer in DI water for 1 minute.
8. **Dry**
   Dry the wafer with a nitrogen gun.

### Mask 3 - Contact Opening (Negative Tone)

1. **Prepare BOE Etch**
2. **Prepare BOE Quench**
3. **Prepare DI Water Rinse**
4. **Measure FOX Thickness**
   Measure the thickness of the GOX layer, we need to etch through the GOX layer to create the contact opening. Use the etch rate calculated from the previous etch to determine the etch time required to remove the remaining GOX layer, use a 10% over etch time.
5. **Etch**
      Dip the wafer in the BOE etch. Etch for the calculated time in step 4.
6. **Quench**
   Dip the wafer in the BOE Quench for 30s.
7. **Rinse**
   Rinse the wafer in DI water for 1 minute.
8. **Dry**
   Dry the wafer with a nitrogen gun.

### Mask 4 - Metal Etch (Positive Tone)

   **REFER TO THE METAL DEPOSITION ETCH SOP**

---

## Equipment and Materials

### Equipment

- Karl Suss Contact Aligner.
- Spin Coater.
- Hot Plate.
- Oven.
- Fume Hood.
- Wafer Holder.

### Materials

- **Adhesion Promoter**
  - Hexamethyldisilane (HMDS).
- **Photoresist**
  - `AZ® 1512` Photoresist (Positive Tone).
  - `AZ® nLOF™ 2020` Photoresist (Negative Tone).
- **Developer**
  - `AZ® 300 MIF`.
- **Stripper**
  - `AZ® 910 Remover`.
  - `AZ® NMP Rinse`.
  - `AZ® KWIK Strip`.
- **Solvent / Cleaning**
  - Acetone.
  - Isopropanol (IPA).
  - Methanol.
  - DI Water.
- **Support & Process Gasses**
  - UHP Nitrogen.
  - Compressed Air.

  ### Karl Suss MBJ3 Contact Aligner

   The Karl Suss MBJ3 Contact Aligner is a contact photolithography tool used for aligning and exposing photoresist-coated wafers. It utilizes a UV light source to transfer patterns from masks to substrates.

   ![MJB Contact Aligner](sops/image-1.png)

   1. Lamp Power Supply
   2. Manometer
   3. Karl Suss Aligner
   4. UV Light Meter
   5. Wafer Slide
   6. Mask Holder
   7. Contact Lever
   8. Separation Lever
   9. Theta-Axis Micromanipulator
   10. Y-Axis Micromanipulator
   11. X-Axis Micromanipulator
   12. Light Source
   13. Microscope

   ### Hot Plate
   USe the thermo scientific hot plate for soft bake and hard bake steps. This hot plate is more accurate than the others in the lab.

   ![alt text](sops/image-2.png)

---

## Startup Procedures

### Contact Aligner Startup

1. Turn on Nitrogen in the chase.
2. Switch on the power strip below the Karl Suss.
3. Press the "Power" button on the Karl Suss.
4. Flip the manometer switch up.
5. Turn on the lamp power supply.
6. Press "START" after system self-checks.
7. Wait for "Cold Fire" to complete.
8. Wait 1–5 hours for lamp stabilization.
9. Measure lamp intensity using a UV light meter.

### Spin Coater Startup

1. Place the spin coater inside the fume hood.
2. Power on the pump using the power strip.
3. Open the nitrogen line to purge excess air.
4. Increase nitrogen pressure to 50 psi to turn on the screen.

---

## Shutdown Procedures

### Contact Aligner Shutdown

1. Turn off the Nitrogen Lamp Power Supply.
2. Wait 45–60 minutes for lamp cooldown.
3. Turn off the manometer.
4. Press "Power" on the Karl Suss.
5. Turn off the power strip below the Karl Suss.
6. Turn off Nitrogen in the chase.

### Spin Coater Shutdown

1. Close the nitrogen line.
2. Power off the spin coater and pump.
3. Clean the spin coater bowl and chuck using acetone and IPA.
4. Store the spin coater if necessary.
