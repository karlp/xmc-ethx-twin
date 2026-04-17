# Ethercat + Ethernet using the same physical ports

XMC4800 has ethercat ports _separate_ from ethernet, and you're expected to add a third port.

That sounds super dumb.  

I'm not trying to use ethernet and ethercat at the same time, but in an environment without ethercat, or, prior to commissioning, being able to use one of the ports as a plain ethernet port would be "nice"

This board attempts to evaluate whether that is actually possible, by using two MII phys (the ethercat ports only support MII in xmc4800) with one of them, connected in parallel to the ethernet interface.  I'm hoping to be able to just switch IOs off to the "unused" interface, and.... hope the trace stubs are minor enough to not care about...


