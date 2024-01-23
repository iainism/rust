# Cargo Embed #
Debug: `cargo embed --features v2 --target thumbv7em-none-eabihf`

Release: `cargo embed --features v2 --target thumbv7em-none-eabihf --release`

# GDB #
Start-up: `gdb-multiarch ../../target/thumbv7em-none-eabihf/debug/`

Connect: (gdb)`target remote :1337`

Breakpoint at entry to main: `break main`

See next line: `stepi`

Continue (e.g. to breakpoint): `c`

Step to next line: `next`

See list of breakpoints: `info break`

See initialised variables: `info locals`

# Minicom #
To monitor serial: `minicom -D /dev/ttyACM0 -b 115200`
