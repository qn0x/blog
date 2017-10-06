---
title: Building A Custom 60% Mechanical Keyboard
updated: 2017-10-01 22:00
categories:
    - mechanical-keyboards
---
**TL;DR**  
If you just want the build pictures without any explanations, here's the link to the [Imgur album](https://imgur.com/a/JqzZP).
- - -
I've been into mechanical keyboards for a little more than a year. After throwing myself into cold water by buying a Pok3r as my first board, I've since been accustomed to the 60% form factor. 60% meaning using basically just the alphanumeric "block" and moving the F-keys and the number pad to function-layers that are accessible via different key-combinations across different virtual keyboard layers.  
After gaining some more soldering experience by building my first DIY-keyboard, the [S-60X](https://sentraq.com/collections/kits/products/s60-x-diy-keyboard-kit), I've made my decisions on what parts to use for my first truly custom board.  

My goals were pretty straight forward: I wanted to use the high profile aluminum case with a weight insert for which I entered a Group Buy in May (it also has underglow), my brass plate that I bought on impulse some time earlier this year, as well as a custom layout (split backspace, split right shift, split space bar, arrow cluster on the bottom right):  

![custom keyboard layout]({{site.baseurl}}/assets/images/keyboard-layout.png)

As you can see, the split space bar consists of three keys (6.25u space bar = 2.25u + 1.25u + 2.75u keys). The right shift is also split into three keys (2.75u shift = 1u + 1.75u keys) and moved to the left by 1u. The bottom right row is split into five instead of four keys to allow space for the navigation cluster (4 x 1.25u = 5 x 1u).  
With the already very limited options because of the complex layout, it was impossible to find a PCB/plate/case-combo that satisfied all of my wishes. I've shelved some of the layout customizations for a later project and decided to stick with parts that I already had or were scheduled to ship to me in the near future.

## Parts
 * **Case**: I originally planned to use this beautiful [aluminum high profile case from Sentraq with brass weight](https://sentraq.com/collections/group-buys/products/sentraq-60-high-profile-aluminum-case) but after countless delays of the Group Buy that more than doubled the waiting time, I decided to temporarily use this [acrylic case from mechboards UK](https://mechboards.co.uk/shop/all/60-diffused-acrylic-case/) until my case arrives.
 * **Plate**: [Brass plate from mechanisk](https://mekanisk.co/).
 * **Switches**: I've loved [Zealios](https://zealpc.net/collections/switches/products/zealio) ever since modding my Pok3r with the tactile 65g version. This board will have the tactile 67g variant.
 * **Switch tops**: Stumbled upon these [dyed switch tops from KBDfans](https://kbdfans.cn/collections/keyboard-part/products/gateron-rainbow-dyeing-top-house-10pcs) and decided to use the purple ones.
 * **Stabilizers**: [Transparent screw-ins from Zealpc](https://zealpc.net/collections/switches/products/zealstabilizers).
 * **PCB**: The [b.faceX2 from Winkeyless](http://winkeyless.kr/product/b-face-x2-pcb/). I wanted one that came with pre-soldered underglow and support for my desired layout which includes a split backspace and split right shift.
 * **Keycaps**: I stripped my [Originative GMK Skeletor](https://originative.co/products/skeletor) set from my S-60X because I wanted to go with the whole purple/golden theme. It was the only set I had that kind of matched my theme and supported my planned layout.
 * **Miscellaneous**:  
   [Lube](https://zealpc.net/collections/switches/products/ghlube) for switches and stabilizers,  
   Cable: currently undecided whether to even get a new one,  
   Cotton wool from Q-Tips to lessen the rattling sound from the stabilizers,  
   Sound dampening inlay inside the case cut out of a thick old [Roccat mouse mat](https://www.roccat.org/en-DE/Products/Gaming-Mousepads/Taito-Series/Taito/). This will be put in when the Sentraq case arrives.

#### Other Considerations:
 * __Sentraq PCB__   
   _pro:_ used it before, has underglow, easy to cofigure and flash(website configurator)  
   _con:_ seems unreliable, people that were in the Massdrop GB of the S-60X have reported that their underglow LEDs stopped working after some time(happend to mine, too)
 * __GH60 Satan PCB__  
   _pro:_ easy to source, popular(meaning more community-support in case something goes wrong)  
   _con:_ no underglow
 * __Banana Split PCB__  
   _pro:_ compatible with a lot of key sets (6.25u space bar = 2.25u + 1.25u + 2.75u keys)  
   _con:_ requires a special plate, missed the GB
 * __Zeal60 PCB__  
   _pro:_ per-switch LED  
   _con:_ expensive, no underglow, wasn't available when I decided which PCB to use
 * __In-switch LEDs (with hotswap-sockets)__  
 I may add the LEDs later but without being sure whether sockets will fit or not, I've, as of now, decided against them.
 * __Holtites__  
 They seem to be compatible with the b.face PCB but I'm not planning on replacing the switches anytime soon. I also don't know how tight they fit the switches and because I may travel with the board, I didn't want to risk them being loose and the switches falling out.

### Tools
 * small flat head screwdriver that allows opening of the switches (alternatively a switch opener)
 * pliers/scissors for removing the excess plastic from the PCB-mountable switches, cutting the sound dampening material and opening all the packages :)
 * small philipp's head screwdriver for the stabilizers and case
 * paper clip for testing of the PCB
 * something small like a toothpick to apply the lube to the switches and sqeeze the cotton wool into the stabilizers
 * soldering equipment (soldering iron, solder, just in case: desoldering pump)

## The Build
Almost all of the parts are already here! I already opened the switches so I could solder them without the switch tops.  

![Parts](https://i.imgur.com/ZbVpj0e.jpg)  

Checking the PCB with a bent paper clip. I used [Aqua Key Test]((https://geekhack.org/index.php?topic=34670) from Geekhack but this site http://www.keyboardtester.com/ works, too.  

![Checking PCB](https://i.imgur.com/P3HYQQY.jpg)  

Assembling the stabilizers. The description said that they are pre-clipped so no need for any mods.  

![Assembling stabilizers](https://i.imgur.com/JZXb7Dp.jpg)  

Very funny.  

![Haha](https://i.imgur.com/ewZPlK6.jpg)  

Screwed-in stabilizer  

![stabilizer](https://i.imgur.com/S4t9OUl.jpg)  

I only soldered the switch housings because the tops hadn't arrived. Started with the switches in the corners, then the edges and worked my way in.  

![Soldering](https://i.imgur.com/xYoJeKo.jpg)  

Another test to make sure there are no cold solder points before screwing in PCB + plate. Used the left CTRL to access the bootloader. Seems good.  

![PCB Test](https://i.imgur.com/dxh6OGr.jpg)  


## Lessons Learned
 1. Group Buy delays are unpredictable.
 2. Shipping from China to Germany can faster than shipping from the UK to Germany  
 3. This can get pretty expensive really fast. Not including the shipping costs and customs fees this beauty ended up costing me around 500€
 4. Time. Lubing the switches was by far the most time-consuming step of the build.
