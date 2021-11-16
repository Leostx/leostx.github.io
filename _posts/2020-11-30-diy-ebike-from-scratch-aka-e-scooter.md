---
title: DIY Ebike from scratch aka e-scooter
date: 2020-11-30T17:18:26+01:00
layout: post
permalink: /ebike/
read_time: true
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
---
A few months ago I got a Hub-Motor from a broken e-scooter, within a day I welded it on the back wheel of my bike. This was the beginning of a long journey on electrifying a bike.

<!--more READ more--><figure class="wp-block-gallery aligncenter columns-2 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_01.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_01-1024x768.jpg" alt="" data-id="51" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_01.jpg" data-link="https://stexo.eu/ebike_fd_mk1_01/" class="wp-image-51" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_01-1024x768.jpg?v=1606687971 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_01-300x225.jpg?v=1606687971 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_01-768x576.jpg?v=1606687971 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_01-1200x900.jpg?v=1606687971 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_01.jpg?v=1606687971 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_02.jpg"><img loading="lazy" width="768" height="1024" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_02-768x1024.jpg" alt="" data-id="52" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_02.jpg" data-link="https://stexo.eu/ebike_fd_mk1_02/" class="wp-image-52" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_02-768x1024.jpg?v=1606687970 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_02-225x300.jpg?v=1606687970 225w, https://stexo.eu/wp-content/uploads/2020/11/ebike_fd_mk1_02.jpg?v=1606687970 960w" sizes="(max-width: 768px) 100vw, 768px" /></a></figure>
  </li>
</ul></figure> 

Today I know, that you often refer to this first type of drive system as &#8220;friction drive&#8221;. Later on, I changed the battery and speed-controller arrangement. During the whole summer I used this contraption and it worked quite well, but I stumbled across two main problems: During fast acceleration, the bike wheel gets consumed quite a lot and on wet or dusty roads the drive wheel doesn&#8217;t have enough friction to drive the rear wheel. So it was time to plan …

## Mark II {#mkII}

To address the previously mentioned problems I decided to go with a &#8220;belt drive&#8221; system, driven from a 280kv BLDC motor.  
Organizing the belt and the motor pulley, without waiting two months for things arriving from china, wasn&#8217;t that easy. So the only ones I could get were HTD-3M ones. The motor pulley has 20 teeth. The wheel pulley has got 204 and was 3d printed.  
I had to fiddle around quite a while to get the tolerances right, but in the end, the belt was fitting nicely.<figure class="wp-block-gallery columns-2 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_01.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_01-1024x768.jpg" alt="" data-id="61" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_01.jpg" data-link="https://stexo.eu/?attachment_id=61" class="wp-image-61" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_01-1024x768.jpg?v=1606687969 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_01-300x225.jpg?v=1606687969 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_01-768x576.jpg?v=1606687969 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_01-1200x900.jpg?v=1606687969 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_01.jpg?v=1606687969 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a><figcaption class="blocks-gallery-item__caption">Belt and BLDC motor</figcaption></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_02.jpg"><img loading="lazy" width="1024" height="711" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_02-1024x711.jpg" alt="" data-id="62" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_02.jpg" data-link="https://stexo.eu/?attachment_id=62" class="wp-image-62" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_02-1024x711.jpg?v=1606687968 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_02-300x208.jpg?v=1606687968 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_02-768x533.jpg?v=1606687968 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_02.jpg?v=1606687968 1033w" sizes="(max-width: 1024px) 100vw, 1024px" /></a><figcaption class="blocks-gallery-item__caption">204T wheel pulley</figcaption></figure>
  </li>
