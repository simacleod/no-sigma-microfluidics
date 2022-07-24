# No-sigma microfluidics

## Glass/PDMS microfluidics fabrication protocol


This protocol is designed to enable anyone who decides for some strange reason they need to start prototyping microfluidics to do so without having a job at some fancy laboratory or a sigma account. Everything used in this protocol is available on amazon.The bare minimum setup will run $400-500 including the printer and both kinds of resin. 

The key to this process is the use of a commercial cosmetics grade handheld plasma wand to produce an oxygen plasma suitable for surface treatment of the glass/PDMS before bonding. The laboratory grade versions of this device are a lot beefier (30W vs 10W) and can treat a much larger area, but they cost upwards of $900. It may be possible to modify a cosmetic grade plasma wand to boost the output, potentially by bypassing the potentiometer in order to increase the effectiveness of the wand. Further research in this area is required.

The other obvious boon to the setup is the recent commercialization of cheap 4K resin printers; when I started down the microfluidics rabbithole 5 years ago similar hardware cost well over $1k -- mine has a 35um pixel size and cost about $350.


### Equipment

- Toaster oven
- 4K 3D resin printer
- UV curing chamber or UV flashlight
- resin printer cleaning station or >250ml mason jar
- 10W cosmetic plasma wand

### Materials

- \> 90% Isopropyl alcohol
- Dish soap, unscented ~0.5ml
- Scotch tape
- Small cups for mixing
- Microscope slides
- Polydimethylsiloxane (PDMS) resin kit
- 3D printer resin

### Safety

When using the plasma wand or any other high voltage equipment, use only one hand to work. NEVER touch the device or place your other hand anywhere near the work area.

Wear a facemask and gloves when working with the 3D printer/PDMS resin.

## Instructions

### MASTER MOLD FABRICATION
1. Design a master mold for your device. Remember poiseuille's law, and trust your instincts. Or do a bunch of math in comsol like a nerd lol.
2. Print the mold at the optimal settings for your printer/resin that give the best detail.
3. Follow the usual steps for cleaning/curing a resin print. Ensure all uncured resin is thoroughly removed.

### MOLD RELEASE COAT
4. Mix 1 part dish soap with 20 parts isopropyl alcohol.
5. Pour the mixture into the master, evenly coating all surfaces, and pour off the excess. The goal is to make a thin coating of dish soap as a mold release agent.
6. Using a blowdryer, quickly evaporate most of the mixture.
7. Wick off the portions of the mixture that remain with a cotton swab. 
8. Blowdry the master until bone-dry

### PDMS REPLICATION
9.  Mix the recommended amount of PDMS resin and crosslinker.
10. Remove most of the bubbles by poking them with a toothpick
11. Attach any hardware, tubing which plugs into the mold
12. Pour the resin into the mold
13. Place the master on a foil sheet and put in toaster oven at the recommended temperature and maximum cure time for your resin.

### DEVICE BONDING
14. Clean a microscope slide with dish soap and water. Observe the surface to ensure no oils remain. 
15. Pat the slide clean with a paper towel or tissue.
16. Place a few piece of scotch tape to cover the slide.
17. Remove the master from the oven.
18. Use a butterknife to remove the replica from the master. Slide it between the edges of the mold to start, and slowly, gently peel the PDMS from the master. DO NOT TOUCH the surface with the channels or your device will fail.
19. Remove the tape from the microscope slide.
20. Run the plasma wand electrode for two minutes along both surfaces, as close as possible without touching.
21. Place the replica over the slide, taking care to line up the edges. Press gently on the device until no air bubbles remain.
22. Place the device in the toaster oven at 210f for one hour. Allow 10mins cooling time before removal.
23. Test the device.

If everything was done correctly, the device should now be firmly bonded to the microscope slide. Pinch the sides firmly to confirm the strength of the bond.


#### my specific setup:
- printer - Elegoo Mars 3 Pro 4K https://www.amazon.com/dp/B09JNRVBYB?psc=1&ref=ppx_yo2ov_dt_b_product_details
- uv resin - Elegoo ABS-like translucent https://www.amazon.com/dp/B09D82B1GQ?psc=1&ref=ppx_yo2ov_dt_b_product_details
- PDMS resin - QSIL 216 https://www.amazon.com/dp/B075F5CKFX?psc=1&ref=ppx_yo2ov_dt_b_product_details
- print settings - 50um layer height, 15sec exposure time  60sec/3 layer burn-in
- Plasma wand - NuDerma https://www.amazon.com/dp/B06W5PD1KY?psc=1&ref=ppx_yo2ov_dt_b_product_details

### Troubleshooting:

1. The PDMS fails to cure in some places
- A: Ensure PDMS is thoroughly mixed. Wash the dish soap coating from the master and re-do it, ensuring your coating is as thin and uniform as possible

2. The PDMS is difficult to remove from the master
- A: Yes, it is. You have to be careful and patient. 

3. The PDMS is impossible to remove from the master
- A: If the soap coating is insufficient to keep the PDMS from sticking the PDMS will be very difficult to remove completely. Print a new master.

4. The PDMS has failed to bond to the microscope slide in some places. 
- A: You either have a contaminant on your surfaces or the plasma cleaning process wasn't thorough enough. Start over with a freshly casted replica. 
