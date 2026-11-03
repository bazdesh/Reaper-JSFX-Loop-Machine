Reaper JSFX loop machine

<img width="917" height="618" alt="image" src="https://github.com/user-attachments/assets/d71310bc-cbaa-4238-ab76-3c88ad1e7edb" />


A single-loop looper for reaper, written by claude, in jsfx. Made because I coudlnt get guitar rig 7 and yabridge to communicate. 
Buttons/idea/function based on the Loop Machine in GR7.

features:

- one loop, locked to the project tempo, length set in bars
- record start: immediately, on the next bar, or when you start playing (level trigger)
- overdub up to 15 layers, with undo and redo per layer (idk, claude wanted some limits because jsfx and memory; this has been more than enough for me, you can theoretically record infinitely into just one layer)
- hold-to-double button: repeats the loop twice as long so you start with a short lick and then do a longer chord progression over that
- input level, pan, and mode (stereo, mono, or off)
- output level with a zero-latency limiter
- live input monitoring on/off
- keeps playing if you stop the transport, and re-syncs to the bars when you hit play again
- simple gui, main buttons are big, mouse only

known limits: recording needs the transport running, tempo changes mid-loop will throw the sync off, and loops aren’t saved with the project.

install: drop loop_machine.jsfx into reaper’s Effects folder.

