Standard Operating Procedure (SOP)
Fort Lewis College
Senior Seminar 2024-2025

**Author:** Lincoln Scheer
**Updated:** April 15, 2025

---

## Adapted From

PSR Photolithography Unit Process SOP.

---

## Notes

This SOP outlines the photolithography unit process, providing a standardized procedure for wafer preparation, photoresist application, patterning, and development. The goal is to ensure process consistency, repeatability, and safety. This document is actively developed and refined; modifications may be made as improvements are identified.

---

## Table of Contents

1. [Photolithography Process Overview](#photolithography-process-overview)
2. [Quick Reference Parameters](#quick-reference-parameters)
3. [Generic Photolithography Process Flow](#generic-photolithography-process-flow)
4. [Mask Procedures](#mask-procedures)
   1. [Mask 1 - Active (Positive Tone)](#mask-1---active-positive-tone)
   2. [Mask 2 - Gate Ox (Negative Tone)](#mask-2---gate-ox-negative-tone)
   3. [Mask 3 - Contact Opening (Negative Tone)](#mask-3---contact-opening-negative-tone)
   4. [Mask 4 - Metal Etch (Positive Tone)](#mask-4---metal-etch-positive-tone)
5. [Equipment and Materials](#equipment-and-materials)
6. [Startup Procedures](#startup-procedures)
7. [Shutdown Procedures](#shutdown-procedures)
8. [Detailed Process Steps](#detailed-process-steps)
   1. [Spin Coating &amp; Soft Bake](#spin-coating--soft-bake)
   2. [Patterning](#patterning)
   3. [Development](#development)
   4. [Hard Bake](#hard-bake)
   5. [Stripping](#stripping)
9. [Process Documentation](#process-documentation)
10. [Appendices](#appendices)
    1. [Appendix A: Process Parameter Tables](#appendix-a-process-parameter-tables)
    2. [Appendix B: Process Logbook Template](#appendix-b-process-logbook-template)

---

## Photolithography Process Overview

The standard photolithography workflow consists of these key steps:

1. **Wafer Cleaning** - Prepare substrate surface
2. **Spin Coating** - Apply photoresist uniformly
3. **Soft Bake** - Evaporate solvents and stabilize film
4. **Exposure** - Transfer mask pattern to photoresist
5. **Post-Exposure Bake** (for negative resists) - Stabilize exposed areas
6. **Development** - Remove unwanted photoresist
7. **Hard Bake** (when needed) - Increase chemical resistance
8. **Processing** - Etching, implantation, etc.
9. **Stripping** - Remove remaining photoresist

---

## Quick Reference Parameters

### Photoresist Parameters Table

| Parameter            | AZ® 1512 (Positive)            | AZ® nLOF™ 2020 (Negative) |
| -------------------- | ------------------------------- | --------------------------- |
| Spin Speed           | 3000 RPM for 30 s (0.5 min)     | 3000 RPM for 30 s (0.5 min) |
| Soft Bake            | 110°C for 60 s (1.0 min)       | 110°C for 60 s (1.0 min)   |
| Exposure Dose        | 90–150 mJ/cm²                 | 66–80 mJ/cm²              |
| Post Exposure Bake   | N/A                             | 110°C for 60 s (1.0 min)   |
| Developer            | AZ® 300 MIF                    | AZ® 300 MIF                |
| Development Time     | 45 s (0.75 min)                 | 60 s (1.0 min)              |
| Hard Bake            | 110°C for 5 min (300 s)        | Not typically required      |
| Stripping Solution   | AZ® 910 Remover                | AZ® 910 Remover            |
| Stripping Conditions | 50-60°C for 15 min (900 s)     | 50-60°C for 15 min (900 s) |

### Mask Parameters Summary

| Mask | Purpose         | Photoresist      | Tone     | Unique Processing Notes                   |
| ---- | --------------- | ---------------- | -------- | ----------------------------------------- |
| 1    | Active          | AZ® 1512        | Positive | BOE etch, hard bake required              |
| 2    | Gate Ox         | AZ® nLOF™ 2020 | Negative | Post exposure bake, SOD removal           |
| 3    | Contact Opening | AZ® nLOF™ 2020 | Negative | Post exposure bake, contact opening       |
| 4    | Metal Etch      | AZ® 1512        | Positive | Hard bake required, follow metal etch SOP |

### Example Exposure Calculation

Using a measured intensity of 6.7 mW/cm²:

**For AZ® 1512 (Target: 120 mJ/cm²):**

- Exposure Time = 120 mJ/cm² ÷ 6.7 mW/cm² = 17.9 seconds

**For AZ® nLOF™ 2020 (Target: 73 mJ/cm²):**

- Exposure Time = 73 mJ/cm² ÷ 6.7 mW/cm² = 10.9 seconds

---

## Generic Photolithography Process Flow

This standardized process can be used for all mask steps with appropriate parameters.

1. **Wafer Preparation**

   1. Clean wafers with acetone, IPA, and methanol
   2. Dry with nitrogen gun
   3. **CHECKPOINT**: Surface should be clean, free of particulates and fingerprints
2. **Spin Coating**

   1. Program spin coater (3000 RPM, 30 s, 3 s accel, 0.5 s decel)
   2. Center wafer on chuck and verify proper vacuum
   3. Apply adhesion promoter (7 drops HMDS) if needed
   4. Spin HMDS
   5. Apply photoresist (full dropper, approximately 1-2 mL)
   6. Run spin program
   7. **CHECKPOINT**: Coating should be uniform with no streaks or comets
3. **Soft Bake**

   1. Transfer wafer to hot plate set to 110°C
   2. Bake for 60 s (1.0 min)
   3. Allow wafer to cool to room temperature
   4. **CHECKPOINT**: Surface should appear uniform with no bubbles
4. **Exposure**

   1. Measure UV intensity using light meter
   2. Calculate exposure time based on required dose
   3. Load appropriate mask (brown/chrome side up)
   4. Load substrate onto chuck
   5. Use microscope to align features if needed
   6. Bring into contact and expose for calculated time
   7. **CHECKPOINT**: No apparent light leakage during exposure
5. **Post Exposure Bake** (for negative resist only)

   1. Transfer to hot plate set to 110°C
   2. Bake for 60 s (1.0 min)
   3. Allow wafer to cool to room temperature
   4. **CHECKPOINT**: No visible defects
6. **Development**

   1. Prepare appropriate developer solution
   2. Immerse wafer in developer for specified time
   3. Rinse thoroughly with DI water (30 s in each of two beakers)
   4. Final rinse under flowing DI water
   5. Dry with nitrogen gun
   6. **CHECKPOINT**: Pattern is clearly visible and properly defined
7. **Hard Bake** (if required)

   1. Place wafer in oven at 110°C
   2. Bake for prescribed time (typically 5 min/300 s for AZ® 1512)
   3. Allow wafer to cool
   4. **CHECKPOINT**: No visible defects or cracking in resist
8. **Process** (etch, implant, etc.)

   1. Perform required process according to specific SOP
   2. **CHECKPOINT**: Process completed as expected
9. **Stripping**

   1. Heat AZ® 910 Remover to 50-60°C
   2. Immerse wafer for 15 min (900 s)
   3. Rinse in DI water for 5 min (300 s)
   4. Perform solvent cleaning with acetone, IPA, and methanol
   5. Dry with nitrogen gun
   6. **CHECKPOINT**: All photoresist removed, surface clean

---

## Mask Procedures

### Mask 1 - Active (Positive Tone)

**Purpose**: Define active regions for device fabrication

**Process Parameters**:

- Photoresist: AZ® 1512 (Positive)
- Spin Speed: 3000 RPM for 30 s (0.5 min)
- Soft Bake: 110°C for 60 s (1.0 min)
- Exposure: 120 mJ/cm² (17.9 s at 6.7 mW/cm²)
- Developer: AZ® 300 MIF for 45 s (0.75 min)
- Hard Bake: 110°C for 5 min (300 s)

1. **Wafer Preparation**

   1. Clean wafers with acetone, IPA, and methanol
   2. Dry with nitrogen gun
   3. **CHECKPOINT**: Surface should be clean, free of particulates
2. **Spin Coating**

   1. Program spin coater (3000 RPM, 30 s, 3 s accel, 0.5 s decel)
   2. Center wafer on chuck
   3. Apply 7 drops of HMDS
   4. Spin HMDS
   5. Apply full dropper of AZ® 1512
   6. Run spin program
   7. **CHECKPOINT**: Coating should be uniform
3. **Soft Bake**

   1. Transfer wafer to hot plate at 110°C
   2. Bake for 60 s (1.0 min)
   3. Allow wafer to cool
   4. **CHECKPOINT**: Surface should appear uniform
4. **Exposure**

   1. Measure UV intensity
   2. Calculate exposure time (120 mJ/cm² ÷ measured intensity)
   3. Load Mask 1 (brown/chrome side up)
   4. Load substrate onto chuck
   5. Expose for calculated time
   6. **CHECKPOINT**: Exposure completed successfully
5. **Development**

   1. Immerse wafer in AZ® 300 MIF for 45 s (0.75 min)
   2. Rinse in DI water for 30 s (0.5 min) in each of two beakers
   3. Final rinse under flowing DI water
   4. Dry with nitrogen gun
   5. **CHECKPOINT**: Pattern is clearly visible
6. **Hard Bake**

   1. Place wafer in oven at 110°C
   2. Bake for 5 min (300 s)
   3. Allow wafer to cool
   4. **CHECKPOINT**: No visible defects
7. **BOE Etch**

   1. Position wafers in boat with the lapped side facing away from the handle
   2. Etch for approximately 15 min (900 s) until complete oxide sheeting
   3. Calculate 20% overetch time based on oxide thickness
   4. Rinse in DI water for 30 s (0.5 min)
   5. Final rinse under flowing DI water
   6. **CHECKPOINT**: Oxide fully removed from active areas
8. **Drying**

   1. Dry with nitrogen gun
   2. **CHECKPOINT**: Surface is dry and clean
9. **Stripping**

   1. Heat AZ® 910 Remover to 50-60°C
   2. Immerse wafer for 15 min (900 s)
   3. Perform solvent cleaning with acetone, IPA, and methanol
   4. Dry with nitrogen gun
   5. **CHECKPOINT**: All photoresist removed

### Mask 2 - Gate Ox (Negative Tone)

**Purpose**: Define gate oxide regions

**Process Parameters**:

- Photoresist: AZ® nLOF™ 2020 (Negative)
- Spin Speed: 3000 RPM for 30 s (0.5 min)
- Soft Bake: 110°C for 60 s (1.0 min)
- Exposure: 73 mJ/cm² (10.9 s at 6.7 mW/cm²)
- Post Exposure Bake: 110°C for 60 s (1.0 min)
- Developer: AZ® 300 MIF for 60 s (1.0 min)

1. **Wafer Preparation**

   1. Clean wafers with acetone, IPA, and methanol
   2. Dry with nitrogen gun
   3. **CHECKPOINT**: Surface should be clean
2. **Spin Coating**

   1. Program spin coater (3000 RPM, 30 s, 3 s accel, 0.5 s decel)
   2. Center wafer on chuck
   3. Apply 7 drops of HMDS
   4. Spin HMDS
   5. Apply full dropper of AZ® nLOF™ 2020
   6. Run spin program
   7. **CHECKPOINT**: Coating should be uniform
3. **Soft Bake**

   1. Transfer wafer to hot plate at 110°C
   2. Bake for 60 s (1.0 min)
   3. Allow wafer to cool
   4. **CHECKPOINT**: Surface should appear uniform
4. **Exposure**

   1. Measure UV intensity
   2. Calculate exposure time (73 mJ/cm² ÷ measured intensity)
   3. Load Mask 2 (brown/chrome side up)
   4. Load substrate onto chuck
   5. Expose for calculated time
   6. **CHECKPOINT**: Exposure completed successfully
5. **Post Exposure Bake**

   1. Transfer to hot plate at 110°C
   2. Bake for 60 s (1.0 min)
   3. Allow wafer to cool
   4. **CHECKPOINT**: No visible defects
6. **Development**

   1. Immerse wafer in AZ® 300 MIF for 60 s (1.0 min)
   2. Rinse in DI water for 30 s (0.5 min) in each of two beakers
   3. Final rinse under flowing DI water
   4. Dry with nitrogen gun
   5. **CHECKPOINT**: Pattern is clearly visible
7. **BOE Etch**

   1. Follow SOD Removal SOP for BOE etch
   2. **CHECKPOINT**: Etching completed successfully
8. **Stripping**

   1. Heat AZ® 910 Remover to 50-60°C
   2. Immerse wafer for 15 min (900 s)
   3. Perform solvent cleaning with acetone, IPA, and methanol
   4. Dry with nitrogen gun
   5. **CHECKPOINT**: All photoresist removed

### Mask 3 - Contact Opening (Negative Tone)

**Purpose**: Create contact openings for metallization

**Process Parameters**:

- Photoresist: AZ® nLOF™ 2020 (Negative)
- Spin Speed: 3000 RPM for 30 s (0.5 min)
- Soft Bake: 110°C for 60 s (1.0 min)
- Exposure: 73 mJ/cm² (10.9 s at 6.7 mW/cm²)
- Post Exposure Bake: 110°C for 60 s (1.0 min)
- Developer: AZ® 300 MIF for 60 s (1.0 min)

1. **Wafer Preparation**

   1. Clean wafers with acetone, IPA, and methanol
   2. Dry with nitrogen gun
   3. **CHECKPOINT**: Surface should be clean
2. **Spin Coating**

   1. Program spin coater (3000 RPM, 30 s, 3 s accel, 0.5 s decel)
   2. Center wafer on chuck
   3. Apply 7 drops of HMDS
   4. Spin HMDS
   5. Apply full dropper of AZ® nLOF™ 2020
   6. Run spin program
   7. **CHECKPOINT**: Coating should be uniform
3. **Soft Bake**

   1. Transfer wafer to hot plate at 110°C
   2. Bake for 60 s (1.0 min)
   3. Allow wafer to cool
   4. **CHECKPOINT**: Surface should appear uniform
4. **Exposure**

   1. Measure UV intensity
   2. Calculate exposure time (73 mJ/cm² ÷ measured intensity)
   3. Load Mask 3 (brown/chrome side up)
   4. Load substrate onto chuck
   5. Expose for calculated time
   6. **CHECKPOINT**: Exposure completed successfully
5. **Post Exposure Bake**

   1. Transfer to hot plate at 110°C
   2. Bake for 60 s (1.0 min)
   3. Allow wafer to cool
   4. **CHECKPOINT**: No visible defects
6. **Development**

   1. Immerse wafer in AZ® 300 MIF for 60 s (1.0 min)
   2. Rinse in DI water for 30 s (0.5 min) in each of two beakers
   3. Final rinse under flowing DI water
   4. Dry with nitrogen gun
   5. **CHECKPOINT**: Pattern is clearly visible
7. **BOE Etch**

   1. Follow Contact Opening SOP for BOE etch
   2. **CHECKPOINT**: Etching completed successfully
8. **Stripping**

   1. Heat AZ® 910 Remover to 50-60°C
   2. Immerse wafer for 15 min (900 s)
   3. Perform solvent cleaning with acetone, IPA, and methanol
   4. Dry with nitrogen gun
   5. **CHECKPOINT**: All photoresist removed

### Mask 4 - Metal Etch (Positive Tone)

**Purpose**: Define metal patterns for device connections

**Process Parameters**:

- Photoresist: AZ® 1512 (Positive)
- Spin Speed: 3000 RPM for 30 s (0.5 min)
- Soft Bake: 110°C for 60 s (1.0 min)
- Exposure: 120 mJ/cm² (17.9 s at 6.7 mW/cm²)
- Developer: AZ® 300 MIF for 45 s (0.75 min)
- Hard Bake: 110°C for 5 min (300 s)

1. **Wafer Preparation**

   1. Clean wafers with acetone, IPA, and methanol
   2. Dry with nitrogen gun
   3. **CHECKPOINT**: Surface should be clean
2. **Spin Coating**

   1. Program spin coater (3000 RPM, 30 s, 3 s accel, 0.5 s decel)
   2. Center wafer on chuck
   3. Apply full dropper of AZ® 1512
   4. Run spin program
   5. **CHECKPOINT**: Coating should be uniform
3. **Soft Bake**

   1. Transfer wafer to hot plate at 110°C
   2. Bake for 60 s (1.0 min)
   3. Allow wafer to cool
   4. **CHECKPOINT**: Surface should appear uniform
4. **Exposure**

   1. Measure UV intensity
   2. Calculate exposure time (120 mJ/cm² ÷ measured intensity)
   3. Load Mask 4 (brown/chrome side up)
   4. Load substrate onto chuck
   5. Expose for calculated time
   6. **CHECKPOINT**: Exposure completed successfully
5. **Development**

   1. Immerse wafer in AZ® 300 MIF for 45 s (0.75 min)
   2. Rinse in DI water for 30 s (0.5 min) in each of two beakers
   3. Final rinse under flowing DI water
   4. Dry with nitrogen gun
   5. **CHECKPOINT**: Pattern is clearly visible
6. **Hard Bake**

   1. Place wafer in oven at 110°C
   2. Bake for 5 min (300 s)
   3. Allow wafer to cool
   4. **CHECKPOINT**: No visible defects
7. **Metal Etch**

   1. Follow Metal Etch SOP
   2. **CHECKPOINT**: Etching completed successfully

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

---

## Detailed Process Steps

### Spin Coating & Soft Bake

1. Program the spin coater and hot plate to the settings.
   - *See [Spin Coater Parameters](#appendix-a-process-parameter-tables) and [Soft Bake Parameters](#appendix-a-process-parameter-tables) in Appendix A.*
2. Center the wafer on the rotation chuck.
3. Test the spin for uniform rotation.
4. Apply approximately 7 drops of HMDS at the wafer center.
   - *Note: HMDS is the adhesion promoter for Si/SiO₂ substrates.*
5. Close the lid and press "Start."
6. Immediately deposit approximately 1–2 mL of photoresist.
   - *1–2 mL is an approximate amount; in general, this is a full dropper.*
7. Close the lid and press "Start."
8. Immediately transfer the coated wafer to the center of the hot plate.
9. Wait the prescribed time (see [Soft Bake Parameters](#appendix-a-process-parameter-tables) in Appendix A), then remove the wafer from the hot plate and let it cool down.

### Patterning

**IMPORTANT:** Do not let the mask's brown/chrome side contact any surface.

#### UV Intensity & Exposure Calculation

1. Measure the UV intensity with the intensity meter.
2. Calculate the exposure time:

   Exposure Time [s] = Required Dose [mJ/cm²] / Measured Intensity [mW/cm²]
3. See [Exposure Dosage](#appendix-a-process-parameter-tables) in Appendix A for required doses.

#### Loading the Mask

1. Unscrew the mask holder from the stage.
2. Carefully slide the mask holder from the stage.
3. Place the mask (brown-side up and not contacting any surface) on the mask holder.
4. Ensure that the mask is centered in the hole.
5. Reinsert the mask holder into the stage and clamp it down using the knurled knobs.

#### Loading the Substrate

1. Ensure that the transport slide (labeled 32) is not under the mask.
2. Load the substrate (wafer with spun photoresist) onto the chuck, covering all vacuum holes.
3. Move the transport slide so that the substrate is under the mask.

#### Exposure & Alignment

1. Rotate the contact lever 180° counterclockwise to bring the wafer into contact with the mask. The contact indicator should light.
2. Separate slightly to focus with the microscope, and align using X-Y micromanipulators.
3. Return to contact and verify alignment at high magnification.
4. Set the exposure timer based on your dose calculation.
5. Press "EXPOSURE" (never look directly at the UV light).
6. Ensure that the contact indicator is illuminated before the actual exposure.
7. After exposure, rotate the lever 180° clockwise to release.
8. Pull the transport slide and remove the wafer from the chuck.

#### Post Exposure Bake (AZ® nLOF™ 2020 Only)

1. Program the hot plate settings.
   - *See [Post Exposure Bake Parameters](#appendix-a-process-parameter-tables) in Appendix A.*
2. Place the exposed wafer in the center of the hot plate.
3. Wait the prescribed time (see [Post Exposure Bake Parameters](#appendix-a-process-parameter-tables) in Appendix A), then remove the wafer from the hot plate and let it cool down.

### Development

**Developer Selection:**

- AZ® 300 MIF is compatible with both `AZ® 1512` and `AZ® nLOF™ 2020` photoresist.

1. Secure the wafer in a 3-prong holder.
2. Immerse the wafer in AZ® 300 MIF developer.
   - *See [Quick Reference Parameters](#quick-reference-parameters) for development times.*
3. Replace the developer if time exceeds 90 s (developer exhaustion).
4. Rinse in two DI water beakers for approximately 30 s each.
5. Perform a final DI rinse under flowing DI water.
6. Dry with a nitrogen gun.

### Hard Bake

**Note:** Increasing the hard-bake time significantly increases the likelihood that the photoresist will not effectively strip, specifically for `AZ® 1512` processes.

1. Program the oven settings.
   - *See [Hard Bake Parameters](#appendix-a-process-parameter-tables) in Appendix A.*
2. Place the wafers on a sheet of aluminum foil near the center of the oven.
3. Wait the prescribed time (see [Hard Bake Parameters](#appendix-a-process-parameter-tables) in Appendix A), then remove the wafer from the oven and let it cool down.

### Stripping

#### AZ® NMP Rinse & AZ® KWIK Strip

1. Program the hot plate settings.
   - *See [Strip (AZ® NMP &amp; AZ® KWIK Strip) Parameters](#appendix-a-process-parameter-tables) in Appendix A.*
2. Submerge the wafer in the stripper with gentle agitation.
3. Wait the prescribed time (see [Strip (AZ® NMP &amp; AZ® KWIK Strip) Parameters](#appendix-a-process-parameter-tables) in Appendix A), then remove the wafer from the bath.
4. Immediately rinse in a warm (60°C) DI water beaker.
5. Immediately rinse in a room-temperature DI water beaker.
6. If residue remains, repeat the process or apply mild ultrasonic cleaning.
7. Perform solvent cleaning with acetone, IPA, and methanol.

#### AZ® 910 Remover

1. Program the hot plate settings.
   - *See [Strip (AZ® 910 Remover) Process Parameters](#appendix-a-process-parameter-tables) in Appendix A.*
2. Submerge the wafer in `AZ® 910 Remover` maintained at 50–60°C for 5–20 minutes.
   - *Note:* Use the recommended parameters in [Strip (AZ® 910 Remover) Process Parameters](#appendix-a-process-parameter-tables) in Appendix A.
3. Rinse the wafer in DI water for 5 minutes.
4. Dry the wafer using a nitrogen gun.
5. Perform solvent cleaning with acetone, IPA, and methanol.

---

## Process Documentation

### Process Logbook

Maintaining accurate process records is essential for achieving consistency and troubleshooting issues. Users should record key parameters for each process run:

1. **Basic Information**

   1. Date and time
   2. Operator name
   3. Process description/purpose
   4. Wafer identification
2. **Process Parameters**

   1. Photoresist type and batch number
   2. Spin coating parameters (speed, time)
   3. Bake temperatures and times
   4. Measured UV intensity
   5. Calculated and actual exposure time
   6. Developer type and time
   7. Process results and observations
3. **Troubleshooting Notes**

   1. Any issues encountered
   2. Solutions attempted
   3. Recommendations for future runs

A sample logbook template is provided in Appendix B.

## Appendices

### Appendix A: Process Parameter Tables

### Exposure Dosage

| **Photoresist Type** | **Recommended Dosage [mJ/cm²]** |
| -------------------------- | -------------------------------------- |
| AZ® 1512                  | 90–150                                |
| AZ® nLOF™ 2020           | 66–80                                 |

*Table: Photoresist Recommended Dosages*

### Spin Coater Parameters

| **Parameter** | **Value** |
| ------------------- | --------------- |
| Acceleration (s)    | 3               |
| Deceleration (s)    | 0.5             |
| Target (RPM)        | 3000            |
| Spin Time (s)       | 30              |

*Table: Spin Coater Parameters*

### Additional Spin Coat Dosage Parameters

| **Dosage Type**                                | **Value** |
| ---------------------------------------------------- | --------------- |
| HMDS Dosage (Non-Metal Substrate)                    | 7 Drops         |
| Positive/Negative Tone Dosage (1500 and 2000 Series) | Full Dropper    |

*Table: Additional Spin Coat Dosage Parameters*

### Soft Bake (SB) Parameters

| **Parameter** | **Value** |
| ------------------- | --------------- |
| Temperature (°C)   | 110             |
| Time (s)            | 60              |

*Table: Soft Bake Parameters*

### Post Exposure Bake (PEB) Parameters

| **Parameter** | **Value** |
| ------------------- | --------------- |
| Temperature (°C)   | 110             |
| Time (s)            | 60              |

*Table: Post Exposure Bake Parameters*

### Hard Bake (HB) Parameters

| **Parameter** | **Value** |
| ------------------- | --------------- |
| Temperature (°C)   | 110             |
| Time (min)          | 0–60           |

*Table: Hard Bake Parameters*

### Strip (AZ® NMP & AZ® KWIK Strip) Parameters

| **Parameter** | **Value** |
| ------------------- | --------------- |
| Temperature (°C)   | 90              |
| Time (min)          | 45–60          |

*Table: Strip (AZ® NMP & AZ® KWIK Strip) Parameters*

### Strip (AZ® 910 Remover) Process Parameters

| **Parameter**       | **Value**        |
| ------------------------- | ---------------------- |
| Temperature (°C)         | 50-60                  |
| Strip Time (min)          | 15                     |
| DI Water Rinse Time (min) | 5                      |
| Drying                    | Nitrogen Gun           |
| Solvent Cleaning          | Acetone, IPA, Methanol |

*Table: Strip (AZ® 910 Remover) Process Parameters*

### Chemical Compatibility

AZ® 1512 Photoresist:

- Adhesion Promoter
  - HMDS.
- Developer
  - AZ® 300 MIF.
- Stripper
  - AZ® 910 Remover.
  - AZ® NMP Rinse.
  - AZ® KWIK Strip.

AZ® nLOF™ 2020 Photoresist:

- Adhesion Promoter
  - HMDS.
- Developer
  - AZ® 300 MIF.
- Stripper
  - AZ® 910 Remover.
  - AZ® NMP.
  - AZ® KWIK Strip.

### Appendix B: Process Logbook Template

| Parameter                                 | Value | Notes |
| ----------------------------------------- | ----- | ----- |
| **Date/Time**                       |       |       |
| **Operator**                        |       |       |
| **Process Description**             |       |       |
| **Wafer ID**                        |       |       |
| **Photoresist Type/Batch**          |       |       |
| **Spin Speed (RPM)**                |       |       |
| **Spin Time (s)**                   |       |       |
| **Soft Bake Temp (°C)**            |       |       |
| **Soft Bake Time (s)**              |       |       |
| **Measured UV Intensity (mW/cm²)** |       |       |
| **Required Dose (mJ/cm²)**         |       |       |
| **Calculated Exposure Time (s)**    |       |       |
| **Actual Exposure Time (s)**        |       |       |
| **Developer Type**                  |       |       |
| **Development Time (s)**            |       |       |
| **Hard Bake Temp (°C)**            |       |       |
| **Hard Bake Time (s)**              |       |       |
| **Process Results**                 |       |       |
| **Issues Encountered**              |       |       |
| **Solutions/Recommendations**       |       |       |
