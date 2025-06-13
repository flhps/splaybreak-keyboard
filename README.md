# SplayBreak

_A simple but versatile 36-key split ergonomic wireless keyboard._

---

![Model B](/images/splaybreak_model_b.jpg)
_Model B with MX switches and XDA keycaps_
![Model A](/images/splaybreak_model_a.jpg)
_Model A with MX switches and OEM keycaps_

This is a split keyboard, that is heavily inspired by my recent personal dive into the world of open mechanical split keyboards. At the time of writing, I have used these two models on an almost daily basis for over 6 months.

## Features

There are two models that use the same PCB and mostly the same build parts:

| Model                  | Hot Swap MX | Hot Swap Choc V1 | Gasket Mount | Battery | Magnetic Access Hatch | Nice Case Buttons |
| ---------------------- | ----------- | ---------------- | ------------ | ------- | --------------------- | ----------------- |
| [A](/build-guide-a.md) | ✅          | ⚠               | ✅           | 2000mAh | ✅                    |                   |
| [B](/build-guide-b.md) | ✅          | ⚠               |              | 500mAh  |                       | ✅                |

More information can be found in the individual build guides:

- [SplayBreak Model A](/build-guide-a.md)
- [SplayBreak Model B](/build-guide-b.md)

> [!WARNING]
> While the PCB accepts hot swap sockets for Choc V1 switches, the case dimensions are not tested with them.

## Design Rationale

A big focus was to keep this keyboard somewhat simple and cheap. That is why it uses the popular Pro Micro controllers and that limits the number of keys per side to 18 because we want to avoid having to solder diodes. The keyboards are wireless with massive batteries for easier daily use at home and on the go. Since the whole keyboard layout is in the firmware, these can also be used with devices such as phones or tablets. While screens can be cool, this design has none because they cost money and reduce battery life.

For flexibility (and cost reduction), the PCB is reversible. It means you need to order less and any PCB you have left can replace one that you accidentally destroyed. Also, the PCB has support for MX switches and Choc v1 switches. That would enable the use of this PCB for a super thin travel option.

There are only two thumb keys, because they would increase the design's footprint by a lot if they were to be positioned comfortably. The current inner thumb key is the resting position, meaning a third one would have to be even more toward the inside. However, I wanted to create a somewhat compact key arrangement and case.
Instead, the extra thumb key is moved to the pinky. This emulates the extra outer keys like tab or enter on a conventional keyboard an is intended to make it easier for people who frequently switch between conventional and split keyboards. It also makes switching from a conventional keyboard to this one easier.

This project features two different keyboard models, which only differ in assembly instructions and the provided case files, which are FDM-printable. I was never a big fan of the very gritty designs featuring lots of open electronics, so I designed some fully enclosed cases.

For repairability, model A has everything socketed, making error search and replacements easier. It is also built to improve sound through a gasket mount. Model B foregoes some of that and becomes more compact and arguably more stylish. There, the controller is soldered directly to the PCB.

## Firmware and Layout

Both models can use the same firmware. I have prepared a template that already contain a usable layout:

[zmk-config-splaybreak-template](https://github.com/flhps/zmk-config-splaybreak-template)

## Open Ideas and TODOs

- clean up the PCB and make it more aesthetic (transparent case?)
- create another model as a thin travel option with choc v1
- more in-depth build guides

## Development

Build ergogen in the `ergogen` directory:

```sh
ergogen --clean .
```

## Attributions

Big inspirations were:

- [TOTEM](https://github.com/GEIGEIGEIST/TOTEM)
- [Ferris Sweep](https://github.com/davidphilipbarr/Sweep)

The design uses ergogen footprints from [@ceoloide's ergogen PCB footprints](https://github.com/ceoloide/ergogen-footprints).
The reversible hotswap footprint for both MX and Choc is extracted from the [Lily58 Pro's](https://github.com/kata0510/Lily58) kicad file.

The [ergogen guide](https://flatfootfox.com/ergogen-introduction/) from FlatFootFox was very helpful.

And of course, this project would probably not exist without the excellent tool that is [ergogen](https://github.com/ergogen/ergogen).
