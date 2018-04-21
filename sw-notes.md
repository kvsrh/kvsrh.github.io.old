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
