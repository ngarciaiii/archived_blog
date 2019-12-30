---
layout: post
title: "CompTIA A+ Safety and Hardware Part 1"
date: 2019-03-19 09:08:30 -0400
categories: CompTIA
tags: [A+]
comments: true
---

# Safety first

When working with computer hardware can be dangerous when it is plugged. I can't think of any reason to assemble or disassemble computer while it is plugged. So <b>NEVER LEAVE IT PLUGGED</b> when working with computer and its components. If it was already plugged, unplug and wait at least 5 minutes before upgrading/replacing component. When ordering components, they usually come in `antistatic bags`, typically made from plastic <i>polyethylene terephthalate</i> (PET) to protect components that are sensitive to electrostatic discharge. It works by being slightly conductive, forming what is known as <b>Faraday Cage</b>.

![antistatic bag](/public/img/A+/antistatic_bag.jpg){: .center-image }

It is recommended to wear `ESD (electrostatic discharge) strap` when taking components out of the antistatic bags and installing into computer. There are many types, but wrist strap is the most common. Follow the same example as the image below, clip onto metal frame of the computer case.  

![ESD_strap](/public/img/A+/ESD_strap.png){: .center-image }

I suspect those are the most important to know. There are other ways to prevent electrical charges like `ESD mat`, where you place computer equipments on, or another way is `Self-grounding` where you touch the any non-computer equipment metal object to let go of electrical charges from your body before resumes working on components.

Electrical fire rarely occurs but when it does, be sure to use the right fire extinguisher. It should have a C letter marked on it. `Class C fire extinguisher`, easy to remember C for computer.

Worn out computer components like batteries and or CRTs do not go into trash. They should be recycled to prevent soil and water contamination. `CRTs (Cathode-ray tube)` are huge heavy <b>stone age computer and television monitors</b>.

# Hardware Part 1

I ordered all parts and built my PC. Check out [PCPartPicker][PCPartPicker] if you are interested in building a PC. I remember that the first thing I looked to buy was a `computer case`, `enclosure`, or some people would say `Desktop PC Tower`. It encases as a protector of all parts together. There are different sizes depending on the size of motherboard and CPU cooler. The sizes are not limited to as displayed in the figure below.

*Figure: Sizes of Towers*
![desktop tower](/public/img/A+/pctowers.png){: .center-image }

Full and or mid towers are the most common because people intend to get ATX motherboard. Notice XL-ATX, ATX, EATX, mATX, ITX, and Mini-ITX listed under towers in the image, these are just names of `motherboard` designs which are known as `form factors` that have their own specifications like the <b> dimensions, power supply type, locations of mounting holes, number of ports on the back panel, etc</b>. Nevermind the "bays" listed, they are what hold disk drives.

*Figure: Types of Motherboards*
![mobos](/public/img/A+/mobos.jpg){: .center-image }

`Motherboard` is one of the most important hardwares. It serves as a backbone for entire computer system which is why some people call it either `main board`, or `system board`. <b>FUN FACT:</b> Apple call it `logic board`. PC builders would call it `mobo` for short. Mobo has some components soldered in like <b>RAM slots and driver connectors which are irreplaceable</b>. These sockets/slots ready to be pinned in. There are few components like <b>CPU and CMOS battery that are replaceable</b>. Components will be detailed after the image of sizes of motherboards below. Take a closer look on a mobo below.

*Figure: Motherboard Form Factor*
![mobospecs](/public/img/A+/mobospecs.png){: .center-image }

## CPU

`CPU` is short for <b><i>Central Processing Unit</i></b>, a silicon microchip that processes all instructions from computer's hardware and software. The CPU has two primary components: <b><i>control unit (CU)</i></b> and <b><i>arithmetic logic unit (ALU)</i></b>. CU fetches instructions from memory, decodes, and executes them, calling on the ALU to perform arithmetic and logic operations when necessary.

![CPU](/public/img/A+/CPU.jpg){: .center-image height="300px" width="auto" }

The speed of CPU is in megahertz or `MHz`, number of million of instructions or cycles the CPU can process in a second. The number of `cores` is the best way to determine the speed CPU has. `Core` is an independent processor embedded onto CPU. Multiple cores allow the CPU to process multiple instructions at once. Typically newer laptops have 6 cores, but I believe most of people who use 10 year old or fair-priced laptops have 4 cores.

`Hyperthreading` is an alternative to having multiple cores but will not equal to at least dual cores cpu. It <b>simulates two logical processors on one physical processor</b> by using registers to overlap two instruction streams. It is about 30% gain in performance and it can be enabled by going through system BIOS. Not all CPU support hyperthreading.

