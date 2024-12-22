# 3d-printing
An accumulation of my settings and experiences

## Checklist before starting a print:
- Slicer: Correct Printer, Profile, Filament used? Checked for Oerhangs/Bridging?
- Machine: Belt Tension correct? Nozzle unclogged/clean? Any signs of changes on last print?

## First Layer Problems:
- Adhesive force is caused by a complex behaviour between two surfaces. Keep your plate very clean! Wash your plate with water, soap and a kitchen sponge (maybe multiple times)! Don’t use IPA! Don’t touch your Plate! Don’t get dust or fibers on your plate (maybe use cleaning paper)! Use one plate for one purpose/material or clean the plates very good (multiple times) between those applications! Maybe wear latex-gloves!
- Heat your bed up! Slow Down First Layer speed (30-60 mm/s on ABS)! Make your first Layer height larger (0.25 on a 0.4 nozzle)! Do more squish (~0.04) on a textured plate!
- Make sure your squish is correct over the whole plate (just test-print 9x 20x20x0,25 samples)! Calibrate your Z-Offset with everything (bed, chamber, nozzle, ...) Pre-Heated!
- If your probe has an offset (especially a Y-Offset) to your nozzle, check the real distances after your bed-mesh calibration! Your Toolhead could tilt in different locations depending on your 3D-printers setup.
        
## ABS Warping:
- Check the Section First Layer Problems!
- Heat soak your machine for a minimum of one hour! Also Pre-Heat your nozzle to the printing temperature!
- No Fan-Speed for the first Layers 1-4. Use Fan-Speeds in your Enclosure (Maybe 50% for larger plates, ~80% for smaller plates)! This will shrink your freshly printed locations faster and you’ll have smaller regions of contractions! BUT using the fan also increases the risk of bad layer adhesion!
- Only as a last resort use Adhesion-Helpers (3DLAC, etc.)!

## Curling:
![Parts with curling on overhangs](https://github.com/interias/3d-printing/blob/main/images/curling.jpg)
- Try more Part-Cooling-Fan-Speed.
- Maybe Part-Cooling-Fan is defect or to weak?
- Decrease perimeter-speeds, like 30-40 mm/s for outer-perimeter and 80 for inner-perimeter
- Reduce Bed-Temperature.

## Burned material
Material and fine threads can get caught on the nozzle and the silicone sock of the hotend and burn. The burnt pieces can get into the print part.
![Burned material in parts](https://github.com/interias/3d-printing/blob/main/images/burned-material.jpg)
- Clean your hotend and silicon sock from the outside
- Reduce print temperature, especially on bright and transparent materials.
- Clean your nozzle and heatbreak. A good helper can be cleaning filament.
