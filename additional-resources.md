# Other resources that might be worth looking into

Some of these links might also be scattered around this repo, but it's probably useful to collect them on this page too.

 - [**rutabaga**](https://github.com/wrl/rutabaga/) - [@wrl](https://github.com/wrl) made his own OpenGL GUI crate in C called `rutabaga`, which he used for his commercial VST [cadmium](https://lhiaudio.com/cadmium/). He's interested in eventually porting some of the ideas over to Rust, but in the meantime he's open to people looking into it and getting ideas for their own Rust toolkits. Relicencing from 2-clause BSD is possible if needed; that and other questions about rutabaga can be directed to him (he's pretty active on [the RustAudio Discord](https://discord.gg/QPdhk2u)).
 - [**rtb-rs**](https://github.com/rust-dsp/rtb-rs) is one such attempt at (very vaguely) "porting some ideas" of `rutabaga` over to rust. `rtb-rs` is a joint-effort by a few members of the [RustDSP GitHub organization](https://github.com/rust-dsp). Unfortunately, development has ultimately stalled for the time being, but some of the code might still be useful to reference in the future (particularly, how to structure a cross-platform crate composed of platform-specific modules). I wrote a little bit more about the project [on this page](https://github.com/crsaracco/vst2-gui-research/blob/master/gui-from-scratch.md#rtb-rs).
 - [**vst2-window**](https://github.com/crsaracco/vst2-window) is another (very similar to `rtb-rs`) attempt at creating a cross-platform crate "from scratch", by [@crsaracco](https://github.com/crsaracco). The main idea that's different from `rtb-rs` is to let the platform-agnostic API part grow more organically than it did in `rtb-rs`. Some [platform-specific VST prototypes were made](https://github.com/crsaracco/vst2-gui-prototypes) for some pre-development research, which might be useful to reference in the future. I wrote a little bit more about the project [on this page](https://github.com/crsaracco/vst2-gui-research/blob/master/gui-from-scratch.md#vst2-window).