`CPU cache` is fast memory used to process of instructions or data. Instruction cache speeds up the executable instruction fetch. Data cache speed up data fetch and store. Data caches are stored in hierarchy starting with Level 1  (L1), its a small high speed cache. Subsequently like L2, L3, and so on cache is slower and larger than L1.

There are <b>32-bit</b> and <b>64-bit processors</b>. When people talk about <b><i>processor</i></b>, they mean CPU. I am not going to dive too deep in this topic. 32-bit CPU can support 32 bit on memory addresses which means about 34,359,738,368 bits at a time and <b>8 bits are called a byte</b> so its 4,294,967,296 bytes. One ASCII character is usually a byte. 32-bit CPU can support at max of 4 GB RAM. If it's 64-bit CPU then definitely can handle above 4GB RAM.

There are `integrated GPU` CPU where it also controls computer's display circuitry. The integrated GPU CPU is basically GPU and CPU on the same chip. Most of times for desktops, `GPU` (Graphic Processing Unit) are standalone graphic card using an empty expansion slot on the motherboard.

Other considerations when selecting CPU is those with ability to do `virtualization` and `execute disable bit`. Virtualization allows computer system to run more than one Operating System like Linux and Windows, or Apple and Windows, or Apple and Linux. Execute disable bit is used to classify areas of memory as non-executable, preventing the CPU from running any code residing there. Prevents malicious software from inserting its code into a program's data storage area then having CPU run its malicious code form within that memory area.

There are two different types of CPU sockets, <b><i>pin grid array</i> (PGA)</b> and <b><i>land grid array</i> (LGA)</b>. `PGA` cpu socket is where CPU is inserted by pinning pins in. `LGA` cpu socket replaces the pins with gold pads called lands. The pins are already located in the socket instead. I would prefer LGA, because pins on PGA can be damaged easily if forced to be inserted. LGA just snaps the CPU in. There are over 1000 pins for both LGA and PGA. Intel and AMD CPUs are not same and they have different numbers of pins.

There are CPU slot types. <b><i>Single Edge Contact Cartridge</i> (SECC)</b> is plastic housing covered CPU. Would have heat sink and fan attached to the housing. <b><i>SECC v2</i></b> doesn't use heat sink thermal plate. <b><i>Single Edge Processor</i> (SEP)</b> is similar to SECC, just doesn't use plastic housing. <b><i>Pin Array Cartridge</i> (PAC)</b> is designed to lay flat in a socket on the motherboard.      

There are about five different <b>CPU cooling methods</b>:
- `Cooling fans`: sits over on the top of CPU and pulls the warm air away to maintain a temperature of 32-43°C (90-110°F)

![cooling_fan](/public/img/A+/cooling_fan.jpg){: .center-image }

- `Heat sink`: also sits over top of a processor, they have metal "fingers" or "fins", absoring the heat from the processor. Made of aluminum or copper, copper is better but more expensive. One of perks is no CPU fan noise.

![heatsink](/public/img/A+/heatsink.jpg){: .center-image height="270px" width="auto" }

- `CPU cooler`: a system of heat sink, fan, and heat pipes. It is a popular choice and recommends to have <b>thermal paste</b> on the CPU before attaching CPU cooler.

![cpu_cooler](/public/img/A+/cpu_cooler.jpg){: .center-image height="270px" width="auto" }

- `Liquid cooling`: uses a pump to move deionized water or another patented, engineered liquid through a series of tubes over the processor, absorbing heat and move through water block where it cools. It is quieter than fans and coolers. The risk is if liquid spills... oh well.

![liquid_cooler](/public/img/A+/liquid_cooler.jpg){: .center-image height="270px" width="auto" }

## CMOS Battery

Lithium coin cell <b>CMOS battery</b> (shown in motherboard form factor figure above) provides continuous power to the computer's real-time clock and maintains the system BIOS settings. CMOS batter can last from 2 to 10 years before needing a replacement. Knowing when might need a replacement:
- incorrect or slow date system and time
- losing BIOS settings when computer is powered off

## RAM Slot

Mobo usually have 2 to 4 RAM slots to hold the memory chips. One RAM chip would be usually from 2 to 8 GB. If have multiple chips, then these GB add up. The 30Bird textbook focus on components on the motherboard for now.The <b><i>Random Access Memory</i> (RAM)</b> will be covered later in different post.

## Northbridge/Southbridge chipset

