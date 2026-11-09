+++
title = "Assembly Language Learning Resources"
date = 2022-11-30T09:00:00
+++
## Why learn assembly language, considering it is hardly used today?

A basic knowledge of assembly language is required to understand how CPUs work and is considered an essential part of a computer science education. Furthermore, many people consider it fun!

## Which assembly language to learn

Modern Intel assembly language is designed to be written by compilers and so is quite difficult to learn for humans. There’s also not much you can practically do with it outside of writing advanced vectorised video codecs.

I recommend [6502](https://en.wikipedia.org/wiki/MOS_Technology_6502) assembly because it is pleasant to write and it does have the practical use of creating games for 8 bit computers (for which it is still used, because those systems can’t be programmed in higher level languages optimally.)
It's also still used in embedded systems.

The [Z80](https://en.wikipedia.org/wiki/Zilog_Z80) is similar but I don't like it so much.

The only other option I would consider is [ARM](https://en.wikipedia.org/wiki/ARM_architecture_family) assembly. It too was designed for humans to write, and it has the advantage of running on modern systems like Raspberry Pi. However the other aspects of these ARM systems are more complex and they don’t have the wealth of learning communities that the old 6502 systems do.

## Approach

6502 assembly is not particularly difficult in itself, but a 6502 chip alone is unable to generate sound and video, so each 6502 computer required additional chips and the details of how to access them vary a lot between different systems.  So I would break down learning into two (interleaved) phases:

1. Learn generic 6502 code. Platform doesn't really matter. Write simple algorithms. Use a debugger to view the results in memory. Possibly use some platform specific code to output results as text.

2. Choose a specific platform and learn how the video chip works on that platform in order to create graphical programs and games. I think the most interesting platforms are probably [C64](https://en.wikipedia.org/wiki/Commodore_64), [Commander X16](https://www.commanderx16.com/) and [NES](https://en.wikipedia.org/wiki/Nintendo_Entertainment_System). (Possibly the [BBC](https://en.wikipedia.org/wiki/BBC_Micro) might be easier, but not many people are impressed by BBC games.)

## Texts

### [Easy6502](https://skilldrick.github.io/easy6502/)


Easy6502 is a short tutorial text that is very interesting because it comes with a 6502 emulator that runs in the web browser. The emulator supports graphics in a much simpler way than any real systems, so it’s a good way to get started and quickly see graphical results.

TokyoEdTech has made a **video** of himself writing some programs on the Easy6502 simulator. The first half is a good introduction; the second half is quite rambling and unprepared since he’s coding live.

<iframe width="560" height="315" src="https://www.youtube.com/embed/PxZGoiWvA4A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[There is an older version of the emulator here](http://6502asm.com/), which is worth checking out because it includes example programs: 

### [Machine Language for the Commodore 64 book by Jim Butterfield](https://archive.org/details/Machine_Language_for_the_Commodore_Revised_and_Expanded_Edition)

[PDF](https://datassette.nyc3.cdn.digitaloceanspaces.com/livros/machine_language_for_the_commodore_revised_and_expanded_edition.pdf)

This is an *excellent* book for learning 6502 but is focused on the Commodore 64 and spends a lot of time explaining how to use machine code monitors, assemblers and disassemblers on that system, which isn’t required today since we can write the code on our PCs. It doesn’t actually have space to get into the useful Commodore specific stuff of generating graphics and sounds.


### [Famicom Party](https://famicom.party/book/)

A very nice free tutorial-style book that introduces both NES hardware and 6502 assembly.


## Videos

### Matt Heffernan series on Commander X16

The X16 is like a souped up, modern C64.  You can't currently buy X16 hardware, but you can learn
with the emulator, and then run on real when hardware when it is available.

<iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?list=PLPSrOWYluVLIJ1n-TsVb-BESL1tkSTRI_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### NESHacker on NES

NESHacker's content is primarily videos, and they are very well produced.

If you are interested in *hacking* existing games as well as making your own, I highly recommend these videos, although the final one is very technical so you may want to skip it:

#### Hacking NES

<iframe width="560" height="315" src="https://www.youtube.com/embed/oQXulNLXPdw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/HLzEhyvHBos" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/nxIWTIPS6Sc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/vc4P_Inb0iw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

#### NES Hardware

<iframe width="560" height="315" src="https://www.youtube.com/embed/GssRNEaKoPw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/7Co_8dC2zb8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/nAStgQzPrAQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/PwZEBE66an0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

#### 6502 Assembly on NES

<iframe width="560" height="315" src="https://www.youtube.com/embed/a8eKbrcBYPM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/RtY5FV5TrIU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/yEiNs7pKNh8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/2syeHRYx1Hg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/303HT9jDBdw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/6tNSxabHqRI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### [ChibiAkumas](https://www.chibiakumas.com/6502)



ChibiAkumas takes a very systematic approach to covering the entire subject in his many videos, as you would expect from a professional programmer mindset. This may not appeal to those with short attention spans who prefer want a tutorial with flashy results from the start and theory only introduced as necessary throughout.

ChibiAkumas is so systematic that he doesnt just cover 6502 assembly on one machine. He covers every 8 bit CPU on every machine. That’s a very completionist attitude to acquiring knowledge. To this end he provides library code that allows the same program to run on many different machines. I think this is fine (but unnecessary) during the initial stage of just learning the assembly. During the later stage of learning the machines, I suspect most will want to focus on a specific machine and so won’t use the library code.

ChibiAkumas provides a toolkit for Windows that includes a text editor, the VASM assembler, system emulators and his own library code.  It gets you set up fairly quickly.  However, it's all rather... idiosyncratic.  This isn't the text editor or assembler that most people would want to use for their project.  The emulators don't include debuggers because he prefers to write his own.

If you like his style, then the videos are informative, and you can follow along using the tools, but I wouldn't use this as the basis for my own projects.

Here's some videos I find interesting, but you can find many more **as well as text tutorials** on the website:

<iframe width="560" height="315" src="https://www.youtube.com/embed/lsvSZamCCBM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/nOPI0Xbj_Yc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/Yp5INk8c2bU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/mVz6DnCDWcY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/A9xF7shM_9k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/DdnaqSa629k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/pf57ytdyEo0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/8W6Yg6UAReA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/89wxjn9p_38" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Tools

### [8 Bit Workshop](https://8bitworkshop.com/)

8 Bit Workshop is a very impressive IDE for many 8-bit systems.  It combines text editor, C compiler, assembler, debugger, sprite editor, emulator and some library code.  It runs entirely in the browser so you don't even have to install it.  There some tutorial books for sale on the site, but it comes with several examples.

However, the examples and books mostly focus on C coding.  I tried to write an assembly program using the CA65 assembler and it worked at first and then stopped working.  Apparently the DASM assember works

### [CA65](https://github.com/cc65/cc65)

This is the most popular 6502 assembler.  It comes as part of CC65 C compiler.

There are binaries for Windows.  For Linux you might have to compile source, unless your distro includes it in the package manager.

If you want to try older, simpler alternatives:

[DASM](https://dasm-assembler.github.io/)

[VASM](https://www.chibiakumas.com/z80/vasm.php)

### [LLVM MOS](https://llvm-mos.org/)

A fork of LLVM compiler suite that targets 6502.  Getting C and similar languages
to run on 6502 is not easy and so only recently has this even become usable.

### [Prog8](https://prog8.readthedocs.io/en/latest/)

Prog8 is a high level language and compiler that is designed to be compiled to 6502 assembly much
more efficiently than C.  It currently supports C64 and X16 and looks to be one of the best
ways of programming these systems.

### [FCEUX](https://fceux.com/web/download.html)

A NES emulator with debugger.  Probably the best.  Binaries for Windows and Linux.

### [Nintaco](https://nintaco.com/)

Another NES emulator with debugger.  Nice because it's Java so cross-platform, but that may not matter now FCEUX has been ported to LInux.