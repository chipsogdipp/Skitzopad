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
* Storage: 914 GB SATA SSD.



**[Firmware]**



**[Software]**

**[Setbacks]**

I am personally familiar with modification of general/common hardware, as of writing this section I've had no issues. 
(Note: I haven't made any difficult hardware changes such as the screen, as my Thinkpad already came with a good/decent screen.)

As for Firmware, the first major roadblock personally was the poor official documentation. I found it difficult to be certain of what exactly had to be done and in what order. 
For the second roadblock it was the programmer, for firmware modification you need a programmer and the hardware to facilitate changes to the relevant chips. 
When I came to the point of flashing the chip I realized that I don't currently have the tools to do so. As far as I know there are no local retailers for those tools so I got a bit stuck, not knowing what I should order.
