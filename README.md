# KW4EX — station software

Open-source tools I use to tie my **Elecraft KPA1500** amplifier, a
**FlexRadio FlexControl** tuning knob and an SDR program together. Written for
operators, not programmers: each one comes with a step-by-step guide.

## For Zeus SDR (Windows, Mac, Linux, Raspberry Pi)

Add-ons ("community features") that install from inside Zeus.

| | Latest | Get it |
| --- | --- | --- |
| **Elecraft KPA1500** — meters and buttons for the amp and its ATU; works with a FlexRadio too; the amp follows the VFO; Standby on Tune; "No antenna?" warning; a browser page for your computer, tablet or phone; power-on over the network | 1.4.4 | [**Download**](https://github.com/kw4ex/kpa1500-for-zeus/releases/latest) · [Guide (PDF)](https://github.com/kw4ex/kpa1500-for-zeus/blob/main/docs/guides/KPA1500-for-Zeus-guide.pdf) |
| **FlexControl Knob** — VFO tuning, AF volume, AGC gain and more; every press programmable | 1.0.1 | [**Download**](https://github.com/kw4ex/flexknob-for-zeus/releases/latest) · [Guide (PDF)](https://github.com/kw4ex/flexknob-for-zeus/blob/main/docs/guides/FlexControl-Knob-for-Zeus-guide.pdf) |

**How to download a Zeus add-on:** click its **Download**, scroll to **Assets** at the bottom of that page, and
click the file for your computer (the page has a table saying which). Don't click "Source code", and don't
unzip it. Older versions are on each add-on's Releases page.

More about each add-on: **[kpa1500-for-zeus](https://github.com/kw4ex/kpa1500-for-zeus)** · **[flexknob-for-zeus](https://github.com/kw4ex/flexknob-for-zeus)**

## For FlexRadio SmartSDR (Windows only, experimental)

| | Latest | Get it |
| --- | --- | --- |
| **KPA1500 SmartSDR Bridge** (experimental) — SmartSDR sees the KPA1500 as a **Power Genius XL** amplifier and a **Tuner Genius XL** tuner: meters, Operate/Standby, tuner Operate/Bypass/Tune, the amp follows your transmit frequency, C1/L/C2 bars; no serial cable; one-click installer. Mac, Linux and Raspberry Pi versions are still being tested. | 2.51 | [**Download**](https://github.com/kw4ex/kpa1500-smartsdr-bridge/releases/latest) · [Guide (PDF)](https://github.com/kw4ex/kpa1500-smartsdr-bridge/blob/main/docs/guides/KPA1500-SmartSDR-Bridge-guide.pdf) |

## For Thetis and NereusSDR (Windows only)

| | Latest | |
| --- | --- | --- |
| **KPA1500 SDR Bridge** — the KPA1500 with **Thetis or NereusSDR** (and Thetis HL2, SDR-VST3): an Applet window with meters, buttons and knob info, Thetis windows, safe TUNE, "No antenna?" protection, browser control panel, FlexControl knob support, LP-100A readings, one-click installer | 2.49 | [**Download**](https://github.com/kw4ex/kpa1500-sdr-bridge/releases/latest) · [Guide (PDF)](https://github.com/kw4ex/kpa1500-sdr-bridge/blob/main/docs/guides/KPA1500-SDR-Bridge-guide.pdf) |
| **FlexControl Knob for Thetis** — the FlexControl knob for Thetis, Thetis HL2 and SDR-VST3 with **no amplifier needed**: VFO tuning, AF volume, AGC gain and more; every press programmable; browser panel and Thetis window | 1.0.0 | [**Download**](https://github.com/kw4ex/flexknob-sdr-bridge/releases/latest)· [Guide (PDF)](https://github.com/kw4ex/flexknob-sdr-bridge/blob/main/docs/guides/FlexControl-Knob-for-Thetis-guide.pdf) |

## KPA Bridge — Thetis and FlexRadio in one program (Windows only, experimental)

Essentially the **KPA1500 SDR Bridge** and the **KPA1500 SmartSDR Bridge** combined into one program. Use it with Thetis, NereusSDR, Thetis HL2 or SDR-VST3, with a FlexRadio running SmartSDR, or with both (one radio on the air at a time). The two bridges above stay available.

| | Latest | Get it |
| --- | --- | --- |
| **KPA Bridge** (experimental) — the KPA1500 with **Thetis, NereusSDR, Thetis HL2, SDR-VST3 and FlexRadio SmartSDR** (the amplifier appears as a PGXL and the tuner as a TGXL). The amplifier follows the radio you last tuned or transmitted on. One-click installer, one shortcut that starts and stops the bridge, Applet window, browser control panel. Design and on-air testing by KW4EX. | 3.0g (experimental) | [**Download**](https://github.com/kw4ex/kpa-bridge/releases/latest) · [Guide (PDF)](https://github.com/kw4ex/kpa-bridge/blob/main/docs/guides/KPA-Bridge-guide.pdf) · [Project page](https://github.com/kw4ex/kpa-bridge) |

## Stand-alone tools for amateur radio

No amplifier and no SDR program needed.

| | Latest | Get it |
| --- | --- | --- |
| **RF Noise Map** (testing) — drive a route with up to **four radios** (an **SDRplay RSP1**, a **Hermes Lite 2**, an **ANAN** (Apache Labs, for example the ANAN-7000DLE MkIII) and low-price **RTL-SDR dongles**, in any mix; any radio can serve any of the four slots) plus a GPS; it logs the signal about every 10 feet on up to 4 frequencies and draws a street map of dots from blue (weak) to red (strong), so you can find noisy power lines and poles. Live panadapter and its own S-meter for each frequency, with sound and recording on the Hermes and the ANAN, and auto gain and gain per band for the Hermes. A compact, laptop-friendly screen with pop-up windows for drives, maps and tools. Practice mode, one-click installer, built-in health check, GPS finder and one-minute full test. The Hermes Lite 2, SDRplay and ANAN have been run on real radios; the RTL-SDR dongle support has only been tried with simulated dongles. Mac version is experimental (Hermes goes through a USB Ethernet adapter, Wi-Fi left on). | 1.6.0 (testing, untested with real dongles) | [**Download**](https://github.com/kw4ex/RFNoise-Mapping/releases/latest) · [Guide (PDF)](https://github.com/kw4ex/RFNoise-Mapping/blob/main/docs/guides/RFNoise-Mapping-guide.pdf) · [Project page](https://github.com/kw4ex/RFNoise-Mapping) |

## Good to know

- **Only one program should control the amplifier at a time.** Use the Zeus
  feature *or* the KPA1500 SDR Bridge, not both at once.
- **The KPA1500 SmartSDR Bridge also controls the amplifier.** Run only one bridge at a time (SmartSDR bridge
  or SDR bridge); each closes the other when it starts. Don't combine it with the Zeus feature.
- **KPA Bridge (experimental) also controls the amplifier.** Run only one bridge at a time (KPA Bridge, SDR bridge or SmartSDR bridge); each closes another that is running when it starts. Don't combine it with the Zeus feature.
- **Only one program can use the FlexControl knob at a time.** If you have both
  the KPA1500 SDR Bridge and *FlexControl Knob for Thetis*, switch off the knob in
  the bridge (the knob program's instructions show how).
- **RF Noise Map needs each radio to itself.** Close other SDR programs (SDRuno, SDRconnect, Thetis and similar) first; it can list and close them for you. The Hermes Lite 2 connects by network cable and needs no driver; RTL-SDR dongles need a one-time driver step (the guide shows it).
- Questions or problems: open an issue on the program's page.

## No warranty — use at your own risk

Everything here is shared by one radio operator, **as is**. There is **no
warranty of any kind**: no promise that it works, that it is safe, or that it
suits your equipment or purpose. Amplifiers, radios and antennas can be
damaged, and RF can be dangerous. You are responsible for checking that it
behaves correctly with your own station and for operating within your license.
The author is not liable for any damage or loss. Not made, approved or
supported by Elecraft, FlexRadio, SDRplay, Telepost, Thetis, NereusSDR, Apache Labs, Apple or Zeus.

73 de KW4EX
