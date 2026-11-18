# Anamorphic SD Before Upscaling: Non-Square Pixels, 1.185× Stretch, Measured

720×480 with SAR 32:27 stores 16:9 on a grid 15.6% coarser horizontally. Measured: the correct upscale caps detail at 360 cycles/width and everything above folds back (400→320, 600→120); PSNR ranked a 15.7%-wrong image first. Also measured: the destretch width cancels out (−0.008 dB for 852 vs 854), pad keeps the old SAR and produces an 18.5% stretch error, and 4:2:0 quantises chroma edges to a 2-pixel grid.

**Read it with the tables and the reproduction snippets:** <https://celticgemini001.github.io/upgolab-anamorphic-sd-upscale/>

## About this repo

This repository exists to serve one measured article. Every number in it came from
ffmpeg and numpy run on real files on this machine — the commands are in the page so
you can re-run them and get the same rows. Where the measurement contradicted the
hypothesis, the page says so.

## The tool behind the notes

<https://upgolab.com> — browser-based AI upscaler for photos and short video.

## Index

All the guides are cross-linked from the hub:
<https://celticgemini001.github.io/upgolab-tools/>
