# Build Guide: SplayBreak Model B

![Model B](/images/splaybreak_model_b.jpg)

This version is a more stylish variant intended for travel. It is a little lighter and more compact, but has a smaller battery. Still, it should last weeks on one charge.

My personal build uses silent TTC Frozen V2 switches and XDA profile keycaps to create a compact office and travel keyboard.

## PCBs

You can order your PCB at services like JLCPCB or PCBWay. Download the gerbers ZIP archive from the [pcb](./pcb/) directory and upload them to the service.

Important Parameters:

- 1.6mm thickness
- 2 layers

Remember that 2 PCBs make 1 keyboard.

## Parts

These are the parts required for one Keyboard consisting of two halves. As a reference, I included rough pricing as of 2025 (worst-case pricing for minimum purchasable quantity). If you already have supplies, this may be much cheaper:

- 2x PCB (ca. 18€)
- 1x 3D printed model B case parts for left and right sides (ca. 1€ in material)
- 2x Pro Micro compatible controller with Bluetooth (ca. 12€)
- 2x 3.7V 500 mAh LiPo battery model 402030 with 2 pin JST PH 2.0mm plug (ca. 4€)
- 36x Kailh MX Hot Swap sockets (ca. 6€)
- 36x MX switches of preferred type (ca. 25€)
- 36x MX compatible keycaps (ca. 25€)
- 2x MSK-12C02 SMD toggle switch (ca. 2€)
- 2x EVQPUC02K SMD tactile switch (ca. 2€)
- 2x 2 pin JST PH 2.0mm housing (ca. 1€)
- 8x M2x6 countersunk screws (ca. 2€)
- 8x rubber feet (ca. 2€)

Total cost for building one keyboard is around 100€ and gets cheaper per unit if you build multiple.

Optional:

- poron switch stickers for sound dampening
- painter's tape for tape modding

And of course you need solder supplies.

## Assembly

Take two PCBs mark opposing sides as the top side. Then, for each PCB:

1. Solder hot swap sockets on the bottom side.
2. Solder the toggle switch as power switch and the tactile switch as reset button. Put both on the top side.
3. Solder the controller on the top side with the USB port toward the PCB edge. Sandwich the included header pin rows between the controller and the PCB with the controller being upside down. The header pin row creates the necessary clearance for the USB port. After soldering, cut off the remaining pin length on top and bottom (max 0.5mm left standing).
4. Solder the JST housing as a connection point for the battery on the top side.
5. Put on the case's key plate and put in switches to connect it to the PCB.
6. Put the battery in the case top's compartment. Optionally secure it with some non-conductive tape.
7. Plug the battery connector in and insert the case's power switch in the top case cutout. Put the PCB assembly into the case top without crushing the Battery cable and without shearing off the power switch. This a bit tricky, so take your time.
8. Close the case by inserting the case's bottom plate and screw the 4 screws directly into the plastic.
9. Put some rubber feet under the bottom plate.
