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
- Only as a last resort use Adhesion-Helpers, e.q. 3DLAC (https://www.3dlac.com/).

## Curling:
![Parts with curling on overhangs](https://github.com/interias/3d-printing/blob/main/images/curling.jpg)
- Try more Part-Cooling-Fan-Speed.
- Maybe Part-Cooling-Fan is defect or to weak?
- Decrease perimeter-speeds, like 30-40 mm/s for outer-perimeter and 80 for inner-perimeter
- Reduce Bed-Temperature.

## Too hot Nozzle-Temperature / Defect Thermistor
![Too hot printing temperature](https://github.com/interias/3d-printing/blob/main/images/too-hot-printing-temperature.jpg)
- Strong Vibration Patterns on areas with acceleration/deceleration can be rooted by too hot Noozzle-Temperature. This can be caused by a defect thermistor or not/wrong tuned in PID Control of the Extruder Heater.

## Burned material
Material and fine threads can get caught on the nozzle and the silicone sock of the hotend and burn. The burnt pieces can get into the print part.
![Burned material in parts](https://github.com/interias/3d-printing/blob/main/images/burned-material.jpg)
- Clean your hotend and silicon sock from the outside
- Reduce print temperature, especially on bright and transparent materials.
- Clean your nozzle and heatbreak. A good helper can be cleaning filament.

## Greasing/Lubrication of Linear Rails
- Hiwin's recommendations: https://www.hiwin.com/pdf/lubricating_instructions.pdf 
- Hiwin explicitly recommends not using greases with solid particles - so anything based on graphite, PTFE/Teflon and MOS2/molybdenum(IV) sulphide is out of the question.
- Recommendations: HIWIN G05, Klüber GL-261, Mobil Mobilux EP1, Fuchs Lubritech Lagermeister BF2, Lubcon TURMOGREASE CAK 2502

## Timing Belts
Inexpensive timing belts are unsuitable for ABS pressure chamber temperatures and have a pronounced settling or creeping behavior, or can even break. Money invested in high-quality timing belts for continuous use at 130 °C is a good investment. These belts have low settling and creep behavior so that the A/B belts remain as similar as possible even after several hundred to thousand hours of pressure.

Ensuring Proper Belt Alignment and Tension: The Key to Precision and Consistent Extrusion Patterns
Before making specific adjustments, such as setting belt tension, analyzing motor frequencies, or other optimizations, it is essential to ensure that the belt is free from transverse stresses. This means that no lateral forces should act on the belt, which could be caused by defective, poorly manufactured, or incorrectly assembled components. Such lateral forces can cause the belt to deviate from its ideal linear motion path, potentially leading to issues like "belt wobble."

A misaligned or unevenly running belt directly affects the motion of the tool head, leading to fluctuations in its movement. These fluctuations can, in turn, result in oscillating extrusion patterns, which negatively impact print quality.

For example, a misaligned idler pulley with a damaged bearing may not rotate smoothly, creating uneven tension in the belt and causing it to run irregularly (see picture below). Similarly, improperly aligned toothed pulleys can cause the belt to sit crookedly on the gear teeth, applying lateral forces that disrupt its linear travel.

![Defect Idler](https://github.com/interias/3d-printing/blob/main/images/defect-idler.jpg)

The observation that the frequency of extrusion patterns changes at different speeds can be explained by the belt's dynamic behavior: at higher speeds, the belt may effectively "skip over" minor imperfections, much like a car driving quickly over a rough grid, experiencing less impact from the unevenness. This highlights the importance of a well-aligned and mechanically sound setup as the foundation for achieving precision in the system.
