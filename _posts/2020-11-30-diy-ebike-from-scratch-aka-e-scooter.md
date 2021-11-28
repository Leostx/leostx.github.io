---
title: DIY Ebike from scratch aka e-scooter
date: 2020-11-30T17:18:26+01:00
permalink: /ebike/
image: https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_03-1200x900.jpg?v=1606689595
categories:
  - Mechanical
tags:
  - 3d print
  - belt drive
  - bike
  - bldc motor
  - direct drive
  - diy
  - ebike
  - electric
  - escooter
  - friction drive
  - holland bike
  - hub motor
  - scooter
  - scratch
  - vesc
excerp: "A few months ago I got a Hub-Motor from a broken e-scooter, within a day I welded it on the back wheel of my bike. This was the beginning of a long journey on electrifying a bike."
header:
  overlay_image: /assets/images/ebike/ebike_p_mk3_04.jpg
  overlay_filter: 0.5
---
A few months ago I got a Hub-Motor from a broken e-scooter, within a day I welded it on the back wheel of my bike. This was the beginning of a long journey on electrifying a bike.

<figure class="half">
  <img src="/assets/images/ebike/ebike_fd_mk1_01.jpg">
  <img src="/assets/images/ebike/ebike_fd_mk1_02.jpg">
</figure>


Today I know, that you often refer to this first type of drive system as &#8220;friction drive&#8221;. Later on, I changed the battery and speed-controller arrangement. During the whole summer I used this contraption and it worked quite well, but I stumbled across two main problems: During fast acceleration, the bike wheel gets consumed quite a lot and on wet or dusty roads the drive wheel doesn&#8217;t have enough friction to drive the rear wheel. So it was time to plan …

## Mark II {#mkII}

To address the previously mentioned problems I decided to go with a &#8220;belt drive&#8221; system, driven from a 280kv BLDC motor.  
Organizing the belt and the motor pulley, without waiting two months for things arriving from china, wasn&#8217;t that easy. So the only ones I could get were HTD-3M ones. The motor pulley has 20 teeth. The wheel pulley has got 204 and was 3d printed.  
I had to fiddle around quite a while to get the tolerances right, but in the end, the belt was fitting nicely.

<figure class="half">
  <img src="/assets/images/ebike/ebike_bd_mk2_01.jpg" alt="Belt and BLDC motor">
  <img src="/assets/images/ebike/ebike_bd_mk2_02.jpg" alt="204T wheel pulley">
</figure>


Finding the right design for the motor mount took way too long. The first iteration build with metal brackets failed badly. But in the end, I came up with a combination of aluminum end a 3d Printed mount. To align the pulleys properly, I had to figure out the right angle between the bike&#8217;s frame and the wheel. I added a tensioner consisting of two ball bearings to prevent the belt from skipping. To prevent the mount from slipping towards the axis I drilled a hole through the frame and the mount so that I could fix it with a bold.

<img src="/assets/images/ebike/ebike_bd_mk2_04.jpg" alt"Failed steel brackets">
<img src="/assets/images/ebike/ebike_bd_mk2_06.jpg" alt"Motor mount 3d model>
<figure class="third">
  <img src="/assets/images/ebike/ebike_bd_mk2_11.jpg" alt="">
  <img src="/assets/images/ebike/ebike_bd_mk2_12.jpg" alt="">
  <img src="/assets/images/ebike/ebike_bd_mk2_13.jpg" alt="">
</figure>

After a lot of unsuccessful test rides, I again figured out two major problems: No matter how much the belt was tensioned, it continued skipping teeth due to a too small pitch for the applied forces.  
Secondly, because of the bike&#8217;s roughness, it was practically impossible to align the pulleys, so the belt continued slipping off them.  
So I started rethinking the whole drive system and came up with…

## Mark III {#mkIII}

In this last version, I decided to go back to the roots and use the hub motor from mkI as it was intended by its creators: as a hub motor.  
To do so I needed to rebuild the front wheel. I calculated the necessary spoke length with some trigonometry and used the original wheel as a reference. It took me a while to find a bike shop selling shorter spokes for a reasonable price. In the end, I took the length they had and design the adapter around them.  
To test things out I started with a 3d-Printed adapter, which worked well, besides the plastics&#8217; very low melting point. So I used the 3d drawing to print the outlines on paper and cut it out from a 1,5mm thick steel sheet.  
I tensioned and rounded the bike’s wheel by myself, but due to a lack of equipment for a perfect result, I will have to bring it to a bike shop.  
I had to enlarge the slot in the bike&#8217;s fork to fit the motor axis, this caused the motor to slip out of it from time to time, to solve this and give the axis some more stability I added a small metal piece on either side.

<img src="/assets/images/ebike/ebike_hd_mk3_01.jpg" alt"Hub Motor Adapter">
<figure class="third">
  <img src="/assets/images/ebike/ebike_hd_mk3_02.jpg" alt="">
  <img src="/assets/images/ebike/ebike_hd_mk3_03.jpg" alt="">
  <img src="/assets/images/ebike/ebike_hd_mk3_04.jpg" alt="">
</figure>
<figure class="third">
  <img src="/assets/images/ebike/ebike_hd_mk3_05.jpg" alt="">
  <img src="/assets/images/ebike/ebike_hd_mk3_06.jpg" alt="">
  <img src="/assets/images/ebike/ebike_hd_mk3_07.jpg" alt="">
</figure>


## Battery & ESC {#battery}

The battery is the one recovered from the e-scooter. It is a 10s Lithium-ion one and has a nominal capacity of 12.8Ah. I placed it between the two down tubes of the holland bike, so that it doesn&#8217;t mess with the center of mass. I couldn&#8217;t find the specs for this specific model online, so I had to find it out the hard way. I blew the internal 30A fuse and had to replace it.

As the ESC I used a VESC 4. The throttle, brake, and front light were also recovered from the scooter. The throttle works like a potentiometer, the break is just a momentary switch.  
Intending to add some custom cruise control, I played around with the VESC firmware and managed to brick the device. Not even through the Serial Wire Debugging Interface (SWD) I was able to reflash it. So I had to unsolder the STM32&#8217;s BOOT0 pin, pull it high to prevent the STM32 from loading the previously flashed code, reflash the original bootloader & firmware and solder it again to the PCB.

With an Arduino and a simple OLED display, I&#8217;ve done a little telemetry screen on the handle. I also attached three buttons and a Bluetooth module for future improvements.

<figure class="third">
  <img src="/assets/images/ebike/ebike_p_mk3_05.jpg" alt="Battery placement">
  <img src="/assets/images/ebike/ebike_p_mk3_06.jpg" alt="VESC placement">
  <img src="/assets/images/ebike/ebike_p_mk3_07.jpg" alt="Handlebar">
</figure>

## Conclusion  {#conclusion}

When I first started this project I had no idea how long this would take. I didn&#8217;t do a lot of mechanical projects before, so this was kind of new terrain. It was an equally interesting and frustrating experience. I am quite happy that I didn&#8217;t give up and that now I&#8217;m in the possession of an electric bike to cruise around easily. I couldn&#8217;t fully test the range out by now, but it should be >20km with a maximum speed of around 30km/h.  
In the future, I would like to add a main-battery driven taillight, a custom cruise control software, and some telemetry over Bluetooth.

<img src="/assets/images/ebike/ebike_bd_mk2_04.jpg" alt"">
<img src="/assets/images/ebike/ebike_p_mk3_04.jpg" alt"">

--
