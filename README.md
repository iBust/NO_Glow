# no_glow means safer from device to router

## 4-step tutorial

### How to be the most safe and secure online.

*Some of these steps can be done on a regular home network and computers, but to build a secure (or ''anonymous'') configuration, you need to dedicate a second computer and a second router (ex. cheap Coreboot compatible Lenovo ThinkPad and a cheap Mango GL.iNet router)*

1. Device
     - Coreboot
     - ME_Cleaner & AMD PSP

2. OS
     - Qubes-Whonix
     - Tails
     - Others (Open or HardenedBSD, etc.)
  
3. Software
     - Invidious (Youtube)
     - Matrix Chat (register over Tor, etc.)
     - i2p
     - SOCKS5

4. Router
     - OpenWrt & DD-Wrt
     - Tomato (Fresh/Advanced)
     - DNSCrypt (for when non Tor, clearnet)
     - 2nd router, keep other as your
     - ufw (port for IME, AMDPSP has uncontrolled memory access,lot worst then the network)

5. Extras
     - Jellyfin (Open source ''Netflix/Plex'')
     - JMP.CHAT/FragmentTON/XMPP
     - Streamio
     - Emailwiz (lukesmith)
     - GrapheneOS (Pixel)
     - Monero
     - Tomato (Fresh/Advanced)
     - DNSCrypt (for when non Tor, clearnet)

# 1. **Device**

*For more info, see Bunnie's (OG XBOX Hacker) **Precursor** (https://www.youtube.com/watch?v=w8BA6_9HCzk) Mobile, Open Hardware, RISC-V System-on-Chip (SoC) Development Kit and **Novena** open source hardware laptop!*

https://precursor.dev/ (in stock)

https://www.crowdsupply.com/sutajio-kosagi/novena (no longer available)

## Corebooted Computer (from easiest to hardest)

### Why?

Intel

Coreboot, formerly known as LinuxBIOS, replace the closed source proprietary firmware (BIOS or UEFI) found in most computers with a lightweight firmware designed to perform only the minimum number of tasks necessary to load and run a modern 32-bit or 64-bit OS.

Since Coreboot initializes the bare hardware, it must be ported to every chipset and motherboard that it supports. As a result, coreboot is available only for a limited number of hardware platforms and motherboard models (mostly Lenovo Thinkpads & Chromebooks).

DEFCON 26 HARDWARE HACKING VILLAGE - Brian Milliron - Disabling Intel ME in Firmware https://www.youtube.com/watch?v=WJo8RsJeqxU

AMD

AMD PSP ... ''IME for AMD''

 AMDPSP has uncontrolled memory access,lot worst then the network)

### How?

Easiest way:

   *You can find devices with Coreboot (Skulls, Libreboot, Heads) on eBay or from System76, Purism, Nitro, FSF and more.*

Harder way:

Skulls pre-built coreboot image for Lenovo Thinkpad (t430, t440p, t530, w530, x230, x230t)
      
     https://github.com/merge/skulls

MrChromebox

     https://mrchromebox.tech
      
Libreboot (compatibility list)

     Servers (AMD, x86) 
     ASUS KFSN4-DRE motherboard
     ASUS KGPE-D16 motherboard
     
     Desktops (AMD, Intel, x86)
     Acer G43T-AM3
     Apple iMac 5,2
     ASUS KCMA-D8 motherboard
     Dell Precision T1650 (easy to flash without disassembly)
     Gigabyte GA-G41M-ES2L motherboard
     HP Elite 8200 SFF/MT (HP 6200 Pro Business probably works too) (easy to flash without disassembly)
     HP Elite 8300 USDT (easy to flash without disassembly)
     Intel D510MO and D410PT motherboards
     
     Laptops (Intel, x86)
     Apple MacBook1,1 and MacBook2,1 (2,1 flashable without disassembly)
     Dell Latitude E6400, E6400 XFR and E6400 ATG, all with Nvidia or Intel GPU (easy to flash, no disassembly, similar hardware to X200/T400)
     Dell Latitude E6430 (Intel GPU (easy to flash, no disassembly)
     HP EliteBook 2170p (socketed flash IC)
     HP EliteBook 2560p
     HP EliteBook 2570p
     HP EliteBook 8470p
     HP EliteBook Folio 9470m
     Lenovo ThinkPad R400
     Lenovo ThinkPad R500
     Lenovo ThinkPad T400 / T400S
     Lenovo Thinkpad T420 (no install docs yet)
     Lenovo ThinkPad T420S (no install docs yet)
     Lenovo ThinkPad T430 (no install docs yet)
     Lenovo ThinkPad T440p
     Lenovo ThinkPad T500
     Lenovo ThinkPad T530 / W530 (no install
     Lenovo ThinkPad T60 (with Intel GPU) (easy to flash without disassembly)
     Lenovo ThinkPad W500
     Lenovo ThinkPad W541 (no install docs yet)
     Lenovo ThinkPad X200 / X200S / X200 Tablet
     Lenovo Thinkpad X220
     Lenovo Thinkpad X220t
     Lenovo ThinkPad X230
     Lenovo Thinkpad X230
     Lenovo Thinkpad X230t
     Lenovo ThinkPad X301
     Lenovo ThinkPad X60 / X60S / X60 Tablet (easy to flash without disassembly)
     
     Laptops (ARM, with U-Boot payload)[link]
     ASUS Chromebook Flip C101 (gru-bob)
     Samsung Chromebook Plus (v1) (gru-kevin)
      
Libreboot image maker

     https://notabug.org/libreboot/lbmk

Coreboot
     
     https://github.com/coreboot/coreboot

**ME_CLEANER**

Intel

     Most of the tools like Coreboot, Libreboot, Skulls & Heads will clean the IME, read the instruction when installing these (and some will also extract/leave the needed closed source blobs that are required for the computer initialisation)

AMD

     Phenom II are the strongest CPU before 2013 when AMDPSP came into existance. You can desactivate AMDPSP

## 2. The OS
   Of course Winblows (spyware) is not a secure and anonymous OS.
   
## 3. Software

## 4. Router

## 5. Extras

Inside your OS, you cannot do everything and open a browser and open all that javascript crap. 
Invidious


100. First list item
     - First nested list item
