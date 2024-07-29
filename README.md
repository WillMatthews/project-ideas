# project-ideas
"Fun" project ideas that I might do if I have enough time. Ranked in the order that I want to do them.

A lot of these claims need citations. Read at own risk.

## squeal
there are no good SQL linters out there for postgres.
Might make sense to make one in golang.

## is-micropackage
I have [opinions](https://willmatthews.xyz/posts/npm-micropackages/) on micropackages - none of them good.
For the sake of comedy and writing an npm package, I want to write `is-micropackage`, which determines if other npm packages are micropackages.
This may be a bit nontrivial, but could be worthwhile.

## Trunp-Or-Markov
I think a Markov chain is about the right level of complexity to approximate Trump.
This project would be making a small game where you have to guess if you're reading a real trump tweet or a markov-chain-generated fragment.

## RISC-V-ML

### The Motive
RISC-V is an interesting standard which offers an exciting avenue toward RISC chips to becoming commonly used.
RISC-V, however, has no counterpart for ML, everything that does ML seems to be CISC.

### The Competition
The chip market for ML is dominated by NVidia. NVidia make GPUs, which while good for video rendering, aren't quite perfect for some ML tasks.
Some companies are trying to make chips bespoke for machine learning.
This part of the competition seem to have the same flaws, every company is in some sort of death spiral of "push the hard problem to software", which never works.
Look at Cerebras, Graphcore etc, it's very much a repetitive case of WOW BIG CHIP LOTS OF CORES!
Well, good luck controlling them and managing the communications between the chips.

### The Solution
A RISC-V like chip may be the way to make this really work. I am not sure what the limitations are, most power usage is in transport of data, and that may be solvable (?) but requires more reasearch.

I want to flesh this idea out a bit more and see where the journey takes me - who knows, I might finally learn hdl.


## UVideo (UV Space Video)

### The Motive
The basal idea of UVideo is that there is no good method of sending "high res" blurred video.
We can send high res video, we can then blur it, but that's not the same - this means there is a high bandwidth requirement.
We can also send low res video, and blur that. That's a slightly better solution, but it's still fundamentally flawed.

What if we wanted to send blurred video for privacy reasons? 'Remote working solutions' frequently use blurred video as avatars, but their "implementation" (if you could call it one) is to just send a video stream and then do a `filter: blur(20px)` on it. (need link) 
Others send a blurry jpeg, which is highly compressed and looks vile.

### The Potential Solution
What if we could send some Fourier space?
Sure, we have existing video sharing methods, and they are heavily optimised, but the same could be done for frequency space.
Free the shackles of your mind that everything must be done in actual space and work in the freuquency domain - it's much nicer.

### Notes
I've tried this in js and python. Fundamentally we need to FFT2 the image three times (r,g,b channels).
FFT2 is quite expensive, so I was only able to get a couple of frames per second. womp womp.


## Pepper Grinder
tbd

## Piss.dev
### The Motive
I bought a funny domain.

### The Gag
Create an estimator for your hydration (and eventually when you piss).
