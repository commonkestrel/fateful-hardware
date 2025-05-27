# Fateful Journal

This is the journal for the hardware version of [fateful](https://github.com/commonkestrel/fateful)!

## May 26, 2025

I worked on putting together a BOM for the control circuit!

![logisim implementation of the control circuit](./control.png)

This is mostly so I know what components to use when making the actual circuit later down the line.
Something that turned out really nice is that the program counter can be entirely isolated on it's own circuit,
since it fully utilizes the components required.

There are a couple components that were a little more difficult to decide between, such as the 74HC173 vs 74HC377 vs 74HC573,
but I settled on the 173 and I'll just double up as these are 4-bit registers.
Lots of reading through datasheets for this update, sorry!
I also ended up needing a lot more inverters than I though,
since most logic inputs on registers and buffers and such are inverted.

Overall, the control circuit seems like it'll cost around $13.18, which is a relatively good price!
Keep in mind though that I already have the EEPROM's on hand,
so without those it would be quite a bit more expensive.

**Total time spent: 4h**
