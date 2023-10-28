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
     - Monero (VPS, CoinCards, etc.)
     - Tomato (Fresh/Advanced)
     - DNSCrypt (for when non Tor, clearnet)

# 1. **Device**

*For more info, see Bunnie's (OG XBOX Hacker) **Precursor** (https://www.youtube.com/watch?v=w8BA6_9HCzk) Mobile, Open Hardware, RISC-V System-on-Chip (SoC) Development Kit and **Novena** open source hardware laptop!*

https://precursor.dev/ (in stock)

https://www.crowdsupply.com/sutajio-kosagi/novena (no longer available)

## Coreboot

### Why?

Intel

Coreboot, formerly known as LinuxBIOS, replace the closed source proprietary firmware (BIOS or UEFI) found in most computers with a lightweight firmware designed to perform only the minimum number of tasks necessary to load and run a modern 32-bit or 64-bit OS.

Since Coreboot initializes the bare hardware, it must be ported to every chipset and motherboard that it supports. As a result, coreboot is available only for a limited number of hardware platforms and motherboard models (mostly Lenovo Thinkpads & Chromebooks).

DEFCON 26 HARDWARE HACKING VILLAGE - Brian Milliron - Disabling Intel ME in Firmware https://www.youtube.com/watch?v=WJo8RsJeqxU

AMD

AMD PSP ''aka IME for AMD''

 AMDPSP can have uncontrolled memory access and many things even worst then even full network stack access.

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

## **ME_CLEANER**

### Why ?

The Intel Management Engine (ME), also known as the Intel Manageability Engine,[1][2] is an autonomous subsystem that has been incorporated in virtually all of Intel's processor chipsets since 2008.[1][3][4] It is located in the Platform Controller Hub of modern Intel motherboards.

The Intel Management Engine always runs as long as the motherboard is receiving power, even when the computer is turned off. This issue can be mitigated with deployment of a hardware device, which is able to disconnect mains power.

**Google**

As of 2017, Google was attempting to eliminate proprietary firmware from its servers and found that the ME was a hurdle to that.

**Dell**

In December, Dell began showing certain laptops on its website that offered the "Systems Management" option "Intel vPro - ME Inoperable, Custom Order" for an additional fee. Dell has not announced or publicly explained the methods used. In response to press requests, Dell stated that those systems had been offered for quite a while, but not for the general public, and had found their way to the website only inadvertently.[96] The laptops are available only by custom order and only to military, government and intelligence agencies.

### How ?

       Most of the tools like Coreboot, Libreboot, Skulls & Heads will clean the IME, read the instruction when installing these (and some will also extract/leave the needed closed source blobs that are required for the computer initialisation)

AMD PSP

Intel's main competitor AMD has incorporated the equivalent AMD Secure Technology (formally called Platform Security Processor) in virtually all of its post-2013 CPUs.

     Phenom II are the strongest CPU before 2013 when AMDPSP came into existance. You can ''desactivate'' AMD PSP in the BIOS, but source code is closed. It could have even worst than a full network stack accesss (like uncontrolled memory access)
## 2. The OS

- Qubes-Whonix

Edward Snowden OS recommandation

https://twitter.com/Snowden/status/781493632293605376

https://twitter.com/snowden/status/941020119609892864 )

          https://www.qubes-os.org/

### Why ?

Secure Compartmentalization
Qubes brings to your personal computer the security of the Xen hypervisor, the same software relied on by many major hosting providers to isolate websites and services from each other. Learn more


Operating System Freedom
Can't decide which Linux distribution you prefer? Still need that one Windows program for work? With Qubes, you're not limited to just one OS. Learn more


Serious Privacy
With Whonix integrated into Qubes, using the Internet anonymously over the Tor network is safe and easy. Learn more

### How ?

          https://www.qubes-os.org/doc/installation-guide/
   
## 3. Software

## 4. Router

## 5. Extras

Inside your OS, you cannot do everything and open a browser and open all that javascript crap. 
Invidious


100. First list item
     - First nested list item
