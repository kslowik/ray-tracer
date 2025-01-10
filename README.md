# raytracer

## Project

I implemented simple ray-tracer based mostly on "Ray Tracing in One Weekend" and partially on "Ray Tracing: The Next Week".


In the first part I implemented basic features, parallelized rendering using rayon and added option to create custom scenes using JSON description.

In the second part I improved code quality, added some reasonable tests and made creating scenes in JSON much easier.
Apart from that I added some new features of which most interesting are in my opinion textures (both sky texture and texture mapping for spheres).

I also tried to do GPU parallelization but it turned out to be much harder than I thought and I don't know if I could even do it purely in Rust.
So instead I focused on adding more features.

## Usage
```
$ cargo build --release
$ ./target/release/raytracer data/test_scene.json picture.png
```
I recommend trying to create picture from impressive_scene.json and/or trying to make your own scene.
