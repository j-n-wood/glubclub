+++
date = '2026-03-01T20:22:14+13:00'
draft = false
title = 'More boot issues'
+++

# Dual boot issue

Turns out grub has issues with the old Windows drive - on cold boot.

Using BIOS to select the windows drive and then restarting - works fine.

Answer appears to be disable 'fast boot' in BIOS, as well as the already disabled 'fast start' from Control Panel - Hardware & Sound - Power - choose what the power buttons do.