</ul></figure> 

  
Finding the right design for the motor mount took way too long. The first iteration build with metal brackets failed badly. But in the end, I came up with a combination of aluminum end a 3d Printed mount. To align the pulleys properly, I had to figure out the right angle between the bike&#8217;s frame and the wheel. I added a tensioner consisting of two ball bearings to prevent the belt from skipping. To prevent the mount from slipping towards the axis I drilled a hole through the frame and the mount so that I could fix it with a bold.<figure class="wp-block-gallery columns-1 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_04-e1606503452793.jpg"><img loading="lazy" width="720" height="862" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_04-e1606503452793.jpg?v=1606513246" alt="Failed steel brackets" data-id="63" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_04-e1606503452793.jpg" data-link="https://stexo.eu/?attachment_id=63" class="wp-image-63" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_04-e1606503452793.jpg?v=1606687967 720w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_04-e1606503452793-251x300.jpg?v=1606687967 251w" sizes="(max-width: 720px) 100vw, 720px" /></a><figcaption class="blocks-gallery-item__caption">Failed steel brackets</figcaption></figure>
  </li>
</ul></figure> <figure class="wp-block-gallery columns-1 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_06.jpg"><img loading="lazy" width="821" height="688" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_06.jpg?v=1606513245" alt="MotorMount 3d model" data-id="64" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_06.jpg" data-link="https://stexo.eu/?attachment_id=64" class="wp-image-64" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_06.jpg?v=1606687966 821w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_06-300x251.jpg?v=1606687966 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_06-768x644.jpg?v=1606687966 768w" sizes="(max-width: 821px) 100vw, 821px" /></a><figcaption class="blocks-gallery-item__caption">MotorMount 3d model</figcaption></figure>
  </li>
</ul></figure> <figure class="wp-block-gallery columns-3 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_11.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_11-1024x768.jpg?v=1606513244" alt="" data-id="66" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_11.jpg" data-link="https://stexo.eu/?attachment_id=66" class="wp-image-66" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_11-1024x768.jpg?v=1606687966 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_11-300x225.jpg?v=1606687966 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_11-768x576.jpg?v=1606687966 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_11-1200x900.jpg?v=1606687966 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_11.jpg?v=1606687966 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_12.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_12-1024x768.jpg?v=1606513242" alt="" data-id="67" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_12.jpg" data-link="https://stexo.eu/?attachment_id=67" class="wp-image-67" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_12-1024x768.jpg?v=1606687965 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_12-300x225.jpg?v=1606687965 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_12-768x576.jpg?v=1606687965 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_12-1200x900.jpg?v=1606687965 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_12.jpg?v=1606687965 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_13.jpg"><img loading="lazy" width="576" height="1024" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_13-576x1024.jpg?v=1606513241" alt="" data-id="68" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_13.jpg" data-link="https://stexo.eu/?attachment_id=68" class="wp-image-68" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_13-576x1024.jpg?v=1606687963 576w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_13-169x300.jpg?v=1606687963 169w, https://stexo.eu/wp-content/uploads/2020/11/ebike_bd_mk2_13.jpg?v=1606687963 720w" sizes="(max-width: 576px) 100vw, 576px" /></a></figure>
  </li>
</ul></figure> 

After a lot of unsuccessful test rides, I again figured out two major problems: No matter how much the belt was tensioned, it continued skipping teeth due to a too small pitch for the applied forces.  
Secondly, because of the bike&#8217;s roughness, it was practically impossible to align the pulleys, so the belt continued slipping off them.  
So I started rethinking the whole drive system and came up with…

## Mark III {#mkIII}

