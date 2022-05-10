1. ~~Setup Odin language server (and included formatter) for Neovim~~
	  - ~~[Odin language server](https://github.com/DanielGavin/ols)~~
	    - ~~[Issue: Language Server not Starting](https://github.com/DanielGavin/ols/issues/105)~~
1. Learn Odin
	  - ~~[Odin Overview](https://odin-lang.org/docs/overview/)~~
	  - [Odin Demo](https://github.com/odin-lang/Odin/blob/master/examples/demo/demo.odin)
	  - [Odin Examples](https://github.com/odin-lang/examples)
1. Create basic data structures in Odin
	  - Reference: [Pointers in C](https://github.com/mkohlhaas/Pointers-C-Programming)
	  - singly linked list
	  - doubly linked list
	  - binary tree
	  - tree
	  - ...
1. Guideline: Use same [libraries as VCV Rack](https://github.com/VCVRack/Rack#software-libraries)
1. Wavetable Oscillator
	  - Algorithm in Odin with SIMD support
	  - Use existing wavetables from Odin 2, create handishly with Audacity, or whatever, ...
	    - Create wavetable for basic wave forms: sine, triangle, sawtooth, square
	  - Expose Oscillator as [Clap](https://github.com/free-audio/clap) plugin
	  - Implement waveshaper algorithms
	  - MIDI, UI, and signal flow should run in separate threads
	  - Build UI around Oscillator with NanoVG
	    - See [UI of EmberGEN](https://www.youtube.com/watch?v=mVmcGlQa6_U)
	    - Create Odin bindings to NanoVG
	    - [Create Odin bindings to NanoSVG. See VCV Rack how they do it.]
	    - Use [existing binding to GLFW](https://pkg.odin-lang.org/vendor/glfw/)
	    - Design hierarchical layout system
	    - Design hierarchical event propagation system
	  - Micro Sampling
	    - Record audio
	    - Load audio
	    - Cut audio
	    - ...
	  - Add MIDI support with RTMidi
	    - Create Odin bindings to RTMidi.
	    - [C interface to RtMidi](https://www.music.mcgill.ca/~gary/rtmidi/group__C-interface.html)
	  - Support for Ableton Link.
	    - [C Interface to Ableton Link: c-wrapper](https://github.com/magdaddy/ableton-link-rs/blob/master/c-wrapper/link_rs.cpp)
	    - [C Interface to Ableton Link: link-c](https://github.com/artfwo/link-c)
1. Create modules
	  - Filters
	  - Effects
	  - LFOs
	  - Envelopes
	  - Waveshapers
	  - Mixer (2-way): Could be used as a directive for spawning threads. Two threads in, one thread out.
	    - In general when signal flow forks
	    - Input 1, Output Many
	  - Splitter
	  - ...
1. REST Interface
	  - Logon, Logoff
	  - Update license key
	  - Upload/download/search/... patchsets
	  - Vote for patchsets
	  - ...
1. Musical Pattern Generator à la [ScribbleTune](https://scribbletune.com/)
