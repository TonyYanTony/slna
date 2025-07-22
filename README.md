# slna
A cross-platform software LNA (Low Noise Amplifier) for SDR (Software Defined Radio).

**Work in progress, use at your own risk.**

## Philosophy

The goal of the slna project is to provide software radio enthusiasts with a simple, no-cost rough substitute for hardware LNA, entirely via software algorithms. The project is intended to work as an audio pipeline that takes input from SDR software output (*tested on SDR++*), processes the audio real-time, and directly outputs to audio devices.

The slna project is largely based on the works of [PortAudio](https://www.portaudio.com/) and [LibTorch](https://docs.pytorch.org/docs/stable/cpp_index.html).

## Installation

### Prerequisites

- [gcc](https://gcc.gnu.org/)
- [cmake](https://cmake.org/)
- [portaudio](https://www.portaudio.com/)
- [libtorch](https://pytorch.org/get-started/locally/)
- any virtual audio loopback device, see below

### Virtual Audio Loopback Device

#### Windows

Although I strongly prefer open-source software over proprietary, there are yet no simple and mature open-source virtual audio loopback software available for the Windows platform. As a result, the majority of people are recommended to use VAC (Virtual Audio Cable), a proprietary and freemium app.

*As an open source alternative, you can also try jackaudio, but I haven't tested it yet.*

1. Download VAC Lite from [here](https://vac.muzychenko.net/en/download.htm).

2. Install VAC Lite.

3. Setup the virtual audio loopback device according to the steps of the [Manual](https://vac.muzychenko.net/en/manual/simple.htm)