In this last version, I decided to go back to the roots and use the hub motor from mkI as it was intended by its creators: as a hub motor.  
To do so I needed to rebuild the front wheel. I calculated the necessary spoke length with some trigonometry and used the original wheel as a reference. It took me a while to find a bike shop selling shorter spokes for a reasonable price. In the end, I took the length they had and design the adapter around them.  
To test things out I started with a 3d-Printed adapter, which worked well, besides the plastics&#8217; very low melting point. So I used the 3d drawing to print the outlines on paper and cut it out from a 1,5mm thick steel sheet.  
I tensioned and rounded the bike’s wheel by myself, but due to a lack of equipment for a perfect result, I will have to bring it to a bike shop.  
I had to enlarge the slot in the bike&#8217;s fork to fit the motor axis, this caused the motor to slip out of it from time to time, to solve this and give the axis some more stability I added a small metal piece on either side.<figure class="wp-block-gallery columns-1 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_01.jpg"><img loading="lazy" width="1024" height="702" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_01-1024x702.jpg" alt="Hub Motor Adapter" data-id="70" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_01.jpg" data-link="https://stexo.eu/?attachment_id=70" class="wp-image-70" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_01-1024x702.jpg?v=1606687962 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_01-300x206.jpg?v=1606687962 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_01-768x527.jpg?v=1606687962 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_01.jpg?v=1606687962 1040w" sizes="(max-width: 1024px) 100vw, 1024px" /></a><figcaption class="blocks-gallery-item__caption">Hub Motor Adapter</figcaption></figure>
  </li>
</ul></figure> <figure class="wp-block-gallery columns-3 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_02.jpg"><img loading="lazy" width="768" height="1024" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_02-768x1024.jpg" alt="" data-id="71" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_02.jpg" data-link="https://stexo.eu/?attachment_id=71" class="wp-image-71" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_02-768x1024.jpg?v=1606687961 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_02-225x300.jpg?v=1606687961 225w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_02.jpg?v=1606687961 960w" sizes="(max-width: 768px) 100vw, 768px" /></a></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_03.jpg"><img loading="lazy" width="768" height="1024" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_03-768x1024.jpg" alt="" data-id="72" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_03.jpg" data-link="https://stexo.eu/?attachment_id=72" class="wp-image-72" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_03-768x1024.jpg?v=1606687960 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_03-225x300.jpg?v=1606687960 225w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_03.jpg?v=1606687960 960w" sizes="(max-width: 768px) 100vw, 768px" /></a></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_04.jpg"><img loading="lazy" width="576" height="1024" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_04-576x1024.jpg" alt="" data-id="73" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_04.jpg" data-link="https://stexo.eu/?attachment_id=73" class="wp-image-73" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_04-576x1024.jpg?v=1606687959 576w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_04-169x300.jpg?v=1606687959 169w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_04.jpg?v=1606687959 720w" sizes="(max-width: 576px) 100vw, 576px" /></a></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_05.jpg"><img loading="lazy" width="768" height="1024" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_05-768x1024.jpg" alt="" data-id="74" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_05.jpg" data-link="https://stexo.eu/?attachment_id=74" class="wp-image-74" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_05-768x1024.jpg?v=1606687958 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_05-225x300.jpg?v=1606687958 225w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_05.jpg?v=1606687958 960w" sizes="(max-width: 768px) 100vw, 768px" /></a></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_06.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_06-1024x768.jpg" alt="" data-id="75" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_06.jpg" data-link="https://stexo.eu/?attachment_id=75" class="wp-image-75" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_06-1024x768.jpg?v=1606687957 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_06-300x225.jpg?v=1606687957 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_06-768x576.jpg?v=1606687957 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_06-1200x900.jpg?v=1606687957 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_06.jpg?v=1606687957 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_07.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_07-1024x768.jpg" alt="" data-id="76" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_07.jpg" data-link="https://stexo.eu/?attachment_id=76" class="wp-image-76" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_07-1024x768.jpg?v=1606687956 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_07-300x225.jpg?v=1606687956 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_07-768x576.jpg?v=1606687956 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_07-1200x900.jpg?v=1606687956 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_hd_mk3_07.jpg?v=1606687956 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a></figure>
  </li>
</ul></figure> 

## Battery & ESC {#battery}

