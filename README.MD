testing

Note 7/17/2026: If you put CP on each x0 x1 y0 y1 channel that's ported into the calculated parameter, it forces the calculated record to calculate in some intermediate state when some channels are updates but others aren't. What you can do instead is use a forward link on whichever BPM channel is processed last. If you check with TPRO, the x0 is processed first and finishes last. So you put the SCAN ".1 second" and the FLINK on this channel to the computed parameters, and then you won't have weird jumps where calculated parameters are calculated too many times. 
