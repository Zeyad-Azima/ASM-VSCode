# ASM-VSCode
VSCode Configuration files to easily compile, debug &amp; run Assembly codes using system (Linux) utilities

# ARM
- Install the needed packages:
```
sudo apt-get install gcc-arm-linux-gnueabihf gcc-aarch64-linux-gnu gdb-multiarch qemu-user-static qemu-user
```
- Install [Arm Assemmbly Syntx support](https://marketplace.visualstudio.com/items?itemName=dan-c-underwood.arm) extention for `VSCode`
- Move/add `tasks.json` & `keybindings.json` files to `.config` folder related to `VSCode`
## Usage
Now, For usage don't forget to name your `ASM` file with the `.s` exetantion which is related to `ARM`:
- `CTRL+SHIFT+1`: build 32-bit `ARM` for remote debugging using `gdb-multiarch` & `qemu` (`Works on non-arm architecture also`).
- `CTRL+SHIFT+2`: build 64-bit `ARM` for remote debugging using `gdb-multiarch` & `qemu` (`Works on non-arm architecture also`).
- `CTRL+SHIFT+L`: build `ARM` for your device architecture for local debugging using `gdb-multiarch`.
- `CTRL+SHIFT+R`: build `ARM` for your device architecture and run it.