The battery is the one recovered from the e-scooter. It is a 10s Lithium-ion one and has a nominal capacity of 12.8Ah. I placed it between the two down tubes of the holland bike, so that it doesn&#8217;t mess with the center of mass. I couldn&#8217;t find the specs for this specific model online, so I had to find it out the hard way. I blew the internal 30A fuse and had to replace it. 

As the ESC I used a VESC 4. The throttle, brake, and front light were also recovered from the scooter. The throttle works like a potentiometer, the break is just a momentary switch.  
Intending to add some custom cruise control, I played around with the VESC firmware and managed to brick the device. Not even through the Serial Wire Debugging Interface (SWD) I was able to reflash it. So I had to unsolder the STM32&#8217;s BOOT0 pin, pull it high to prevent the STM32 from loading the previously flashed code, reflash the original bootloader & firmware and solder it again to the PCB.

With an Arduino and a simple OLED display, I&#8217;ve done a little telemetry screen on the handle. I also attached three buttons and a Bluetooth module for future improvements.<figure class="wp-block-gallery columns-3 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_05.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_05-1024x768.jpg" alt="" data-id="99" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_05.jpg" data-link="https://stexo.eu/?attachment_id=99" class="wp-image-99" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_05-1024x768.jpg?v=1606751969 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_05-300x225.jpg?v=1606751969 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_05-768x576.jpg?v=1606751969 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_05-1200x900.jpg?v=1606751969 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_05.jpg?v=1606751969 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a><figcaption class="blocks-gallery-item__caption">Battery placement</figcaption></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_06.jpg"><img loading="lazy" width="768" height="1024" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_06-768x1024.jpg" alt="" data-id="97" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_06.jpg" data-link="https://stexo.eu/?attachment_id=97" class="wp-image-97" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_06-768x1024.jpg?v=1606751936 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_06-225x300.jpg?v=1606751936 225w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_06.jpg?v=1606751936 960w" sizes="(max-width: 768px) 100vw, 768px" /></a><figcaption class="blocks-gallery-item__caption">VESC placement</figcaption></figure>
  </li>
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_07.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_07-1024x768.jpg" alt="" data-id="98" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_07.jpg" data-link="https://stexo.eu/?attachment_id=98" class="wp-image-98" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_07-1024x768.jpg?v=1606751940 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_07-300x225.jpg?v=1606751940 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_07-768x576.jpg?v=1606751940 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_07-1200x900.jpg?v=1606751940 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_07.jpg?v=1606751940 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a><figcaption class="blocks-gallery-item__caption">Handlebar</figcaption></figure>
  </li>
</ul></figure> 

## Conclusion  {#conclusion}

When I first started this project I had no idea how long this would take. I didn&#8217;t do a lot of mechanical projects before, so this was kind of new terrain. It was an equally interesting and frustrating experience. I am quite happy that I didn&#8217;t give up and that now I&#8217;m in the possession of an electric bike to cruise around easily. I couldn&#8217;t fully test the range out by now, but it should be >20km with a maximum speed of around 30km/h.  
In the future, I would like to add a main-battery driven taillight, a custom cruise control software, and some telemetry over Bluetooth.<figure class="wp-block-gallery columns-1 is-cropped">

<ul class="blocks-gallery-grid">
  <li class="blocks-gallery-item">
    <figure><a href="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_04.jpg"><img loading="lazy" width="1024" height="768" src="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_04-1024x768.jpg" alt="" data-id="94" data-full-url="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_04.jpg" data-link="https://stexo.eu/ebike_p_mk3_04/" class="wp-image-94" srcset="https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_04-1024x768.jpg?v=1606689603 1024w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_04-300x225.jpg?v=1606689603 300w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_04-768x576.jpg?v=1606689603 768w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_04-1200x900.jpg?v=1606689603 1200w, https://stexo.eu/wp-content/uploads/2020/11/ebike_p_mk3_04.jpg?v=1606689603 1280w" sizes="(max-width: 1024px) 100vw, 1024px" /></a></figure>
  </li>
</ul></figure>
