+++
title = "An investigation on ray tracer parallelization"
slug = "raytracer"
template = "portfolio-entry.html"
[extra]
tags = ["graphics", "C++"]
opt_preview_img = ["ray01.jpg", "default", 4, 2]
+++

{{ image(src="ray02.jpg", stretch=true, can_toggle_full_width=true) }}

Future shines bright for ray tracers, and although the theory behind them is fairly simple, they are magnificently slow.

I investigated different parallelization techniques to speed up a path tracer. I used *[smallpt](http://www.kevinbeason.com/smallpt/)* as a base, but to keep it as simple as possible I removed unnecessary features such as pixel subdivision and tent filter.

The two methods that I implemented are [OpenMP](https://www.openmp.org/) for CPU parallelization and [CUDA](https://developer.nvidia.com/cuda-zone) for GPU parallelization. They both target the loop that iterates through all the pixels.

You can already find an OpenMP in *samllpt*, and the only difference is one single line. CUDA implementation took a bit more effort, especially because when you put too much data into the GPU there's no easy way to tell whether it's going to crash. It just happens.

By the end, an image with a resolution of 1024 &#215; 768 pixels with 100 samples per pixel took:

* 94 seconds with sequential code
* 15 seconds with OpenMP
* 2 seconds with CUDA

{{ article_buttons(buttons=["Source code", "https://github.com/marcomoroni/set10108", "Report", "https://github.com/marcomoroni/set10108/blob/master/Report.pdf"]) }}
