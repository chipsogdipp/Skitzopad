# Skitzopad

On this Github page I will document the improvements and changes I have made, and will make to my Thinkpad T480. This will be an ever growing list, as I experiment and learn new things.

**[Why?]**

Computers have always struck me as a masterpiece of refined, principled logic. An engineering puzzle, one I've longed to solve through hands-on tinkering, but never fully grasped.  That's the core reason behind these laptop upgrades and improvements: I want to understand computing from the silicon upward, not merely how to operate it. Sticking with one known-good set of hardware gives me the clean, predictable canvas I need to experiment without endless fights against drivers or abstraction layers.

My goals are: 
* Understanding the boot process end-to-end, including the interplay of firmware, bootloader, kernel and early userspace.
* Sharpen my skills with Linux, being able to utilize it more properly to fit a more restrictive set of hardware specs.
* Connecting the physical behavior of hardware components directly to the code I write and debug
* Ultimately bridging the human-computer gap, being able to visualize concretely what goes on inside computers

In short, I want to demystify the apparent black magic that makes computers work. I want to understand what makes a system tick, not just GUIs or Python scripts. This project is about transforming "it just works" to "I know exactly why and how it works." 

**[Hardware]** 

(Note: This is a Lenovo Thinkpad T480 serving as an ongoing experimental platform-specs are subject to upgrades and changes as I learn and iterate.)

* Display: 14", 1920x1080@60Hz
* CPU: Intel i5-8350U, 4 cores / 8 threads turbo up to 3.6 GHz
* GPU: Intel UHD Graphics 620 (integrated, up to ~1.1 GHz)
* RAM: 32GB DDR4
* Storage: 1.8 TB NVME SSD.



**[Firmware]**

Modification of firmware was the reason I started documenting the changes. I discovered Libreboot (https://libreboot.org/) whose emphasis on software freedom and user control closely aligned with my own views. As a result I felt the need to replace the factory firmware with Libreboot.
Switching the BIOS for the Libreboot alternative was not only a technical exercise but a small act of independence from increasingly opaque computing platforms and a step towards understanding and controlling the software that runs on my hardware. 
In a world where users are expected to trust systems they don't understand and cannot inspect, Libreboot offers a refreshing alternative.

The modification so far involves two flash chips on the motherboard: the **Winbond W25Q128JVSJQ** and the **Winbond W25Q80DV**. Since they have the same pinouts, no changes in the wiring were required for flashing to the chips. 

**[Software]**

**[Setbacks]**

I am personally familiar with modification of general/common hardware, and so far I've had no major issues.
(Note: I haven't made any difficult hardware swaps such as the screen, as my Thinkpad already came with a good IPS panel.)

As for firmware, my first major roadblock was the official documentation. It's fragmented across multiple pages, dense with technical assumptions, and hard to follow in sequence, for instance, figuring out exactly when to dump/backup the stock flash, or what "injecting vendor files" actually entailed (inserting neutered Intel ME blobs, applying deguard for Boot Guard bypass, and running build scripts or manual tools on release ROMs). Despite having a dedicated page for the T480, it somehow made things more uncertain: it bombarded me with warnings, prerequisites, and cross-references to other guides (like ivy_has_common.html for vendor insertion, spi.html for flashing basics, and separate Thunderbolt handling), without a clear, linear checklist tying everything together for this specific model. I constantly second-guessed the order and whether I'd missed a critical step.

For the second roadblock it was the programmer, for firmware modification you need a programmer and the hardware to facilitate changes to the relevant chips. 
When I came to the point of flashing the chip I realized that I don't currently have the tools to do so. As far as I know there are no local retailers for those tools so I got a bit stuck, not knowing what I should order.
