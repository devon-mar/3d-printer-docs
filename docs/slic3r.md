# Slic3r

## Enable supports

1. Open the **Print Settings** tab
2. Select **Support material** from the left hand menu
3. Check **Generate Support Material**
4. Click **Yes** to detect bridging perimeters
5. Select **0.2 (detachable)** for **Contact Z distance**
6. Optionally, check **Support on build plate only** to build supports only on the build plate
7. Optionally, uncheck **Don’t support bridges**

## Enable brim

1. Open the **Print Settings** tab
2. Select **Skirt and brim**
3. Enter a value in mm under **Brim width**

## OctoPrint Integration

Integrating slic3r with octoprint enables the Send to printer button to send gcode files directly to OctoPrint for printing.

1. Open OctoPrint
2. Copy the API key under **Settings > API Key**
3. In Slic3r, select the **Printer Settings** tab
4. Select the **OCTOPRINT** profile

    !!! note
        If the Octoprint profile doesn’t exist (new Slic3r installation) select the **Original Prusa i3 MK2 profile.** This will edit the stock profile with OctoPrint settings.

5. Enter the hostname :code:`j3d-prusa.vsb.bc.ca` under **Host or IP**
6. Enter the API key copied earlier
7. Click ![slic3r save](images/slic3r-saveicon.png)
8. If the OCTOPRINT profile didn't previously exist, append `octoprint` to the profile name. Otherwise, skip this step
9. Click **OK**

## Change print temperatures

1. Select the **Filament Settings** tab
2. Enter the desired extruder and bed temperatures in the corresponding boxes.
