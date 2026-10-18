### Hi, I'm Gage

I build the software and hardware that test things on a factory floor: test fixtures, the firmware inside them, the desktop
tools operators run, and the internal platforms that tie it all together. Day job is manufacturing engineering at
[Sensit Technologies](https://www.gasleaksensors.com/), a maker of gas detection instruments.

Most of that work is private, so here's what it looks like:

- **Production test fixtures, end to end.** ESP32 / Arduino firmware in C and C++, custom PCBs in EasyEDA (and KiCad), mechanical
  jigs in SolidWorks. Display, Bluetooth signal-strength, battery, leak, burn-in and sensor testers running on the line today.
- **Replacing legacy tooling.** Rewrote a C# sensor programmer in Rust and swapped a proprietary I²C adapter for a
  Raspberry Pi Pico bridge with a small serial protocol of my own.
- **An internal platform for manufacturing engineering.** Go backend, Svelte frontend, and a Tauri desktop client
  that identifies the fixture on a bench over serial, fetches the matching tool, and launches it. Tools post results
  back for yield tracking. Includes CI, deploys, and a two-person release approval flow.
- **Search over a decades-old engineering archive.** Full-text search over a ~37k-document fileshare for the whole
  engineering team, built in Go on SQLite FTS5 with ranking that learns from what people open.
- **Instrument control and vision.** PyVISA / DAQ-driven characterization rigs (thermistor binning with
  Steinhart-Hart matching), and camera-based OCR that reads instrument displays with a CNN plus a vision-language model.

### Things you can actually run

| | |
|---|---|
| [**lp-engine**](https://github.com/gage-marshall/lp-engine) | A native Rust runtime for the Nintendo DS dating sim *LovePlus+*, with a full English translation and up to 4× rendering on wgpu. Reverse engineered from the original game. |
| [**ttyflix**](https://github.com/gage-marshall/ttyflix) | Streams video as ANSI art over Telnet and SSH. Try `ssh anything@nisemonogatari.com -p 2222` ([deployment](https://github.com/gage-marshall/Nisemonogatari-Telnet)). |
| [**Carpenter930**](https://github.com/gage-marshall/Carpenter930) | Safe-Rust library (plus C FFI) for generating program files for a Carpenter 930 wire cutter, reverse engineered from the machine's format. |
| [**LF-Parser**](https://github.com/gage-marshall/LF-Parser) | Decodes and re-encodes Fisnar / Everprecision dispensing-robot programs, round-tripping byte for byte. |
| [**CriticalRegion**](https://github.com/gage-marshall/CriticalRegion) | A server-authoritative daily-seed puzzle game with accounts, friends and leaderboards (FastAPI). |

### Usually reaching for

Rust · Go · C / C++ (ESP32, Arduino) · Python · Svelte / TypeScript · EasyEDA · KiCad · SolidWorks · SQLite / Postgres · Docker
