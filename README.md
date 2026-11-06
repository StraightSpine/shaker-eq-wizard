# Shaker EQ Wizard

**Measure how your bass shakers really move, then build an EQ that
corrects them.**

A free, guided tool that runs in your browser. It plays test sweeps
through your shakers, reads the vibration your phone recorded, and works
out the parametric EQ filters that flatten the response. No install, no
account, and nothing you record leaves your device.

The wizard includes a built-in demo mode, so you can explore the
interface without connecting any equipment or recording a measurement. 

Made for people new to EQ, with settings that more advanced users can adjust.

![Shaker EQ Wizard Interface](Shaker%20EQ%20Wizard%20Interface.png)

## Why

Bass shakers (tactile transducers) never have a flat response. Some
frequencies are strong, others barely register, and the pattern changes
with the shaker, the seat and the amp. This tool measures that pattern
with the accelerometer in an ordinary phone, then fits a handful of EQ
filters to correct it.

## How it works

1.  **Play a sweep.** The wizard plays test sweeps through your shakers.
2.  **Record and upload.** A phone on the seat records the vibration
    with the free Phyphox app. You export the recording and drop it into
    the wizard.
3.  **Generate EQ.** The wizard shows the response before and after,
    gives you the filters, and can refine them with a second
    measurement.

A typical session takes about 15 to 20 minutes.

## What you need

-   A computer or device to play audio through your shaker amplifier
-   A phone with [Phyphox](https://phyphox.org) (free on [Google
    Play](https://play.google.com/store/apps/details?id=de.rwth_aachen.phyphox)
    and the [App Store](https://apps.apple.com/app/phyphox/id1127319693)
-   Somewhere to apply EQ on the shaker channel: a DSP such as a
    miniDSP, an AVR or amplifier with parametric EQ, or an app

## Features (v1.0)

-   Plays the sweeps and sets your level, all in the browser
-   Reads Phyphox recordings (CSV, Excel or ZIP)
-   Fits parametric EQ filters and shows the predicted before and after
-   Optional second pass to refine the filters from a re-measurement
-   Exports a filter list, CSV, a miniDSP 2x4 HD preset and a PDF report
-   Built-in demo with a simulated shaker measurement
-   Everything runs locally. No uploads, no tracking

## Roadmap

-   Send Phyphox results straight to the app, with no file to export and
    upload
-   Optional multi-pass sweeps at different seat or phone positions, for
    a more consistent result

## Safety

Sweeps move a lot of energy through your shakers and seat. The wizard
shows two warnings and a countdown before any sound, and a Stop button
is always on screen. Start with your level control all the way down and
raise it slowly.

## Credit

The method comes from Tyler Gauharou's Bass Shaker EQ workbook,
described on Simple Home Cinema in [Revolutionizing Bass Shaker
Equalization](https://simplehomecinema.com/2023/12/19/eqing-bass-shakers-a-new-approach/).
This wizard is an independent implementation of the same idea. It adds
automatic sweeps, filter fitting and file export, and it does not
contain or reuse his workbook. This project is not affiliated with Tyler
Gauharou or Simple Home Cinema.

## Run it yourself

The project is a single HTML file. Download `index.html` and open it in
a modern browser, or host it anywhere static, such as GitHub Pages.

## Limitations

-   Corrections are only valid for the exact setup you measured: same
    equipment, settings, seat and phone position
-   The miniDSP preset export targets the 2x4 HD. Other models can use
    the filter list or CSV
-   Tested on desktop browsers. Phone and Safari behaviour has had
    little testing, so please report problems

## Feedback

Found a bug or have an idea? Please open an issue in the [GitHub
repository](https://github.com/StraightSpine/shaker-eq-wizard/issues).