The `Northbridge chipset` connects directly to few components: CPU (via Front Side Bus (FSB)), RAMS, PCI Express graphics bus, and the Accelerated Graphics Port (AGP). Memory controller is located on the Northbridge which gives CPU faster access to the memory. Information from CPU has to go through Northbridge before reaching to the `Southbridge chipset`, which why Southbridge is slower. Northbridge is the only real communication bridge, connecting Southbridge chip to the CPU.  Many manufacturers would incorporate Northbridge onto the CPU itself to save cost and to improve the performance.

There are busses that connects to Southbridge chipset to the PCI bus, USB ports, IDE, SATA and or hard disk connections.

## Bus

`Bus` is a circuit that connects a component to another component. We saw FSB mentioned above about Northbridge and CPU, and there are several other busses. The faster (measured in MHz) bus is, the more data it can carry over at time. If people discuss about the speed of bus, they are likely talking about FSB because that's the most important part, CPU hello! Take a good look at the figure of busses below

![busses](/public/img/A+/busses.jpg){: .center-image height="300px" width="auto" }

- <b><i>FSB</i> (Front Side Bus)</b> connects Northbridge to CPU, and speed ranges from 66 to over 800 MHz
- <b><i>BSB</i> (Back Side Bus)</b>  connects CPU to L2 cache(s), CPU determines the speed
- <b><i>IDE or ATA Bus</i></b> connects Southbridge to the disk drives
- <b><i>PCI Bus</i></b> connects PCI slots to Southbridge and they average at 33 MHz speed, <b><i>PCI Express</i></b> (set of wires vs circuits) will replace PCI and AGP busses.

## SATA driver connectors

`Serial AT Attachment (SATA) driver connectors` connect modern hard disk drives HDD, solid state drives SSD, and optical drives to the circuity. AT is short for Advanced Technology in case you are wondering!  

## IDE driver connectors

`Integrated Drive Electornics (IDE) drive connectors` hooks up HDD/SSD to busses of the motherboard, two IDE drivers share one data cable, and it wil configure one as the master and the other as the slave.

## Other connectors

There are two types of power supplies: <b><i>AT/LPX and ATX</i></b>. Older PC motherboard uses AT/LPX power supplies whereas newer motherboards use ATX power supply.

- <b><i>ATX power connector</i></b> connects the 24-pin power cable of the power supply unit to provide the power, and it spuulies three spearate voltage levels: 3.3, 5, and 12V DC

- <b><i>ATX 12V power connector</i></b> is connects the 12 volt, 4-pin power cable of the power supply unit to provide low-voltage, high-ampere power to the CPU. There are motherboards that require 8-pin EPS 12 V power connector.

- <b><i>Fan connectors</i></b> typically have 3 or 4 pins. Three common pins are electrical ground, power, and a "sense output" pin that singals fan speed, if there are a fourth pin (control poin) it is used to adjust the rotation speed of the fan without adjusting the voltage. Some are for RGB LED colors too.

- <b><i>Front panel connector (fpanel or system panel connector)</i></b> contains socket to plug in five system cable: computer's power button, reset button, internal speaker, Hard disk activity LED light, and computer power LED light.

## Motherboard ports

Motherboard ports are the exposed part through the tower case cover (usually through back side of the tower). They are used for peripheral devices to plug in.

![mobo_ports](/public/img/A+/mobo_ports.jpeg){: .center-image height="270px" width="auto" }

- `Universal Serial Bus (USB)` plugs in all peripheral devices such as keyboard, mouse, digital cameras, printers, external disk drives and etc to the motherboard. There are USB types: A, B, and C.

![USB_types](/public/img/A+/USB_types.png){: .center-image height="200px" width="auto" }

Let's focus on USB Type A for now. There are three specifications: 1.x, 2.x, and 3.x. Each have differences, look at the chart below. I would like to note that there are difference between <b><i>megabit per second (mbps)</i></b> and <b><i>megabyte per second (MBps)</i></b>. A 8 of bits are a byte but both speed unit have different use for transmission rate. Speed unit mbps is used to measure a download speed while MBps is used to measure the file size.  

| USB | 1.x | 2.x | 3.0 | 3.1 |
|-------|-------|-------|-------|
| mbps | 12 | 480 | 5 Gbps | 10 Gbps |
| MBps | 1.5 | 60 | 625 | 1.21 GB/s |
| port colors | white | white or black | blue | blue |

- PS/2 six-pin interface used to connect older keyboards and pointing device (mouse), newer keyboards and mouse uses usb now. They are usually color coded like purple/pink for keyboards and lime/green for mouse.




[A+ 901 Study Guide]:https://docs.google.com/document/d/1Shh_BNuw4xh2mlr3UVBpBWqbvWJNnTtuSq12RFsjvAo/edit
[PCPartPicker]:https://pcpartpicker.com/
