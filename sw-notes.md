---
layout: page
title: sw-notes
permalink: /sw-notes/
---
## Installing rtags.

-- Download the code opencv and rtags.
-- Building opencv.
cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=1 .
make

-- Build rtags

cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=1 .
make

Start the RTags daemon (rdm) -- ./bin/rdm &

Index the RTags project, and wait until rdm is silent -- ./bin/rc -J .

rtags usage:

#04-22-2018#

Installing auto-complete in Vim.

YouCompleteMe was complaining that the vim version was lower than supported.
Installed the vim 8. And once the Valloric/YouCompleteMe plugin is installed,
run the ./install.py under the bundle in .vim.

Trying to get the color histogram equalization done in color space.

#Exploring the new Vim.

Installed the latest version.

Vim 8.1

Neovim vs Vim showdown.

Gonna try neovim next week.

Terminal emulator accelerators on GPUS. Wow.

# Hough transform trip:

Bresenham Alogrithm - 
