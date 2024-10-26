---
layout: page
title: Graphics Render
description: A simple ray tracing renderer.
img: assets/img/2000x2000spp3000.png
importance: 1
category:
---

[[Code]](https://github.com/BakaSea/GraphicsRender)

## Path Tracing

Model:

* Sangonomiya Kokomi/miHoYo/观海子
* Bunny/Standford University

1000x1000 spp3000:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1000x1000spp3000.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

2000x2000 spp3000:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/2000x2000spp3000.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Sampler

All 1000x1000 spp16.

Use different sampler in light sampling.

### Uniform

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/uniform.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Random

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/random.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Blue Noise

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/bluenoise.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Polygon Light

|     Quadrilateral      |         Pentagon         |         Hexagon         |
| :--------------------: | :----------------------: | :---------------------: |
| ![](https://github.com/BakaSea/GraphicsRender/blob/main/imgsrc/square.png?raw=true) | ![](https://github.com/BakaSea/GraphicsRender/blob/main/imgsrc/pentagon.png?raw=true) | ![](https://github.com/BakaSea/GraphicsRender/blob/main/imgsrc/hexagon.png?raw=true) |

## Microfacet Model & Multiple importance sampling

| $\alpha$ |       BRDF Sampling       |      Light Sampling       | Multiple importance sampling |
| :------: | :-----------------------: | :-----------------------: | :--------------------------: |
|   0.01   | ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/brdf-0.01.png) | ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/light-0.01.png) |  ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/mis-0.01.png)   |
|   0.1    | ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/brdf-0.1.png) | ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/light-0.1.png) |  ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/mis-0.1.png)   |
|   0.2    | ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/brdf-0.2.png) | ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/light-0.2.png) |  ![](https://raw.githubusercontent.com/BakaSea/GraphicsRender/main/imgsrc/mis-0.2.png)   |