# Build Guide: SplayBreak Model B

![Model A](/images/splaybreak_model_a.jpg)

This version is my original design with a massive PlayStation controller battery and a gasket mount. It also has enough space for foam or other sound-improving material in the bottom.

My personal build uses Gateron Oil King switches and Cherry profile key caps to create a satisfying and comfortable every-day setup.

## PCBs

You can order your PCB at services like JLCPCB or PCBWay. Download the gerbers ZIP archive from the [pcb](./pcb/) directory and upload them to the service.

Important Parameters:

- 1.6mm thickness
- 2 layers

Remember that 2 PCBs make 1 keyboard.

## Parts

These are the parts required for one Keyboard consisting of two halves. As a reference, I included rough pricing as of 2025 (worst-case pricing for minimum purchasable quantity). If you already have supplies, this may be much cheaper:

- 2x PCB (ca. 18€)
- 1x 3D printed model A case parts for left and right sides (ca. 2€ in material)
- 2x Pro Micro compatible controller with Bluetooth (ca. 12€)
- 4x 2.54mm pitch header row female (ca. 2€)
- 48x pins harvested from 4 or 5 pin RGB(W) headers by removing the plastic (ca. 2€)
- 2x 3.7v 2000mAh Sony PS4 controller battery pack with 2 pin JST PH 2.0mm plug (ca. 13€)
- 36x Kailh MX Hot Swap sockets (ca. 6€)
- 36x MX switches of preferred type (ca. 25€)
- 36x MX compatible keycaps (ca. 25€)
- 2x MSK-12C02 SMD toggle switch (ca. 2€)
- 2x EVQPUC02K SMD tactile switch (ca. 2€)
- 2x 2 pin JST PH 2.0mm housing (ca. 1€)
- various M2 standoffs to adapt to needed length depending on gasket (ca. 4x 22mm and 4x 18mm) (ca. 8€)
- 16x M2x6 countersunk screws (ca. 2€)
- 1x sheet of 3 mm poron foam (ca. 5€)
- 4x 6x3mm magnet (ca. 6€)
- 8x rubber feet (ca. 2€)

Total cost for building one keyboard is around 133€ and gets cheaper per unit if you build multiple.

For more information on the slightly unconventional controller socketing, consult this excellent [guide](https://github.com/joric/nrfmicro/wiki/Sockets#machine-pin-socket).

Optional:

- poron switch stickers for sound dampening
- painter's tape for tape modding
- some more foam or eraser putty for the bottom of the case

And of course you need solder supplies.

## Assembly

Take two PCBs mark opposing sides as the top side. Then, for each PCB:

1. Solder hot swap sockets on the bottom side.
2. Solder the toggle switch as power switch and the tactile switch as reset button. Put both on the bottom side.
3. Break the header rows to a length of 12 and solder the header rows for the controllers to the bottom side of the PCB. Put a piece of painter's tape over the sockets to prevent solder from dripping down. Lay the controller on the sockets such that the processor chip faces the PCB and put in all the pins, forcing them through the painer's tape. Then, solder the pins to the controller. Cut off the remaining length of the pins to keep the controller as flat as possible. Remove the painter's tape. Bridge the solder pads on the top side.
4. Solder the JST housing as a connection point for the battery on the bottom side. Bridge the solder pads on the top side.
5. Glue the magnets into the round recesses in the access hatches and frames.
6. Put standoffs into the 4 channels of the case's bottom part and screw them in from the bottom. Put the middle case part in the bottom one.
7. Cut out a strip of poron foam for each recess in the case's bottom and top part and place them in there.
8. Put the case's key plate on the PCB and insert switches to connect them.
9. Plug the battery connector in and lay the battery in its compartment in the case's bottom. Then lay the key pate (and PCB) with its tabs on the poron foam.
10. Carefully place the case's top part on the bottom part without the poron strips falling out. Secure the case by screwing in the top screws.
11. Put some rubber feet under the bottom plate.
