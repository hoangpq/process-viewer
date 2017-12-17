# process-viewer [![Build Status](https://travis-ci.org/GuillaumeGomez/process-viewer.png?branch=master)](https://travis-ci.org/GuillaumeGomez/process-viewer)
A process viewer GUI in rust. It provides current status of your processes (cpu and memory usage) and your system (usage of every core and of your RAM, and the temperature of your components if this information is available).

Please run it in release mode to have good performance:

```bash
cargo run --release
```

## Screenshots

![screenshot](http://guillaume-gomez.fr/image/screen1.png)
![screenshot](http://guillaume-gomez.fr/image/screen2.png)

It can be run on the following platforms:

 * Linux
 * Raspberry
 * Mac OSX

### Running on Raspberry

It'll be difficult to build on Raspberry. A good way-around is to be build on Linux before sending it to your Raspberry:

```bash
rustup target add armv7-unknown-linux-gnueabihf
cargo build --target=armv7-unknown-linux-gnueabihf
```

## Donations

If you appreciate my work and want to support me, you can do it here:

[![Become a patron](https://c5.patreon.com/external/logo/become_a_patron_button.png)](https://www.patreon.com/GuillaumeGomez)
