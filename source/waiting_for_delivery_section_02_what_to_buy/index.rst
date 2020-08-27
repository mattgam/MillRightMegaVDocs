Section 2: What else can I spend money on?
==========================================

NOTE THIS IS  A ROUGH ROUGH DRAFT

Section 2a: Introduction
------------------------

Upgrades to the Mega V are very common and a frequent generator of questions on the forums is where to source various components for those projects.  This page is a fairly extensive list of things I have bought (yes I'm an idiot and no I have not itemized this ever for my spouse :-) ) and tried with my Mega V or used in the past.


Section 2b: Essentials Items
----------------------------

+------------------------------------------------------+-------------------------------------------------------+
| Item                                                 |                       Why                             |
+======================================================+=======================================================+
| :ref:`Roll in 2020 M5 T-Nuts and Slide in 3030 T-Nuts| Needed to secure items to the T-Tracks after assembly |
| <tnuts>`                                             |                                                       |
+------------------------------------------------------+-------------------------------------------------------+
| :ref:`Blue Loctite <loctite>`                        | To be put on literally every screw to help keep the   |
|                                                      | CNC from shaking itself apart while running.          |
+------------------------------------------------------+-------------------------------------------------------+
| :ref:`1-2-3 Machinist Blocks <123_blocks>`           | Machinists have used 1 2 3 blocks for years for       |
| `                                                    | tramming, making jigs, measuring, and squaring tools  | 
|                                                      | keeping it running optimally.                         |
+------------------------------------------------------+-------------------------------------------------------+
| `6' USB Cable with a Ferrite Bead                    | The Arduino USB ports are highly suseptible to any    |
| <https://www.amazon.com/Tripp-Lite-Hi-Speed-Ferri    | inteference.  A quality USB cable can reall help      |
| te-U023-003/dp/B003MQ29B2/>`_                        | to reduce problems                                    |
+------------------------------------------------------+-------------------------------------------------------+
| :ref:`18/2 Shielded Wire<18/2_shielded_wire>`        | The homing switch kit comes with poor quality wire    |
|                                                      | that is too short to be of use.  This upgrade replaces|
|                   Or                                 | the original wire with em shielded heavier gauge      |
|                                                      |                                                       |
| :ref:`12/2 Shielded Wire<22/2_shielded_wire>`        |                                                       |
|                                                      |                                                       |
+------------------------------------------------------+-------------------------------------------------------+
| White Lithium Grease                                 | For the Linea brearings                               |
+------------------------------------------------------+-------------------------------------------------------+
| Dry Lube                                             | For the rack and pinions                              |
+------------------------------------------------------+-------------------------------------------------------+
| Brad Ellerbroek's tramming plate                     | While this may not be 100% essential it really does   |
|                                                      | simplify the process of tramming the Mega V.          |
+------------------------------------------------------+-------------------------------------------------------+
| M3-M5 Metric Socket Cap Screw kit                    | As of mid-August 2020, MillRight seems to now be      |
|                                                      | M4x14mm machine screws for mounting the stepper motors|
| M4x16mm socket cap screws                            | .I still prefer M4x16mm Socket Cap for the added      |
|                                                      | threads securing the motor and the better torque      |
|                                                      | a socket cap can handle.  Your call on if you should  |
|                                                      | get these.  In any case I do recommend this screw kit |
|                                                      | or similar just in case you are short something.      |
+------------------------------------------------------+-------------------------------------------------------+
| :ref:`Feeler Gauges<feeler_gauges>`                  | For measuring gaps                                    |
+------------------------------------------------------+-------------------------------------------------------+
|                                                      |                                                       |
+------------------------------------------------------+-------------------------------------------------------+
|                                                      |                                                       |
+------------------------------------------------------+-------------------------------------------------------+

Section 2c: Spare Parts
-----------------------
If you are generating income from your Mega V and this is more than a hobby for you, then downtime is money.  A 
proper set of spare parts is a small investment in insuring your revenue stream doesn't go away along with your customers satisfaction. 

While they don't advertise it on their site, MillRight will sell you spare parts if you reach out to their sales at support@millrightcnc.com. As noted
elsewhere most of the Mega V is commodity hardware which you can source elsewhere some things like the CNC Shield and V-Wheels are custom. I've found 
MillRight to be happy to take my money and ships quickly.

The spare parts that can be purchased from MillRight are:

* 2.5mm Spacers (qty 4)  - $2.00
* 6.35mm Spacers (qty 4) - $2.00
   While no sane person would take their Mega V apart as much as the author has, the steppers do need regular checking and those spacers seem to want to 
   escape if given the chance.  Spares can be a life saver if you lose one.
* Arduino Uno if 3-Axis (qty 1) - ???
   I don't have a 3-Axis machine so don't know what MillRight charges for a spare.  If anyone knows please let me know.
* Arduino Mega XL 4th Axis if 4-Axis (qty 1) - $17.00
   You can buy the Arduino's off the shelf on Amazon but they will need to be flashed with MillRights firmware.
* Mega V Eccentric Spacers (qty 4) - $10.00
* MillRight CNC Shield (qty 1) - $34.00
* MillRight StepperDriver (qty 1) - $36.00
    You may want to consider 2 for this so you can expand the Y to 2 independent drivers
* MillRight KS130 Stepper Motor with  longer cable (qty 1) - $35.00
* v-wheels and bearings (qty 8) - $44.00 
    I got extra due to some modifications I'm testing out

Other spares that can be bought separately are:

* `Dewalt Brushes <https://www.amazon.com/Replacement-Brushes-Dewalt-DWP611-A27343/dp/B07XB2M86M>`_

  .. note:: A little known fact is that a lot of Ace TrueValue hardware stores carry the replacement brushes for the Dewalt DWP611 router.  

* Homing Switches

  * `XY Homing Switches <https://www.amazon.com/gp/product/B0163B6CV0/>`_
  * `Z Homing Switch <https://www.amazon.com/gp/product/B0163B89AW>`_

Section 2c: Computer to Run From
--------------------------------
CNC's don't just run themselves...well not unless you spend a lot more money than you already have but thats a whole different book in need of authoring.  
While you can run your cuts from the same computer you design from, :term:`gcode senders` are best run from a dedicated host to minimize interferance if budget allows.   
The reason for this is that gcode senders must continuously stream :term:`g-code` to the :term:`cnc controller` in order to keep the stepper motors smoothly  moving and the router cutting.  
Other tools running in parallel can interfere with this and jeopardize the cuts.  If budget doesn't allow for a dedicated machine, then just be careful that nothing is running 
on the computer while running a job that could hog the CPU like a Virus Checker.

Choice of computer to use is highly personal and flexble.  Windows 10, Mac, or Linux based computers can run all the major gcode senders.  Windows 10 is most popular in this space with Linux 
close behind in popularity.  Hardware wise, if being used for just running gcode senders the hardware requirements are minimal.  4GB of ram, and an Intel Atom processor is more than enough to 
handle the overhead.  As a result, shopping Facebook Marketplace, OfferUp, and Craigslist for some ones scrap PC will find you a used computer for as low as $100. Try to find a system with Windows 10 Pro  
preinstalled if possible to gain the added remote management features.  

..  warning:: Used computers can have all manner of viruses and malware on them.  Before doing anything reset windows to factory defaults.  Instructions can be found at https://www.laptopmag.com/articles/reset-windows-10-pc

On the forum's these are examples of a few simple computers that are more than good enough that members have used:

* `10" Windows 10 Fusion5 Ultra Slim Windows Tablet PC- (4GB RAM, 128GB Storage, USB 3.0, Intel, 5MP and 2MP Cameras, Windows 10 S Tablet PC) (128GB) <https://www.amazon.com/gp/product/B07W6QYX8G/>`_
   These will run from 175-$275 and are a decent small tablet that is windows capable and what the author uses.

* `Surface Pro 3 Refurb <https://computers.woot.com/offers/microsoft-surface-3-10-64gb-tablet-3>`_ 
   These regularly come up on Woot for around $300 and are a workhorse for a CNC machine.

* `LattePanda <https://www.amazon.com/LattePanda-Powerful.../dp/B073ZD9XD3>`_
    LattePanda - Of the options listed, this is the only one I've never seen run (for what little value my opinion asss). This is a tiny windows PC that also comes with an Arduino Leonardo on 
    board (people are using this type of Arduino to make CNC pendants). It will cost $189-$225 depending on windows licenses and will need a case but looks super slick.

* `Raspbery Pi 4 <https://www.amazon.com/dp/B07XTRK8D4/>`_  
    A Linux alternative to a windows computer, that is a fantastic embedded computer that can be run either with or without a monitor which you may see referred to as *headless*. There is a bit more work involved in setting up a Raspberry Pi but it is more than capable of running machining jobs.

Section 2d: Computer Accessories
--------------------------------
A wireless keyboard can be a great remote to control the :term:`gcode senders`.  One to consider is:

* `EASYTONE Backlit Mini Wireless Keyboard With Touchpad Mouse Combo and Multimedia Keys  <https://www.amazon.com/dp/B01E3B81HU>`_
   I use this with a Raspberry Pi 4 and it is a fantastic combo.  UGS, CNCJS, and Openbuilds Control all support keyboard based jogging.  Beaver CNC has a good `video tutorial <https://www.youtube.com/watch?v=zWXBgLULq-U>`_ on using this keyboard with CNCJS.

* https://www.amazon.com/Chroma-Cables-Audio-Optimized-Resistor/dp/B083QMZ9L3/
   The Raspberry Pi 4 runs hotter than the prior generations and a heatsink case is a good idea for managing that heat.
  

* USB Hub - 


Section 2e: Endmills
---------------------
.. warning:: Amazon is full of Whiteside counterfeits.  Check the comments and reviews of any endmill you order from them.   
             People tend to call out fakes.  I won't buy Whiteside from Amazon after receiving a 
             counterfeit surfacing endmill.

.. warning:: Measure the shank of all endmills you receive especially from chinese imports.  Sometimes a metric endmill won't have a true 1/4" shank and the collet can't hold it firmly and you'll see :term:`runout<Runout>` and uneven depth of cuts from the slippage.

Endmills are complex enough that they deserve their own book.  It is my belief that a good starter set of endmills consists of:

* 1/4" shank 1/4" diameter 2 flute :term:`upcut<endmill>`
* 1/4" shank 1/4" diameter 2 flute :term:`downcut<endmill>`
* 1/4" shank 1/8" diameter 2 flute :term:`compression<endmill>`
* 1/4" shank 1.0mm tip :term:`ball nose<endmill>` (if 3d carving)
* 1/4" shank 1" or 1.5" spoil board surfacing endmill
* 1/4" shank 60 degree :term:`v-bit<endmill>`
* 1/4" shank 90 degree :term:`v-bit<endmill>`

If carving aluminium you may want to buy special coated upcut endmills that will resist aluminum sticking and generally last longer. Common coatings are Titanium Nitride (TiN) and the even harder Titanium Carbon Nitride (TiCN). There is a lot of debate on number of 
flute's for aluminium.  The accepted wisdom is 1 flute so that it makes larger chips which pulls heat aware from the cutting surface.  Many Mega V users report chatter with 1 flute and suggest 2 or even 3 flute cutters as they make more and smaller chips resulting in a higher quality finish.  
Over 3 flutes seems to hurt rather than help as the chips are too small to eliminate heat. Given all this, my suggestion is buy some cheap endmills to experiment with and then decide on if its worth the fancy coatings.  I've been shocked at how well a $2 cutter can perform.

Etching Acrylic and Tile comes up a lot as something people want to do. While it can  be done with a v-bit, there are special drag bits that can give a more detailed finish in acrylic and granite.
  
  * Drag  Endmills
    
    * `Diamond Drag Engraving Bit with 1/4" Shank for CNC Machines <https://www.widgetworksunlimited.com/CNC_Diamond_Drag_Engraving_Bit_p/cnc-dmnd_engrv-250.htm>`_
    * `DIAMOND SPRING LOADED DRAG ENGRAVING TOOL WITH 90 DEGREE TIP <https://www.amazon.com/gp/product/B07DK1TWKG/>`_
  

Section 2f: Trustworthy EndMill Vendors
---------------------------------------
`Amazon <http://www.amazon.com>`_
`````````````````````````````````

Beware the counterfeits, but informed is protected.  Amazon is great for finding both quality and cheap endmills to try out. Some noteworthy options are:

* `JERRAY CNC Carving 3.92 Deg 2 Flutes Tapered Angle Ball Tip Radius=1.0mm X 1/4" Shank Tungsten Solid Carbide HRC55 with TiAIN Coated <https://www.amazon.com/JERRAY-Carving-Tapered-Tungsten-Carbide/dp/B015C6CHUC/>`_ 
* 

`Hobren <https://www.holbren.com/>`_
````````````````````````````````````
* https://www.holbren.com/spoilboard-cnc-cutter-router-bits/
    While Amazon can be challenging for sourcing Whiteside bits I've had excellent service from Holbren and they have decent pricing.   

`Tools Today <https://www.toolstoday.com/>`_
````````````````````````````````````````````
They may not be the cheapest but they stand behind their products with an amazing `6 Month Warranty <https://www.toolstoday.com/t-returns>`_ where you
can return anything for 6 months for any reason. They have replaced endmills I've dropped on the floor for perspective. Don't abuse the generosity but if you are
buying higher end endmills consider giving them your business.  Also, follow their Instagram where they post tons of CNC content https://www.instagram.com/toolstoday/

`Carbide Plus (aka drillman1) <https://www.ebay.com/str/carbideplus>`_
``````````````````````````````````````````````````````````````````````
drillman1 has been a vendor on ebay selling very reasonably priced endmills with super quick shipping basically forever.  I've bought many times from this store with zero issue and they are a very reputable vendor.

`Carbide Tool Source (aka roguesystemsinc) <https://www.ebay.com/str/carbidetoolsource>`_
`````````````````````````````````````````````````````````````````````````````````````````
This is an American company run by 2 guys based in Oregon that manufacture all their products in-house and sells on ebay with no middle men.  They carry a huge line of products with some very specialized
endmills you don't see at many other stores. If you've ever wondered where to get an endmill for an 80% lower look no more.  I found their products to be high quality and I'm always one to support a small 
business where I can.

Local Big Box 
`````````````
Desperate times call for desperate measures, and most people don't realize that Lowes and True Value stores carry a small selection of CNC endmills.  If you have a project due and you just broke your last
endmill this can be a life saver.


Section 2g: Useful Tools
------------------------
I very much follow the Adam Savage rule of "Buy it from Harbor Freight then buy it for life when that breaks".  This list of tools are suggestions and no one should run out and buy all of 
these unless you have a burning desire to spend an awful lot of money.  When deciding if your Big Box Square is good enough vs something like a Woodpecker square I found the  video
https://www.youtube.com/watch?v=vVeqY0LI5Dc to be a good comparison of low versus high end.  Disclaimer I don't work for WoodPecker they just seem to find an awful lot of my paycheck deposited
in their bank account.  

Calipers
````````
* `Mitutoyo 500-197-30 Advanced Onsite Sensor (AOS) Absolute Scale Digital Caliper, 0 to 8"/0 to 200mm Measuring Range, 0.0005"/0.01mm Resolution, LCD <https://www.amazon.com/gp/product/B00I3UA89C>`_ 
    SOOOOOOOO Nice
* INSERT EMPIRE CALIPER
* INSERT HARBOR FREIGHT LINK

Drill bits
``````````
* `Metric M42 8% Cobalt Twist Drill Bits Set for Stainless Steel and Hard Metal (1mm-10mm/19pcs)  <https://www.amazon.com/gp/product/B07MZQMPMC/>`_
   Metric drill bits are hard to find at big box stores (I once spent hours on a  futile quest for an M4 drillbit) but come in handy when taping holes for the CNC and since so many CNC accessories use metric.

Screw Drivers and wrenches
``````````````````````````
* `Wera Kraftform 7440/41/42 Torque Screwdriver 0.3-6.0 Nm and Bit Set, 27-Piece <https://www.amazon.com/gp/product/B001555G80>`_
   I'm an engineer and like precision, with this screwdriver you can control the torque as you tighten each screw perfectly. While purely subjective they also feel awesome when using them.   

Squares
```````
* Insert Woodpeckers Squares links
* INSERT EMPIRE LINK
* INSERT HARBOR  FREIGHT LINK

Tape measures
`````````````
* `Fastcap PMMR-TRUE32 PMMR True32 5m, Metric/Metric Reverse measuring tape for 32mm system  <https://www.amazon.com/gp/product/B000GFHABG/>`_


Tap and Die Sets
````````````````
* `GEARWRENCH 75 Pc. Ratcheting Tap and Die Set, SAE/Metric - 3887 <https://www.amazon.com/gp/product/B000HBDW48/>`_
* <TODO: INSERT LINK TO HARBOR FREIGHT EQUIVALENT   
   
   .. note:  This is a great example of where Harbor Frieght is just fine.  If you are working mostly in wood a high quality set is likely overkill.  I had to retap several of the holes on my Mega V so having metric and imperial was a big help.

Measuring and Marking Tools
```````````````````````````
* `Woodraphic Professional Dual Function Vernier Calipers for Measuring and Marking  <https://www.amazon.com/gp/product/B07F1DKH2K>`_
* TODO - LINK TO BANGGOOD VERSION
* TODO - LINK TO WOODPECKER VERSION  
  .. note:: The Woodraphic tool is one of those tools that surprised me in just how often I use it.  This tool is great for helping ensure your racks are all evening spaced and for testing positioning of things.  

.. _123_blocks:

1-2-3 blocks
``````````````
* `LLDSIMEX Pair 1" x 2" x 3" Precision Steel 1-2-3 Blocks 23 Holes <https://www.amazon.com/gp/product/B07QWSL7TJ/>`_
   Used for jig making, testing square, CNC calibration, and a million other things depending on your creativity.

.. _feeler_gauges:

Feeler Gauges
`````````````
* `OEMTOOLS 25304 Gauge 12Bl Value Tap Feeler <https://www.amazon.com/gp/product/B000BYEQ3C/>`_
* INSERT HARBOR FREIGHT LINK
    Used for testing the thickness of a gap.  Very useful for getting consistent pinon spacing on the stepper motors, tramming the router, and identifying how much shimming is needed to square a portion of the Mega V.

Cutting Fluid
`````````````
* `Tap Magic 20004A Aluminum, 4 oz. <https://www.amazon.com/gp/product/B07CMNLYRL>`_
   If you are cutting aluminium extrusions on a miter saw or milling blocks of 6061 this is a great cutting fluid to use.
* INSERT HOME DEPOT LINK TO THREAD CUTTING FLUID


Section 2h: Grounding Aids
--------------------------

Ground loops as well as missing grounds while not a problem on every setup can cause drop out's mid-cut, as well as an inability to connect over USB to the CNC Controller.  Cutting certain materials like Acrylic and MDF will generate 
significant amounts of static electricity.  If you find you are failing cuts when working with these materials then you likely have a grounding issue.  If this starts happening there are a several potential solutions:

* Split the load between 2 or more electrical circuits ShopVacs tend to not play well with others when sharing a circuit.
* Shield all wires and earth ground at least 1 end of each. 
* Put a hub between the computer and CNC Controller.  Not all USB ports were created equally and a decent USB hub can smooth out a surprising number of issues.
* Use a USB cable with a ferrite bead 
* Use a USB Ground Isolator.


All of the following can help with these issues:

* `USB Cable with a Ferrite Bead <https://www.amazon.com/Tripp-Lite-Hi-Speed-Ferrite-U023-003/dp/B003MQ29B2/>`_
* `iFi iDefender+ External USB Audio Ground Loop Eliminator (A to A) <https://www.amazon.com/gp/product/B0849J33T9>`_
    USB Ground Loop Protection
*  `HiLetgo ADUM3160 B0505S 1500V USB to USB Voltage Isolator Module Support 12Mbps 1.5Mbps <https://www.amazon.com/dp/B07235PR4V>`_
* `StaticTek Banana Jack Outlet Plug Adapter | Universal Ground 3 Prong Outlet Earth Connection | ESD Control | Black Light Weight Unbreakable Plastic | 1 Piece | STI - DES - 09838 <https://www.amazon.com/gp/product/B071J61CSV/>`_
    Earth Ground Adapter 
* `Superior Electric EC183 9 Feet 18 AWG SJO 3 Wire 125 Volt Electrical Cord <https://www.amazon.com/gp/product/B004GUAJEM/>`_
    Grounded Power Cord for Dewalt Router


Section 2i: Wasteboard Accessories
----------------------------------

.. _tnuts:

T-Nuts
``````
* `Roll in M5 Spring Loaded T Nut for 20mm Series Aluminum Extrusions Pack of 50 <https://www.amazon.com/gp/product/B077MKCJRR/>`_
* `Slide-in M5 T Nut for 3030 Aluminum Extrusions Pack of 12 <https://www.amazon.com/gp/product/B085BYVDL2>`_
* TODO Roll in M5 Spring Loaded T Nut for 3030 Aluminum Extrusions

Threaded Inserts
````````````````
* `E-Z LOK 400-4 Threaded Inserts for Wood, Installation Kit, Brass, Includes 1/4-20 Knife Thread Inserts (5), Drill, Installation Tool  <https://www.amazon.com/Z-LOK-Threaded-Inserts-Installation/dp/B015CAPI54/>`_
* `E-Z Lok Threaded Insert, Zinc, Hex-Flanged, 1/4"-20 Internal Threads, 25mm Length (Pack of 50) <https://www.amazon.com/Z-Threaded-Hex-Flanged-Internal-Threads/dp/B002WC8TUW/>`_
* `E-Z Lok Threaded Insert, Zinc, Hex-Flanged, 1/4"-20 Internal Threads, 13mm Length (Pack of 100) <https://www.amazon.com/Z-Threaded-Hex-Flanged-Internal-Threads/dp/B002KT43MU>`_

Fences
``````
* `PwnCNC Wasteboard  Fence Guide  <https://pwncnc.com/purchase/ols/products/guide-set>`_
   Wasteboard fences can certainly be made (you own a CNC after all), but these are great for having a squared start position for your cuts.


Section 2i: Dust Control
------------------------

Proper dust collection is important when milling. Products like MDF produce a tremendous amount of dust when being milled.  That combination
can cause fires, and generates a lot of static when collected. :term:`CNC Controllers<cnc controller>` can be very suseptible to static 
build up and a grounded dust hose like this is a good part of a holistic approach to static management.

..  warning:: Dust from MDF, FR1 (PCB), Phenolic and a slew of other things consists of very fine particles that can cause long term lung damage. Whichever dust management system you use it is strongly advised that it be HEPA rated so the fine particles don't just blast out the dust port.  Dust control should always be paired with a proper respirator. Lungs are a terrible thing to waste.   

Cyclone Separator
`````````````````
  * ADD LINK TO ONEIDA
  * ADD LINK TO HOMEDEPOT ONE
  * ADD LINK TO FESTOOL

Dust Boots
``````````
  * `KentCNC Standard Dust Boot (Can be bought direct from MillRight for the same price) <https://www.kentcnc.net/nc/dust-shoes-standard-and-mini>`_
  * `Pwncnc Dustboot V2 <https://pwncnc.com/purchase/ols/products/dust-boot-v2>`_
  * `Kraken3d Dustboot <https://www.etsy.com/listing/773198870/dewalt-dwp611-dustboot-with-flexible>`_

Dust Collectors
```````````````
  * ADD LINK TO ROCKLER DUST COLLECTOR
  * ADD LINK TO HARBOR FREIGHT DUST COLLECTOR

Grounded Dust Hoses
```````````````````
* `2 1/2" x 50' CLEAR PVC DUST COLLECTION HOSE BY PEACHTREE WOODWORKING PW369 <https://www.amazon.com/gp/product/B001JBANYM/>`_

ShopVacs
````````
* ADD LINK TO RIGID SHOP ShopVacs
* ADD LINK TO FEIN
* ADD LINK TO FESTOOL


Section 2j: CNC Add-ons and Add-on Shops
----------------------------------------

Collets
```````
* Dewalt: `Precise Bits Precision Collets <https://www.precisebits.com/gateways/ColletsNutsHome.htm>`_
  Precision Collets reduce :term:`runout<Runout>` in a CNC which can cause inaccurate cuts as well as possible endmill breakage.  Collets come in various sizes and stocking specific ones for 1/8" or even 1/16" endmills is preferable to a reduction collet insert.
* Makita: INSERT LINKS
* ER: INSERT LINKS

Coolant Systems
```````````````
* `OriGlam Mist Coolant Lubrication Spray System for Metal Cutting Engraving Cooling Sprayer Machine for Air Pipe CNC Lathe Milling Drill <https://www.amazon.com/gp/product/B071DXGGP4>`_

Drag Chains
```````````
* `URBEST 15mm x 40mm Black Plastic Flexible Nested Semi Closed Drag Chain Cable Wire Carrier 1M for Electrical Machines 15mmx40mm <https://www.amazon.com/gp/product/B07WQ8P3PZ>`_
   This model is a little larger the the MillRight Drag Chain and gives a bit more room for the added size of shielded wires.

.. _iot_relay:

Power Control
`````````````
* `Fulton 110V Single Phase On/Off Switch with Large Stop Sign Paddle for Easy Visibility and Contact for Quick Power Downs Ideal for Router Tables Table Saws and Other Small Machinery <https://www.amazon.com/gp/product/B07SG75TZS/>`_
* `IOT Relay <https://www.amazon.com/gp/product/B00WV7GMA2>`_
      A power strip that has outlets that can be turned on and off by a relay closing.  These are commonly used for automativally turning on/off the CNC's :term:`Router` just before cutting begins.  


.. _aluminium_extrusion:

Wasteboard Reinforcement
````````````````````````
* `Aluminum Extrusion 48" (1220 mm) Clear Anodize Misumi Series 5 (20mm x 40mm) - 4 pack <https://www.amazon.com/gp/product/B079167LZ4/>`_
   Millright ships a single central cross brace for the T-Track Bed as part of the assembly kit. Several forum members and I have added 2 extra 1000mm long 2040 extrusions on either side of the included one to further support the bed.  
   This link is to a 4 pack of longer extrusion that I have bought and then cut down on a miter saw.  Extrusion has a million uses so extra never hurts.  Nothing says you can't just source 2 1000mm pieces though from 
   `Misumi <https://us.misumi-ec.com/vona2/mech/M1500000000/M1501000000/M1501010000/>`_, `80/20 <https://8020.net/>`_, or `Faztech <https://faztek.net/t-slottedaluminum.html>`_.  

.. figure:: Extra_bed_supports.jpg
         :width: 30%


Section 2k: CNC Repair and Replacement Parts
--------------------------------------------

Coupler Alternatives - Z-Axis 
`````````````````````````````
* `uxcell 6.35mm to 8mm CNC Stepper Motor JAW Shaft Flexible Coupling Coupler <https://www.amazon.com/gp/product/B00DCANRC8>`_

Loctite
```````
.. _loctite:

* Loctite
  * `Loctite 248 QuickStix 442-37684 9g Thread Treatment Stick <https://www.amazon.com/gp/product/B000132VH6/>`_
  * INSERT LINK TO LIQUID LOCTITE

If the pinons are slipping down the shaft of the stepper and blue loctite isn't enough then marine epoxy is a more permanent fix
* `J-B Weld 8272 MarineWeld Marine Epoxy - 2 oz. <https://www.amazon.com/gp/product/B000KKPFFA/>`_


Screws
``````

uxcell M3x35mm Thread Button Head Hex Socket Cap Screw Bolt 50pcs
https://www.amazon.com/gp/product/B01B1OD244/


uxcell M3x70mm Fully Thread Hex Socket Head Knurled Cap Screw Bolt Black 10pcs
https://www.amazon.com/gp/product/B01N3UVI74/


uxcell M4x12mm Machine Screws Hex Sock
et Round Head Screw 304 Stainless Steel Fasteners Bolts 20pcs
https://www.amazon.com/gp/product/B07Q3PXHVZ/


Stepper drivers alternatives
````````````````````````````

* `STEPPERONLINE Digital Stepper Driver 1.8~5.6A 20-50VDC for Nema 23, 24 Stepper Motor <https://www.amazon.com/gp/product/B074TBMC7N/>`_
* https://www.automationtechnologiesinc.com/products-page/kl-stepper-drivers/kl5056/?fbclid=IwAR1WmpWmxFA0UqM2xDiblJYAH9gS5jLUW2gCbR_czpnPi14KRwdbEdqnjeY
* https://www.stepper-store.com/product/digital-stepper-driver-1-85-6a-20-50vdc-for-nema-23-24-34-stepper-motor/?fbclid=IwAR3Or490m7iClHHKZOjOOC-mNEuxbtq89aimxLk26H1PWbssoOF7wm1zjvk
* https://www.omc-stepperonline.com/digital-stepper-driver-18~56a-20-50vdc-for-nema-23-24-34-stepper-motor-dm556t.html?fbclid=IwAR0Mifi4nC-F2McjOtrKxgyZm75PqIsOzE0q8na-JY6ef5ozj4BSLVXtHPM


Vendors with a wide range of parts
``````````````````````````````````

*  `Automation Technologies <https://www.automationtechnologiesinc.com/>`_

Section 2x: Work Holding
------------------------
* `Low Profile CNC T-Track Clamps - Set Includes 4 Clamps <https://www.etsy.com/listing/770341658/low-profile-cnc-t-track-clamps-set?ref=shop_home_active_1&crt=1>`_
* `Carbide3D Gator Tooth Clamps <https://shop.carbide3d.com/collections/workholding/products/gatortooth?variant=31475366461501>`_
* `Carbide3D Corner Square <https://shop.carbide3d.com/collections/workholding/products/carbide-corner-square-guides?variant=31487905988669>`_
* `Carbide3D Tiger Claw Clamp <https://shop.carbide3d.com/collections/workholding/products/tiger-claw-clamps?variant=31628957712445>`_
* `Kraken3d Low Profile CNC T-Track Clamps <https://www.etsy.com/listing/770341658/low-profile-CNC-t-track-clamps-set>`_
* INSERT LINK TO CNC Tape
* INSERT LINK TO CA GLUE and ACTIVATOR
* INSERT LINK TO GREENTAPE AND NYC CNC video



Section 2k: 3D Printing Accessories 
-----------------------------------

[ J&J Products ] M3 Brass Insert, 5 mm (Length), Female Thread, Heat Sink/Injection Mold Type, 100 pcs
https://www.amazon.com/gp/product/B07HKW7LKH/


.. _conductive_epoxy:

MG Chemicals 8331 Silver Epoxy Adhesive - High Conductivity, 10 min Working time, 14 g, 2 Dispeners
https://www.amazon.com/gp/product/B003BDMJSY/


Section 2l: Cabling Making Parts
--------------------------------

Connectors
``````````
* `10 Pcs 4 Pin Metal Male Female Panel Connector 16mm Thread GX16-4 Aviation Plug Connector(Silver Tone)  <https://www.amazon.com/gp/product/B07174LCGR/>`_
* INSERT  MOLEX LINKS
* INSERT THOSE MICROPHONE Connectors

Tools
`````
* `Ferrule Crimping Tool Kit - Sopoby Ferrule Crimper Plier (AWG 28-7) w/ 1800pcs Wire Ferrules Kit Wire Ends Terminals <https://www.amazon.com/gp/product/B07PJK2VNT/>`_
  Ferrules are metal tips that can crimp onto wire ends rather than putting bare wires into screw terminals.  While not needed, if you find yourself rewiring your control box then putting htese on everything is a nice to have.

Cables
``````

.. _18/2_shielded_wire:

**18/2 Shielded Wire for Homing Switches** 

* `Belden 5300FE 18/2 Shielded Control Cable 100 Ft  <https://www.amazon.com/Belden-5300FE-Shielded-Control-Cable/dp/B01LXO7H0M/>`_
* `PLTC3-18-1S-1  <https://www.automationdirect.com/adc/shopping/catalog/cables/bulk_multi-conductor_cable/instrumentation_cable/twisted_pairs_with_overall_shield/pltc3-18-1s-1>`_
* `C2G 29204 18 AWG Bulk Speaker Wire - Shielded, Plenum CMP-Rated, White Jacket (50 Feet, 15.24 Meters) <https://www.amazon.com/C2G-29204-Shielded-Speaker-CMP-Rated/dp/B007AS5Z0U>`_
* INSERT EBAY LINKS

.. _22/2_shielded_wire:

**22/2 Shielded Wire for Homing Switches** 

* `2-CONDUCTOR SHIELDED CABLE W/ DRAIN <https://www.allelectronics.com/item/2cs22/2-conductor-shielded-cable-w/drain/1.html?fbclid=IwAR32KdDzoko3_z_kiqKhAo7nth9T-GKre1hVHz-LOLUbvkA26zreAUhA3y4>`_

.. _18/4_shielded_wire:

**18/4 Shielded Wire for Stepper Motor Replacement Cables** 

* `Canare L-4E6S Star-Quad Microphone Cable by the Foot <https://www.markertek.com/product/l-4e6s-bk/canare-l-4e6s-star-quad-microphone-cable-by-the-foot-black>`_
* INSERT EBAY LINKS

.. _vfd_cable:

**16/4 VFD Cable**

* `VFD Cable: 16 AWG, cut to length (PN# VFDC-16-4B-1) <https://www.automationdirect.com/adc/shopping/catalog/cables/bulk_multi-conductor_cable/vfd_cable/vfdc-16-4b-1?fbclid=IwAR3pfOocF0NABDyuep8Z-Kky3Hthkz4L2cUy24mKZau29cPcow8ANTMlb_Q>`_
   When you buy a spindle they generally don't come with the power cord which you need to solder onto airplane connectors.  