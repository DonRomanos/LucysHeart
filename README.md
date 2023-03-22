# LucysHeart

The heart (or brain) of something special. This is my attempt at a central control unit for my wife's and mine self built camper van. Let's see what it becomes.


## Cross compiling for the raspberry pi

Rust contains a nice cross compiling crate called [cross](https://github.com/cross-rs/cross). With it cross compiling works like a charm.

To install it:
```
cargo install cross --git https://github.com/cross-rs/cross
```

Then you can cross compile just like you would build any other application with cargo. This is the command line I use to cross compile for my raspberry pi.

```
cross build --release --target armv7-unknown-linux-gnueabihf
```

Cross uses docker and requires `dockerd` to be running on the system.