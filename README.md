# VVVVVV.OpenFPGAOS.Analogue_Pocket
Port of VVVVVV for the Analogue Pocket via OpenFPGAOS-SDK

This is a port of [VVVVVV](https://github.com/TerryCavanagh/VVVVVV) by [Terry Cavanagh](https://github.com/TerryCavanagh) for the Analogue Pocket via [OpenFPGAOS](https://github.com/openfpgaOS) by [ThinkElastic](https://github.com/ThinkElastic).

This is version 2.4.4 of the game running on the Analogue Pocket. 

Controls are customizable via the In-Game Menu. 

VVVVVV's is hard-coded for the UP and DOWN buttons to flip. Since the Analogue Pocket's D-Pad may trigger mis-inputs, there is an option in the Core's Settings Menu to disable UP/DOWN Flips on the D-Pad. 

Game-play has been optimized to perform fluently on the Pocket, however if you're experiencing lag, try to keep the Game-play at 30 FPS which can be toggled in the Settings Menu. My Analogue Pocket is running firmware 2.7 and runs great on there. There may be some lag on levels with lots of moving graphics, but I try to optimize them. 

# Disclaimer
This was created solely through Codex/Claude. The OpenFPGAOS Core is already stable and I thought it would be nice to try to get VVVVVV to run on the Analogue Pocket, and possibly try other games.

I have not tested it with Analogizer or the Analogue Dock, however it should perform the same as other games. 

## Building the VVVVVV Assets

The VVVVVV game data is **not included with this repository or release**.

You must provide your own legally obtained copy of VVVVVV and build the Analogue Pocket asset files locally.

# Requirements

- A legally obtained copy of **VVVVVV**
- Git
- Python 3, if required by the asset-building script
- This repository

The original VVVVVV game assets must not be redistributed with builds of this port.

### 1. Obtain VVVVVV

Install or download your legally purchased copy of VVVVVV.

Locate the game's `data.zip` file.

Depending on where you purchased the game, its location will vary. You only need the original game data; you do **not** need to compile the VVVVVV desktop application itself.

### 2. Clone this repository

```bash
git clone <YOUR-REPOSITORY-URL>
cd <YOUR-REPOSITORY>
```

### 3. Copy `data.zip`

Copy your VVVVVV `data.zip` into the location expected by the asset-building tools.

For example:

```text
<repository>/
├── tools/
├── data.zip
└── ...
```

Do not extract `data.zip` unless the build instructions specifically require it.

### 4. Build the Pocket assets

Run the asset-building command included with the repository.

For example:

```bash
python3 tools/build_assets.py data.zip
```

or, if the repository uses `make`:

```bash
make assets
```

The script converts the required VVVVVV data into the format used by the Analogue Pocket port.

### 5. Copy the generated `Assets` folder

After the conversion completes, you should have an output resembling:

```text
Assets/
└── <platform-name>/
    └── common/
        └── <generated VVVVVV files>
```

Copy the generated `Assets` directory to the **root of your Analogue Pocket SD card**.

Merge it with the existing `Assets` directory rather than replacing the entire directory.

Your SD card should then contain both the installed core and the locally generated VVVVVV assets.

### 6. Start VVVVVV

Insert the SD card into the Analogue Pocket and launch the VVVVVV platform/core through openFPGA.

If the required asset files were generated and installed correctly, the game should start normally.

## Asset Distribution

This project does **not** distribute VVVVVV's original commercial game assets.

The asset-building tools are intended to allow users who own VVVVVV to convert their own game data for personal use.

VVVVVV was created by Terry Cavanagh. Music is by Magnus Pålsson. Please purchase VVVVVV if you do not already own it.

# Setup
1. Download the current release.
2. Put the respected folder in the folders on your SD Card.
3. VVVVVV should be located in the "Computer" Section of the OpenFPGA Library
4. Boot the "vvvvvv.json" and the game will boot. 

![Picture of Pocket Running VVVVVV](https://github.com/SilverSpork/VVVVVV.OpenFPGAOS.Analogue_Pocket/blob/main/IMG_2239.JPG)
