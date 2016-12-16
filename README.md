# Raster

[![Build Status](https://travis-ci.org/kosinix/raster.svg?branch=master)](https://travis-ci.org/kosinix/raster)

An image processing library for Rust. 

## Pre-Alpha Status

Raster is currently in pre-alpha; There will be breaking changes between versions. The API will stabilize once it reaches 0.1.0. From then on it will follow semver.

## Documentation

Examples and API are [here](https://docs.rs/raster/)

## Current Features

* blend - Combine 2 images using normal, difference, multiply, overlay and screen.
* clone - Clone an image.
* crop - Crop image with support for textual anchor points and offsets.
* equal - Compares if two images are equal.
* fill - Fill image with color.
* resize_fit - Resize an image to fit within the given width and height. 
* resize_fill - Resize image to fill all the space in the given dimension.
* resize_exact - Resize image to exact dimensions ignoring aspect ratio. 
* resize_exact_width - Resize image to exact width.
* resize_exact_height - Resize image to exact height.
* save - Save to raster formats JPEG, PNG, and GIF
* similarity - Compare two images to see how similar they are.
* blur - Blur image using gaussian or box.
* convolve - Apply a convolution matrix.
* sharpen - Sharpen image.
* rotate - Rotate to any arbitrary size in clockwise or counter-clockwise direction.


Checkout the docs for more info.

## Core Principles
* Keep everything simple
* Stick to primitive or simple types if possible, use advance types when neccessary
* Stick to module + functions if possible, no unneccessary abstraction (eg. OOP)
* Speed over abstraction
* Make function names user-friendly by using common or simple English words
* All functions THAT CAN return an error should return the Result type, otherwise return an appropriate type

## License
- MIT License

## To Do List

* ~~More examples and add pictures in docs~~
* Implement bicubic interpolation
* Add geometric transformations
* ~~Add filters and convolution~~
* Memory and perf improvements
* Reduce dependency to image decoders/encoders