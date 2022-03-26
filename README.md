# EZ30D Definitions
01-04 Subaru EZ30D ECU definitions I've mostly created myself. A couple I've collected from other sources.
I only defined what I needed - quick and dirty. Some parameters and codes might be defined in one revision but not another.  

Feel free to use what you can. I might update these if you ask. Adding OBDII codes to them is easy if that's what you need.  

If you have a ROM that isn't defined here, get ahold of me and ask nicely - I may have the time to create and add your definition to this list!  

# How to Use
Copy the definition files to the `C:\Program Files (x86)\OpenECU\EcuFlash\rommetadata\subaru\Outback 3.0R\` directory, or wherever you have installed ECUFlash. Once you close and re-open ECUFlash, you should be able to open a ROM covered by these definitions.  
There's already a D6JM000B in there. I rename the file extension to `.bak` or delete that one to keep it from being loaded. It doesn't have as much defined as the one you get here.  

# General EZ30D ECU Tips
* Flash an EZ30D ECU just like an 02-05 WRX - including flash block and test connectors. Use ECUFlash.  

* If you're manual swapping, it works best to leave the Park/Neutral pin floating on the ECU and remove your TCU completely.  

* Lightweight flywheels cause idle stability issues in most cases.  

* 01-02 EZ30D ECUs and ROMs are interchangeable. 02 added one fuel tank sensor but the code for it can be turned off.  

* 03-04 EZ30D ECUs and ROMs are interchangeable. 03-04 ECUs switched from a fuel pump relay setup to a variable duty FPC (Fuel Pump Controller) like an 02-05 WRX has. Using an 03-04 ROM in a car with a fuel pump relay wired up causes issues. I haven't tried flashing an 01-02 ROM on an 03-04 ECU or vice versa. Good luck to you if you need to attempt that. It will probably not brick your ECU, but no guarantees!  

* I have never been able to read or flash an EZ30D ECU that came with an immobilizer. Some (or all?) EDM delivered EZ30D cars have them. You're welcome to try, and I'd love to hear if you are successful!  

* If you are swapping an automatic EZ30D Outback to manual and you want to retain ABS and cruise, all you need is an ABS module and cruise module from a factory 5-speed Outback.

# Tuning Tips
If you put a manual behind an EZ30D, make these changes:
1. Disable any codes you have active
2. Raise idle to 800ish minimum on all tables
3. Take the low RPM low load timing cells and bump them up to 21 degrees or so. This helps a lot with off-idle driveability.
4. Raise the rev limiter - for fun!

# Interesting Asides
* D6HB200A is the most well-defined ROM here - it's also one I did not create. I just recently found it on the RomRaider forums. Having it to start with would have saved me a lot of work in the beginning, but I did my first EZ30D swap (and subsequent defining/tuning) years before that definition was created. I pored over my original ROM for hours and hours to define not even half of what is in that definition, so I'm no expert.  

* I have a 2002 Subaru Outback Limited that was originally delivered as an EJ25/5mt car. I've owned it for many years. The first EJ25 shot a rod *through* the block. I swapped in EJ25 number two. The original 5mt transmission gave up so I swapped in an '04 JDM Forester dual range 5mt. Threw on a 2" lift and some bigger tires. That really made the EJ25 seem gutless, so I formulated the EZ30 swap plan and acquired a salvage auction '01 LLBean. One day, while cruising the local logging roads, I managed to dunk the intake and hydrolock that EJ25. I wanted to use the EZ30 with the factory ECU, with my dual range 5mt, but with no codes and no stalling at stops. So I dug in and disassembled the ROM on my donor car to start. That being said, I'm not a pro, I'm just a guy with a fun swapped Outback.  

* An EZ30 with a manual is a beautiful thing, and the world needs more of them!  
