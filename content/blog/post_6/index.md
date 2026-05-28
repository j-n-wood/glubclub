+++
date = '2026-05-27T12:22:14+13:00'
draft = false
title = 'iPhone update'
+++

# iPhone update

## Why

So, there is an update due for the phone. For work, I have product apps that we test on our phones, so updating is sort of needed.

Problem - phone is a little old and 'only' has 64 GB of storage. 13.4GB free required to perform the update.

## First attempt

Unloaded a bunch of apps, dropped a bunch of downloaded music, cleared caches - got to enough space free. Quite a bit of stuff to re-enable once done, but that's ok.

Download update. Leave that going while doing other jobs. Check back.

Update not applied. Hmm.

Try again. Need 13.4 GB free space. Err, I had that. What happened?
System data now taking more than 20 GB. System + OS now taking more than 30 GB.

## Help me, bot

How to clear this?

Lots of suggestions for using the phone storage tool, look for the update download, and kill it. No such thing listed.

Various other suggestions to convince the phone that it can drop an unused download. Nope.

## What worked

Turn off iCloud storage for photos. Restart. Frees up 12GB or more.

Update proceeds OK at this point, turn iCloud back on.

Yay software.

## Next weird thing

For my next trick, I replaced the old, telco supplied router with a modern mesh network Wifi. Hooray, no more dead spots in the kitchen!

Some older things (receiver, printer) less happy with new network. Workaround - mesh system has a secondary network for old devices (_IoT). Nice! Built in support for stuff you can't upgrade. Slight issue with connecting with app software - not on the same network, so some link functions seem to break.

Answer: wire the receiver into a mesh node. Wires _work_. Just wish the mesh nodes had more than two ports. Can maybe chuck a cheap switch on there, but that needs another power source.

### The iPhone again

But now some new weirdness - phone stops opening web pages if I'm on the far side of the bedroom. Eh?

Wifi strength is good.

Other apps with network connection seem OK.

Move 2m closer - OK. Step back - new tab - 'network connection lost' message. I call bullshit, as existing tabs still work. Wikipedia is fine, links work, can jump through loads of pages. Just new tabs. Even entering an explicit address (you don't need to search for hat, safari, nor you, chrome) - no good.

The bot suggests some sort of DNS issue when signal strength is tenuous. Signal strength looks fine to me, all sorts of already-connected stuff is fine. 2-3 bars Wifi.

Finally find a suggestion to _change default search engine_. This works! I'm sure there is some totally BS reason why. DuckDuckGo is my new friend. Apparently I should be able to change back to default google, but if I do, the problem recurs.

Yay software again. I'm sure the features that are breaking are 'better' somehow because of this feature. More convenient! SHow stuff in you face withing moments that you probably didn't want! Hooray! And no fallback for 'old' devices that are still in real terms very powerful, or robust handling of non-happy-path.

I'm OK with DuckDuckGo.
