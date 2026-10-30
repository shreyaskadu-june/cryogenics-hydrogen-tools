# Cryogenics and Liquid Hydrogen Tools

Interactive pages on cryogenic hydrogen. Each page is self-contained; the data is embedded in the page or in a JSON file next to it.

## Pages
- `index.html`: phase and property explorer (density and enthalpy vs temperature at a chosen pressure, 1–100 bar, 14–100 K).
- `boiloff/`: liquid hydrogen tank boil-off (heat leak from the NASA 1991 multilayer insulation test, scaled by tank area and insulation factor).
- `cooldown/`: transfer line cooldown to 20 K (copper heat capacity from NIST, hydrogen enthalpy from NIST via CoolProp, utilisation calibrated to the NBS 1966 test).
- `liquefaction/`: liquefaction energy against the theoretical minimum (2.88 kWh/kg, HDSAM) and the DOE industrial range (10–20 kWh/kg).

## Data
- `h2_cryo_props.json`: generated from NIST Standard Reference Database 12 via CoolProp (version in the file).

Status: prototypes, not yet checked against a second source. Known gaps are listed on each page under "Not modelled".

## Sources added
- NBS Report 9264 (Brennan et al., 1967, NASA copy): hydrogen cooldown time vs driving pressure for the 61 m copper line (Figure 8, read from the figure, about ±5 s). Used as a reference on `cooldown/`.
