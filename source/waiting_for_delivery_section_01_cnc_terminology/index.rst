Section 01: CNC Terminology
===========================

Section 1a: Introduction
------------------------

.. figure:: welcome-iszvda.jpg
         :width: 75%

         [#f1]_

Congratulations you just spent thousands of dollars on a super heavy lump of metal. Now What? You are embarking on quite the adventure as you learn how to use the Mega V to make chips and hopeful products for your own use and for sale.  
The CNC world speaks its own dialect of english and learning this can be quite intimidating to newcomers.  This section hopes to demystify the major terms that come up on the Forums that confuse new users.  This is by no means a complete 
list but does give you enough to get started.

.. warning::  The CNC world is heavily based in the metric system.  Be prepared to abandon imperial measurements (aka Freedom Units) for many tasks.

Section 1b: The Glossary
-------------------------

.. glossary::

   Axis
      * X-Axis - Defines the Side to Side travel of the CNC.  X- is to the Left, X+ is to the Right.
      * Y-Axis - Defines the Front to Back travel of the CNC.  Y- is to the Front, Y+ is to the Back.
      * Z-Axis - Defines the Up and Down travel of the CNC.  Z- is Downward, Y+ is Upward.
      * A-Axis/4th Axis - A rotational Axis the pivots around the X-Axis. A+ is Clockwise, A- is Counter Clockwise
      * B-Axis/5th Axis - A rotational Axis the pivots around the Y-Axis. B+ is Clockwise, B- is Counter Clockwise.  The MillRight CNC does not have a 5th Axis option

   bCNC
      An advanced opensource and free GCode Sender that works for 3 Axis CNC's with special features for milling PCBs. See  :ref:`BCNC`

   Carbide motion
      A Commercial but freely available GCode Sender designed for the Carbide3D Nomad and ShapeOKO platforms.  With some effort it can work for the Mega V.

   Chatter
      The telltale noise you will hear, espically when cutting aluminum if your speeds/feeds are off and the cutter is not able to smoothly remove matieral resulting in poort finish quality and a soon to break endmill.

   Chip Load
      The amount that each flute cuts during a single revolution of a cutting tool.

   cnc controller
   CNC Controller
      The embedded computer that communicates with the g-code sender to control the actual electronics of the CNC Machine.  The Mega V uses an Arduino Uno running GRBL 1.1 for its 3-Axis machine and the 4-axis machine uses an Arduino Mega 
      with a customized version of GRBL 1.1.  This board can be replaced with many commercial alternatives such as Mach 3, Mach4, Masso, geckodrive, uccnc, openbuilds blackbox and many others.

   CNCJS
       A popular opensource and free GCode Sender that works for 3 Axis CNC's, runs well on the Raspberry Pi3/4 and has dedicated tablet interfaces. See  :ref:`CNCJS`

   collet
       Mounted in a Router or spindle and used to hold the shank of the endmill.  Imperial Collets commonly come in 1/8", 1/4" and 3/8" for a Dewalt Router.  Metric equivalents are prefaced with ER.  An ER11 is equivalent to 1/4" and an ER20 is equivalent to 1/2".

   D.O.C.
   Depth of Cut
      This along with Speeds and Feeds are what CNCing is all about.  Depth of cut is how far into the matieral the endmill will bite with each pass.  With the right setting the Mega V can cut through almost anything 
      but the harder a material the smaller the DOC and thus longer time to accomplish a stage of the project.  See earlier Time is Money and always remember some jobs should be outsourced to save time!

   Easel
      A Freely available but commercial combination CAD, CAM, and gcode sender.  This works fine with the Mega V and is very easy to use.

   endmill
   EndMill
      * Compression - Compression Spiral Router bits have an upcut and downcut geometry to give you the cleanest cut on both the top and bottom side of the material.  Compression Router Bits are great for plywood or laminate sheet goods.
      * Upcut - The angle of the cutting flutes will push the chips out of the cutting path but can leave a rough top to the cut depending on materials.
      * DownCut - The angle of the cutting flutes pushing the chips down into the hole which can prevent tearout in thinner materials.  The top of the cut is generally very clean while the bottom can be more messy making it excellent for through cuts as well as shallow dados, rabbets, and visible slots.
      * BallNose - Used for milling contoured surfaces, slotting, pocketing and 3D carving.  The smaller the tip diameter the finer the detail in the 3D carve at the cost of increased cutting time. A good strategy is to do a roughing pass with a larger endmill and then use a ball nose for finishing passes.
      * V-Bit - Used to Cut decorative 'V' grooves and lettering on signs, etch acrylic, and carve chamfers into edges.

   flutes
   Flutes
      * Single Flute - Designs are used for high-speed machining and high-volume material removal.
      * Double Flute/Two Flute -  Have the most amount of flute space. They allow for more chip carrying capacity and are used primarily in slotting and pocketing nonferrous materials
      * Triple Flute/Three Flute - Have the same flute space as two flutes, but also have a larger cross-section for greater strength. They are used for pocketing and slotting ferrous and nonferrous materials
      * Four Flute/ Quad Flute - Allow for faster feed rates, but due to the reduced flute space, chip removal may be a problem. They produce a much finer finish than two and three flute tools. Ideal for peripheral and finish milling [#f3]_


   gcode
   g-code
      The programming language of CNC machines that controls how and where the CNC machine will move. G-Codes are not universally standardized 
      although there are many commonalities between machine types.  The full set of g-codes used by the Mega V are located at https://github.com/gnea/grbl/wiki/Grbl-v1.1-Commands . A future section will be added to this 
      document with a overview of g-code. Be aware though that all gcode senders have a console buried in their user interface that allows you to enter raw g-code to control the machine.  This can be handy for reseting alarm 
      states where entering *$x* will reset the system. Futher reading is at https://howtomechatronics.com/tutorials/g-code-explained-list-of-most-important-g-code-commands/ this article is generic so make sure a command is on 
      the GRBL list in the first link.

   g-code senders
   gcode senders
     Historically the hardware that runs the CNC Controller were extremely basic. There wasn't enough memory to load a full g-code program. As a result specialized computer programs are used to transfer chunks 
     of g-code to the controller to execute in stages. In the Mega V world you'll use UGS (universal g-code sender), CNCJS, OpenBuilds Control, picsender, bCNC, easel, or carbide motion (with hackery) to send gcode 
     to the controller. Gcode senders are finicky programs with many being open source (aka freely made by volunteers) so quality can vary.

   GRBL
      Controllers are the "brains" of the machine and are what takes in the instructions in g-code and translates them into X/Y/Z/A movement in the stepper motors. There many types of controllers 
      on the market that can be used by macbines. GRBL is open source/free and popular with hobby level machines.  GRBL was designed to use low cost Arduino boards as its microprocesser which does
      add some limits on functionality due to memory and processing constraints.  3d printers tend to use MARLIN as their controller. Commercial machines use a mix of systems but you will regularly
      see MACH3, MACH4, ACORN, LINUXCNC, and MASSO referred in YouTube Videos and Forum posts. All of these cost money and some require standalone computers while others like Masso are all in one systems.
      Lastly, it is possible to retrofit some of these other control systems into a Mega V if your projects require it.

   Home
      CNC's use the Cartisian Coordinate system of X/Y/Z axes to describe the location in space of the cutting head.  The **home** position is typically the back left corner of the CNC machine with the cutting head at the 
      maximum height of travel.  The following figure shows the 3 Axes and how movement occurs.  Please take note of the directions of X-/X+ Y-/Y+ Z-/Z+ as these labels are used in most gcode senders to control manual movements.

      .. figure:: coordinate_system.gif
         :width: 75%

         [#f2]_

   Homing
      The act of moving the router/spindle head of the CNC to the Home position.

   homing switches
      A mechanical device located at the home position of each axis that when impacted by the CNC's motion signals to the CNC Controller to cease travel in that direction and to note it is the zero point.
   
   IPM
      Inches per Minute: Number of inches the cutter passes through the workpiece in one minute.

   OpenBuilds Control
      A popular opensource and free GCode Sender that works for 3 Axis CNC's See  :ref:`OPENBUILDS_CONTROL`

   Rapids
      Moving at maximum acceleration to a given point.  A common selling point is howfast a machines rapids are.  Time is money, so faster is good but also adds strain on the machine and can shake it and the table apart if you go too nuts.

   RPM
      Revolutions per Minute: How many revolutions the cutter has in one minute.

   Router
      A device used on hobby grade CNC machines as the cutting head. The Mega V was designed to use a `Dewalt DWP611 <https://www.dewalt.com/products/power-tools/routers-planers-and-joiners/routers/114-hp-max-torque-variable-speed-compact-router/dwp611>`_ compact router.  
      
      The following table covers the Dewalt router speeds:

      +--------------+-----------------+
      | Dial Setting | Approximate RPM |
      +==============+=================+
      |      1       |      16,000     |
      +--------------+-----------------+
      |      2       |      18,200     |
      +--------------+-----------------+
      |      3       |      20,400     |
      +--------------+-----------------+
      |      4       |      22,600     |
      +--------------+-----------------+
      |      5       |      24,800     |
      +--------------+-----------------+
      |      6       |      27,000     |
      +--------------+-----------------+

      While not as common on the Mega V the `Makita RT0701CX7 1-1/4 HP Compact Router Kit <https://www.amazon.com/gp/product/B00HAQMHEO/>`_  Speeds are:
      
      +--------------+-----------------+
      | Dial Setting | Approximate RPM |
      +==============+=================+
      |      1       |      10,000     |
      +--------------+-----------------+
      |      2       |      12,200     |
      +--------------+-----------------+
      |      3       |      17,400     |
      +--------------+-----------------+
      |      4       |      22,000     |
      +--------------+-----------------+
      |      5       |      27,000     |
      +--------------+-----------------+
      |      6       |      30,000     |
      +--------------+-----------------+


   Runout
      Runout is a rotation inaccuracy which occurs when the tool is no longer aligned with the main axis. In drilling applications, this can result in a bore diameter that is actually larger than the drill’s nominal diameter

   Speeds and Feeds
      The art and science of using a CNC machine centers around the paired concepts of speeds and feeds and their cousin depth of cut.  Speeds refer to how many RPM's the rotational cutter is moving at.  Feeds are how fast the CNC machine is pushing the cutting head through the matieral.  When the two work together you will get perfect cuts.  When they are set wrong you will get chatter, broken end mils, smoke, and profanity.

   Spindle
      Serve the same purpose as a router in that they spin the cutting device at high speed.  They are much larger and heavier but offer much greater control of rotational speed with the added benefit of being incredibly quiet.
      Air Cooled - One of 2 flavors of spindle.  As the device spins it generates heat, to counter act this the rotational head uses a built in head to stay cool.  This adds to the base noise level but still is not as loud as a compact router.
      Water Cooled - The second of 2 flavors of spindle. As the name implies water cooled use liquid coolant (don't use water it grows bacteria) to draw heat out of the device as it rotates.  Water cooled spindles have added complexity to setup but are essentially silent when operating with the only noise being that of the cutter going through matieral.

   SFM
      Surface Feet per Minute: This is the cutting speed of the end mill in the United States. It is the number of feet per minute that a given point on the circumference of a cutter travels per minute.

   Tram
      Tram is the squareness of your mill head to the table

   Tram Arm
      A device that extends out from the router/spindle and can be used to verify squareness a fixed distance out from the router.  The longer the tram arm the better for ensuring a truly flat machine.

   Tramming
       The act of adjusting the mill head to be square. There is tram parallel to the x-axis, and tram parallel to the y-axis (sometimes called “nod”). 
       https://www.cnccookbook.com/tramming-milling-machine-tool-indicator/#:~:text=Tram%20is%20the%20squareness%20of,designed%20to%20cut%20at%20angles

   UGS
   Universal G-Code sender
      The default g-code sender used with the Mega-V.  See :ref:`UGS` for more details.

   VFD
      Spindles required the use of a VFD (Variable Frequency Drive) to function. These VFDs are also called spindle inverters. The VFD takes the power from the wall and creates a frequency with voltage and current to spin the spindle. The frequency can be controlled to control the RPM of the spindle.
   

.. note :: Please note that aditional terms can be found at: https://www.cnccookbook.com/cnc-dictionary/


Section 1c: The Math
--------------------

CNC Milling isn't an artform all endmills come with data on optimum cutting parameters that can be used in CAM.  Keep in mind that the
optimum may also assume a $250,000 Tormach CNC is doing the cutting so you do need to adjust if the math is more than a Mega V can handle.

The Key formulas are:

Revolutions per Minute(RPM) = SFM x 3.82 ÷ Tool Diameter

Inches per Minute(IPM) = RPM x # of Flutes x Chip Load

Chip Load = IPM ÷ RPM x # of Flutes

Surface Feet per Minute(SFM) = .262 x Tool Diameter x RPM


FootNotes:

.. [#f1] Source http://https://makeameme.org/meme/welcome-iszvda
.. [#f2] Source https://www.dlsweb.rmit.edu.au/Toolbox/furnishindustry/toolbox/shared/resources_mw/techniques/cnc_prog/cartesian.htm
.. [#f3] Liberally borrowed from Source https://www.mscdirect.com/basicsof/end-mills
