Standard Operating Procedure (SOP)  
Fort Lewis College  
Senior Seminar 2024-2025

**Author:** Lincoln Scheer  
**Updated:** March 4, 2025

---

## Adapted From

PSR Photolithography Unit Process SOP.

---

## Notes

This SOP outlines the photolithography unit process, providing a standardized procedure for wafer preparation, photoresist application, patterning, and development. The goal is to ensure process consistency, repeatability, and safety. This document is actively developed and refined; modifications may be made as improvements are identified.

---

## Table of Contents

1. [Equipment and Materials](#equipment-and-materials)
2. [Startup Procedure](#startup-procedure)
3. [Shutdown Procedure](#shutdown-procedure)
4. [Spin Coating & Soft Bake](#spin-coating--soft-bake)
5. [Patterning](#patterning)
6. [Development](#development)
7. [Hard Bake](#hard-bake)
8. [Stripping](#stripping)
9. [Recommended Process Parameters](#recommended-process-parameters)
10. [Chemical Compatibility](#chemical-compatibility)

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
  - `AZ® 400K (4:1)` (for `AZ® 1512`).
  - `AZ® 300 MIF` (for `AZ® nLOF™ 2020`).
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

## Startup Procedure

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

## Shutdown Procedure

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

## Spin Coating & Soft Bake

1. Program the spin coater and hot plate to the settings.  
   - *Process parameters are available in [Recommended Process Parameters](#recommended-process-parameters).*
2. Center the wafer on the rotation chuck.
3. Test the spin for uniform rotation.
4. Apply approximately 7 drops of HMDS at the wafer center.  
   - *Note: HMDS is the adhesion promoter for Si/SiO₂ substrates.*
5. Close the lid and press "Start."
6. Immediately deposit approximately 1–2 mL of photoresist.  
   - *1–2 mL is an approximate amount; in general, this is a full dropper.*
7. Close the lid and press "Start."
8. Immediately transfer the coated wafer to the center of the hot plate.
9. Wait the prescribed time (see [Recommended Process Parameters](#recommended-process-parameters)), then remove the wafer from the hot plate and let it cool down.

---

## Patterning

**IMPORTANT:** Do not let the mask's brown/chrome side contact any surface.

### UV Intensity & Exposure Calculation

1. Measure the UV intensity with the intensity meter.
2. Calculate the exposure time:

   Exposure Time [s] = Required Dose [mJ/cm²] / Measured Intensity [mW/cm²]

3. Process parameters, such as the required dose, are available in [Recommended Process Parameters](#recommended-process-parameters).

### Loading the Mask

1. Unscrew the mask holder from the stage.
2. Carefully slide the mask holder from the stage.
3. Place the mask (brown-side up and not contacting any surface) on the mask holder.
4. Ensure that the mask is centered in the hole.
5. Reinsert the mask holder into the stage and clamp it down using the knurled knobs.

### Loading the Substrate

1. Ensure that the transport slide (labeled 32) is not under the mask.
2. Load the substrate (wafer with spun photoresist) onto the chuck, covering all vacuum holes.
3. Move the transport slide so that the substrate is under the mask.

### Exposure & Alignment

1. Rotate the contact lever 180° counterclockwise to bring the wafer into contact with the mask. The contact indicator should light.
2. Separate slightly to focus with the microscope, and align using X-Y micromanipulators.
3. Return to contact and verify alignment at high magnification.
4. Set the exposure timer based on your dose calculation.
5. Press "EXPOSURE" (never look directly at the UV light).
6. Ensure that the contact indicator is illuminated before the actual exposure.
7. After exposure, rotate the lever 180° clockwise to release.
8. Pull the transport slide and remove the wafer from the chuck.

### Post Exposure Bake (AZ® nLOF™ 2020 Only)

1. Program the hot plate settings.  
   - *Process parameters are available in [Recommended Process Parameters](#recommended-process-parameters).*
2. Place the exposed wafer in the center of the hot plate.
3. Wait the prescribed time (see [Recommended Process Parameters](#recommended-process-parameters)), then remove the wafer from the hot plate and let it cool down.

---

## Development

**Developer Selection:**  
- Note that `AZ® 400K (4:1)` is only compatible with `AZ® 1512` photoresist.  
- `AZ® 300 MIF` is compatible with both `AZ® 1512` and `AZ® nLOF™ 2020` photoresist.

1. Secure the wafer in a 3-prong holder.
2. Immerse the wafer in the appropriate developer.  
   - *Detailed parameters are available in [Recommended Process Parameters](#recommended-process-parameters).*
3. Replace the developer if time exceeds 90 s (developer exhaustion).
4. Rinse in two DI water beakers for approximately 30 s each.
5. Perform a final DI rinse under flowing DI water.
6. Dry with a nitrogen gun.

---

## Hard Bake

**Note:** Increasing the hard-bake time significantly increases the likelihood that the photoresist will not effectively strip, specifically for `AZ® 1512` processes.

1. Program the oven settings.  
   - *Process parameters are available in [Recommended Process Parameters](#recommended-process-parameters).*
2. Place the wafers on a sheet of aluminum foil near the center of the oven.
3. Wait the prescribed time (see [Recommended Process Parameters](#recommended-process-parameters)), then remove the wafer from the oven and let it cool down.

---

## Stripping

### AZ® NMP Rinse & AZ® KWIK Strip

1. Program the hot plate settings.  
   - *Process parameters are available in [Recommended Process Parameters](#recommended-process-parameters).*
2. Submerge the wafer in the stripper with gentle agitation.
3. Wait the prescribed time (see [Recommended Process Parameters](#recommended-process-parameters)), then remove the wafer from the bath.
4. Immediately rinse in a warm (60°C) DI water beaker.
5. Immediately rinse in a room-temperature DI water beaker.
6. If residue remains, repeat the process or apply mild ultrasonic cleaning.
7. Perform solvent cleaning with acetone, IPA, and methanol.

### AZ® 910 Remover

1. Program the hot plate settings.  
   - *Process parameters are available in [Recommended Process Parameters](#recommended-process-parameters).*
2. Submerge the wafer in `AZ® 910 Remover` maintained at 50–80°C for 5–20 minutes.
   - *Note:* Use the recommended parameters in [Recommended Process Parameters](#recommended-process-parameters).
3. Rinse the wafer in DI water for 5 minutes.
4. Dry the wafer using a nitrogen gun.
5. Perform solvent cleaning with acetone, IPA, and methanol.

---

## Recommended Process Parameters

### Exposure Dosage

| **Photoresist Type** | **Recommended Dosage [mJ/cm²]** |
|----------------------|---------------------------------|
| AZ® 1512           | 90–150                          |
| AZ® nLOF™ 2020     | 66–80                           |

*Table: Photoresist Recommended Dosages*

### Spin Coater Parameters

| **Parameter**       | **Value** |
|---------------------|-----------|
| Acceleration (s)    | 3         |
| Deceleration (s)    | 0.5       |
| Target (RPM)        | 3000      |
| Spin Time (s)       | 30        |

*Table: Spin Coater Parameters*

### Additional Spin Coat Dosage Parameters

| **Dosage Type**                                         | **Value**     |
|---------------------------------------------------------|---------------|
| HMDS Dosage (Non-Metal Substrate)                       | 7 Drops       |
| Positive/Negative Tone Dosage (1500 and 2000 Series)    | Full Dropper  |

*Table: Additional Spin Coat Dosage Parameters*

### Soft Bake (SB) Parameters

| **Parameter** | **Value** |
|---------------|-----------|
| Temperature (°C) | 110    |
| Time (s)         | 60     |

*Table: Soft Bake Parameters*

### Post Exposure Bake (PEB) Parameters

| **Parameter** | **Value** |
|---------------|-----------|
| Temperature (°C) | 110    |
| Time (s)         | 60     |

*Table: Post Exposure Bake Parameters*

### Hard Bake (HB) Parameters

| **Parameter** | **Value**  |
|---------------|------------|
| Temperature (°C) | 110     |
| Time (min)       | 0–60    |

*Table: Hard Bake Parameters*

### Strip (AZ® NMP & AZ® KWIK Strip) Parameters

| **Parameter** | **Value** |
|---------------|-----------|
| Temperature (°C) | 90     |
| Time (min)       | 45–60  |

*Table: Strip (AZ® NMP & AZ® KWIK Strip) Parameters*

### Strip (AZ® 910 Remover) Process Parameters

| **Parameter**              | **Value**                  |
|----------------------------|----------------------------|
| Temperature (°C)           | 60-70                      |
| Strip Time (min)           | 15                         |
| DI Water Rinse Time (min)  | 5                          |
| Drying                     | Nitrogen Gun               |
| Solvent Cleaning           | Acetone, IPA, Methanol     |

*Table: Strip (AZ® 910 Remover) Process Parameters*

### Chemical Compatibility

AZ® 1512 Photoresist:
   - Adhesion Promoter
      - HMDS.
   - Developer
      - AZ® 400K (4:1).
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
