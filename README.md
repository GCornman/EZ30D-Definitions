# EZ30D Definitions
01-04 Subaru EZ30D ECU definitions I've collected from various sources, and some I've created myself.  
I only defined what I needed - quick and dirty. Some parameters and codes might be defined in one revision but not another.  
Feel free to use what you can. I might update these if you ask. Adding OBDII codes to them is easy if that's what you need.  

# How to Use
Copy the definition files to the `C:\Program Files (x86)\OpenECU\EcuFlash\rommetadata\subaru\Outback 3.0R\` directory, or wherever you have installed ECUFlash. Once you close and re-open ECUFlash, you should be able to open a ROM covered by these definitions.

# General EZ30D ECU Tips
* Flash an EZ30D ECU just like an 02-05 WRX - including flash block and test connectors. Use ECUFlash.  
* If you're manual swapping, it works best to leave the Park/Neutral pin floating on the ECU and remove your TCU completely.  
* Lightweight flywheels cause idle stability issues in most cases.  
* 01-02 EZ30D ECUs and ROMs are interchangeable. 02 added one fuel tank sensor but the code for it can be turned off.  
* 03-04 EZ30D ECUs and ROMs are interchangeable. 03-04 ECUs switched from a fuel pump relay setup to a variable duty FPC (Fuel Pump Controller) like an 02-05 WRX has. Using an 03-04 ROM in a car with a fuel pump relay wired up causes issues. I haven't tried flashing an 01-02 ROM on an 03-04 ECU or vice versa. Good luck to you if you need to attempt that. It will probably not brick your ECU, but no guarantees!  
* I have never been able to read or flash an EZ30D ECU that came with an immobilizer. Some (or all?) EDM delivered EZ30D cars have them. You're welcome to try, and I'd love to hear if you are successful!  

# Interesting Asides
D6HB200A is the most well-defined ROM - it's also one I did not create. I just recently found it on the RomRaider forums. Having it to start with would have saved me a lot of work in the beginning, but I did my first EZ30D swap years before that definition was created. I pored over my original ROM for hours and hours to define not even half of what is in that definition, so I'm no expert.  
