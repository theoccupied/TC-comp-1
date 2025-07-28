# TC-comp-1
The main repository for accessing challenges for the first architecture building competition in Turing Complete.  
Playing these challenges is as simple as putting the folders into your Turing Complete campaign folder, then loading them with the console (comp_1 is the menu to access all other challenges, so that's a good pick).  
If you wish to take part in the competition, tell me (clearly and directly, please), and I will incorporate you into the official text file with a number.  
If you have any questions, just ask me and I'll explain what and why.  

# Main Rules
This competition takes place in the Alpha branch, since it is the one that custom levels can be made for.  
There are two main phases in the state of this competition: [Before Challenge Reveal](/README.md#bcr) and [After Challenge Reveal](/README.md#acr).

### BCR:
  Only 'visible' challenges can be viewed and worked through (these are the ones available on the repo right now).  
  In this time, competitors should create their architecture and submit it to me (theoccupied) through private means (well, at least not anywhere public) using [this tool](https://github.com/MegaIng/tc-arch-extract) (requires Python 3.10+). Discord DMs are preferred but if you want to do this some other way that is fine as long as I'm aware of the method you're using.  
  Optionally, a competitor can also submit a custom level to be included ACR. Note that the level must be deemed 'reasonable' by me in order for it to be included. That means no bytecode that's suspiciously similar to your architecture's machine code.  

### ACR:
  Every challenge will be revealed, and every competitor must complete these challenges with the same architecture that they submitted, with no modifications apart from RAM contents.  
  After completing each challenge, competitors should submit their code and ISA that they used to complete the challenge. I will then run the architectures on more comprehensive tests on my end, to verify that the challenges have been satisfactorily completed using the same architecture. Challenge solutions should solve the general problem posed, not exploit limited test cases in `test.si`.  
  If a challenge completion fails verification the competitor will be informed of the problem so they can fix their solution.
  Once every competitor has finished (or otherwise decided to stop), scores will be counted up as the sum of in-game scores (with modifications as according to the second section of rules) over all challenges.  
  The overall winner is the competitor that has the lowest total score (I may announce other places for outstanding/unique performances).  
  If a competitor does not finish a challenge, they will be given a score equal to double the worst performance on that level by other competitors.  

All architectures must conform to the second section of rules below:

# Architecture Rules
This section is subject to change if more cheese comes to my attention.  

No more than 1 architecture may be used to complete all the levels. If you submit more than 1 architecture, the most recent architecture submitted will be the one that is verified, unless it was submitted ACR.  

Every architecture only needs to connect to an 8 bit input and an 8 bit output. No other I/O is required. SSD space is also not required.  

Every architecture should have these minimum specs (the visible challenges are designed to all but force this):  
  - 16 bit or larger arithmetic ops
  - 16 bit or larger logic ops
  - 256 bytes of memory, + additional registers for shuffling data and holding addresses and counters.
  - Space for >1000 <ins>instructions</ins> (especially important if your architecture is not very powerful)
  - Must be turing complete (duh)

Ignore these minimum specs at your own risk. At the same time, these are still not ideal specs. They will just allow you to complete all the challenges.  

Aiming higher than minimum specs, the competition will be geared towards architectures that are:
- Arithmetically capable
- Flexible and free of limitations

And, of course, very optimised.
My goal is not to promote the architecture that most closely matches the minimum specs, my goal is to find the architecture capable of tackling any problem (within reason).

RAM will be scored differently in this competition. A new alpha version will come out with fixed scoring for RAM before the competition starts, and thus that scoring will be used.  

### Cheese Blacklist
  I expect everyone to be sensible about this, but I will lay the rules out anyway.  
  It's likely a lot of the scoring-related cheese will get patched out before the competition starts, but I'm covering all my bases here.

  - No bugs or glitches.
  - No free OR gates.
  - No free AND gates.
  - No free (A && ¬B) gates.
  - For that matter, no free gates whatsoever.
