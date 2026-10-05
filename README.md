# KISS cpu
Files for my riscV cpu in logism. Being used for presentation in Drexel's Tinker Tank

# Current State of the Project
This is currently fairly incomplete at the moment. I am evolving this project from the mips cpu I was working on, so there is files from that in here currently. As well as some non-cpu files I'm using for presentations.

I'll get around to organizing this better later.

# Goals
For now the goal is to implement a riscV cpu using the I32 instruction set. This might be expanded in the future depending on how I want things to evolve.

# Design Rules
1. The name is KISS -> Keep it Simple Stupid. The design should prefer easy understanding rather than optimization, while still exploring good designs. A good example of this is using a CLA Adder rather than a Ripple. It is more complex but there is a reward for that, and it is still structured in an understandable way, or at least as best as I can make it.
2. Everything is built up from 2 input logic gates. This is done to cohere to boolean logic better. I know that 3 and 4 input gates would make some things cleaner. Also I started that way and it feels like id be annoyed changing it now. So yay gate cascades.
3. For the sake of performance I had to start using logism built-ins for mux's, decoders, and shifters. Things were starting to get very laggy. But everything must be implemented at least once before I can use a built in. So there are examples of everything in the files.
4. Logism doesn't handle memory cells very well. I have some version implemented but that is a big use of the built-ins
