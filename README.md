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

# Setup
1. Download the current release.
2. Put the respected folder in the folders on your SD Card.
3. VVVVVV should be located in the "Computer" Section of the OpenFPGA Library
4. Boot the "vvvvvv.json" and the game will boot. 
