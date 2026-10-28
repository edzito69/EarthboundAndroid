# EarthboundAndroid
EarthboundAndroid brings EarthBound to Android with touch controls, portrait menus, quicksaves, zoom and experimental co-op. Built on Brian Pugh's code and Herringway/ebsrc's community work. Edzito's edition made with *AI assistance*, love and gratitude to the original creators, developers, translators and players. Requires your own ROM.

An unofficial, experimental EarthBound adaptation for Android, with touch controls, a portrait options menu, save states, modern gameplay settings and experimental local co-op.

Built on Brian Pugh and contributors’ EarthBound C implementation, incorporating the earlier disassembly and research from Herringway/ebsrc. This edition adds modifications to that foundation, with gratitude and respect for its original authors.
Experimental status
The entire Android port—including local co-op—is experimental.

The APK has passed signature, ARM64 library and package-alignment checks. Touch controls and the portrait menu have been tested through SDL simulations on Windows. The latest build has not been fully validated on a physical Android device.

Rendering, audio, Bluetooth controllers, performance and story progression may behave differently between devices. Keep backups of important saves.
Requirements and installation
- Android 8.0 or newer.
- A 64-bit ARM device.
- Your own original, unmodified EarthBound (USA) ROM in .sfc or .smc format.
1. Download and install the APK.
2. Open EarthboundAndroid3.6.4.
3. Use the ROM picker to select your compatible ROM.
4. Start playing and adjust your preferences through the options menu.
No ROM is supplied or downloaded. The app imports the selected ROM into its private storage. Uninstalling the app removes its private ROM, preferences and saves.
Features
- Automatic portrait and landscape orientation.
- Portrait framing with Ness positioned slightly above the screen center.
- A vertical options menu with scrolling and direct touch selection.
- Invisible analog-stick movement and optional running.
- Pinch zoom, with a default zoom setting of 140%.
- English and Brazilian Portuguese language options.
- Manual save states, four quicksaves per drawer and three rotating autosaves.
- Save thumbnails, recording date/time and elapsed-time information.
- Optional fast-forward and rewind controls.
- Configurable button visibility, size and opacity.
- Controller remapping and illustrated control maps.
- Optional Double XP and other gameplay settings.
- A God Menu with cheats and an optional hitkill shortcut.
- Experimental local co-op with a second compatible controller.
Touch controls
Gesture	Action
Touch and drag from the initial contact point	Move using an invisible analog stick
Drag farther from the starting point	Run, when enabled
Tap the center while exploring	Check or talk
Tap a native menu option	Select or interact with that option
Tap the center during menus/dialogue	Confirm
Tap farther from the center during menus	Back
Swipe in a direction	Navigate choices or battle targets
Hold during dialogue	Speed up text
Double tap or use two fingers	Open the personal menu while exploring; return in menus
Pinch	Adjust zoom


Direct taps on native menu options—including the naming keyboard—take priority over the general center/edge gestures.
Phone shortcuts
Only the two phone icons are visible by default.
Shortcut	Action
Tap the black phone	Choose a quicksave slot to save
Tap the red phone	Choose a quicksave slot to load
Hold either phone for approximately 0.6 seconds	Open the options menu


Loading requires selecting a quicksave; tapping the red phone does not immediately overwrite your current session with a saved state.

In landscape orientation, the red phone moves below the Mr. Saturn position.
Optional on-screen buttons
Enable these through the Touch settings:
- OK / Back: hidden by default.
- Fast-forward >> / Rewind <<: optional hold controls, stacked in the upper-right corner.
- Mr. Saturn: an optional direct shortcut to the options menu.
- Hitkill: enabled separately through the God Menu; appears in the lower-right corner.
Visibility and opacity changes apply immediately. The accelerometer is disabled as a gameplay controller; rotating the phone still changes screen orientation automatically.
Options menu
Hold a phone shortcut, or tap Mr. Saturn when enabled, to open the menu.

In portrait orientation, the menu uses a scrollable column with larger selectable cards and a fixed Back button near the upper-right edge.

Available sections include:
- Video/audio: presentation settings, filters, volume, zoom and languages.
- Controls: Touch instructions, controller settings and controller maps.
- Saves: manual states, quicksaves and autosaves.
- Chapters: campaign checkpoints and equipment kits.
- Gameplay: experimental co-op, Double XP, running and other optional features.
- Touch: button visibility, size, opacity, running distance and pinch zoom.
Tap CREDITS to view community acknowledgements.
Saves and quicksaves
Save states are organized into drawers A, B and C.

Each drawer provides:
- Eight manual slots.
- Four quicksave slots, corresponding to slots 9–12.
- Three rotating autosave slots, separate from manual saves and quicksaves.
Save cards include thumbnails and recording information. Autosaves wait for suitable moments after supported transitions and victories. Repeated nearby transitions are throttled to reduce duplicate checkpoints.

Autosaves are experimental and should supplement manual saves.
Experimental local co-op
Enable Experimental co-op under Gameplay, then press Start / Options / Menu on the controller intended for Player 2 and accept the join prompt.

The mode supports a second player as Mess, with independent character attributes and inventory. Depending on settings and the situation, players can explore separately and participate in shared battles.
PlayStation-style controller layout
Equivalent button positions apply to Xbox, Switch and generic controllers.
Input	Action
D-pad / Left stick	Move and navigate
Hold Cross / X while moving	Run
Cross / X	Confirm menus and dialogue
Square	Talk, check and interact
Circle	Personal menu / Back
Triangle	Party HP, PP and money
Cross / X + R1	Photo pose
L3	Request teleport to the other player
P2 R3	Change Mess’s clothing colors
P2 Select / Share	Leave the cooperative session


Controller assignments can be customized. The options menus retain their standard confirm/back positions.

Bluetooth multiplayer and the complete cooperative campaign still require broader physical-device testing. Independent exploration, doors, encounters and scripted events may have remaining issues.
Performance
This build reduces the internal rendering canvas and reuses decompressed scenario data to reduce repeated work in co-op. Output remains scaled to the phone display.

These changes reduce processing work, but a specific FPS improvement is not guaranteed. Actual performance depends on the device, settings and scene.
Cheats
The optional God Menu includes gameplay-altering tools and a toggle for the red hitkill button.

Cheats can disrupt story progression or create invalid situations. Keep a separate save before experimenting.
Community credits
This edition exists because of years of work by other people.

Special recognition goes to:
- Brian Pugh and contributors — the native C implementation and tools in BrianPugh/earthbound.
- Cameron Ross, Herringway and the ebsrc contributors — inherited disassembly, research and documentation through Herringway/ebsrc.
- CJ, Sean Staggs, PhoenixBound, Cooper Harasyn, Anonymous941 and lilliththecreative — additional author names recorded in the upstream revision’s history. Some names may be aliases of the same person.
- angelo_wf and LakeSnes contributors — SPC700/DSP audio.
- Sam Lantinga and SDL2 contributors — windowing, graphics, audio and input.
- Brian Pugh and tamp contributors — compression.
- Dale Weiler and incbin contributors — data embedding tools.
- Alex Foffano, Jared Morgan and the entire EarthBound Brasil translation team.
- FantasyAnime and its save authors, TheRunaway5, and the developers of the build tools used by this edition.
- Every researcher, programmer, translator, documenter, preservationist, tester and player whose contributions helped keep EarthBound accessible.
Thank you to Nintendo, Shigesato Itoi, APE, HAL Laboratory and the original development teams for creating EarthBound.

See [CREDITS.md](CREDITS.md) and the included licenses for expanded attribution and original notices.
AI assistance
OpenAI Codex was used extensively to assist with implementation, debugging, tests, builds and documentation.

Edzito directed this edition’s features and integration. The original game, upstream code, libraries and translations retain their original authorship. AI assistance does not replace testing or the contributions of the community.
This project is made for the community, with affection for EarthBound and respect for everyone whose work made it possible. Thank you for sharing your knowledge, code, tools, translations, feedback and love for this game.

— Edzito


  
22:27







em ingless







22:28






EarthboundAndroid3.6.4
An unofficial, experimental Android adaptation of EarthBound featuring touch controls, portrait and landscape support, save states, customizable settings, and experimental local co-op.

Built on Brian Pugh and contributors’ EarthBound C implementation, incorporating the earlier disassembly and research from Herringway/ebsrc.

This edition adds modifications to those foundations with gratitude and respect for their original authors.
Experimental status
The entire Android port, including local co-op, is experimental.

APK signature, ARM64 libraries, and package alignment have been checked. Touch controls and portrait-menu behavior have been tested through SDL simulations on Windows.

The latest version has not been fully validated on a physical Android device. Performance, Bluetooth controllers, rendering, audio, and story progression may vary between devices.

Keep backup copies of important saves.
Requirements
- Android 8.0 or newer.
- A 64-bit ARM device.
- Your own original, unmodified EarthBound (USA) ROM in .sfc or .smc format.
Installation
1. Download and install the APK.
2. Open EarthboundAndroid3.6.4.
3. Select your compatible ROM through the app’s file picker.
4. Start playing and customize your preferences.
No ROM is supplied or downloaded. The selected ROM is imported into the app’s private storage.

Uninstalling the app removes its private ROM, settings, and saves.
Features
- Automatic portrait and landscape orientation.
- Portrait framing with Ness positioned slightly above the screen center.
- A vertical options menu with scrolling and direct touch selection.
- Invisible analog-stick movement and optional running.
- Pinch zoom, with a default setting of 140%.
- English and Brazilian Portuguese language options.
- Manual save states, quicksaves, and rotating autosaves.
- Save thumbnails, recording dates, timestamps, and elapsed-time information.
- Optional fast-forward and rewind buttons.
- Configurable button visibility, size, and opacity.
- Controller customization and control maps.
- Optional Double XP and other gameplay settings.
- An optional God Menu with cheats and a hitkill shortcut.
- Experimental local co-op using compatible controllers.
Touch controls
Gesture	Action
Touch and drag from the initial contact point	Move using an invisible analog stick
Drag farther from the starting point	Run, when enabled
Tap the center while exploring	Check or talk
Tap a native menu option	Select that option
Tap the center during menus or dialogue	Confirm
Tap farther from the center during menus	Back
Swipe in a direction	Navigate menu choices or battle targets
Hold during dialogue	Speed up text
Double tap while exploring	Open the personal menu
Use two fingers	Open the personal menu while exploring or go back in menus
Pinch	Adjust zoom


Direct taps on native menu options—including the naming keyboard—take priority over the general center/edge gestures.
Phone shortcuts
Only the two phone icons are visible by default.
Shortcut	Action
Tap the black phone	Choose a quicksave slot to save
Tap the red phone	Choose a quicksave slot to load
Hold either phone for approximately 0.6 seconds	Open the options menu


The red phone opens a selection window rather than immediately loading a state.

In landscape orientation, it moves below the Mr. Saturn position.
Optional buttons
Configure these under Touch:
- OK and Back: hidden by default.
- Fast-forward >> and Rewind <<: optional hold buttons, stacked in the upper-right corner.
- Mr. Saturn: an optional direct shortcut to the options menu.
- Hitkill: enabled separately through the God Menu; appears in the lower-right corner.
Visibility and opacity changes apply immediately.

The accelerometer is disabled as a gameplay controller. Rotating the phone still changes screen orientation automatically.
Options menu
Hold either phone shortcut, or tap Mr. Saturn when enabled.

The portrait menu uses a scrollable column of selectable cards and a fixed Back button near the upper-right edge.

Available sections include:
- Video/audio: filters, volume, zoom, languages, and presentation settings.
- Controls: Touch instructions, controller settings, and controller maps.
- Saves: manual states, quicksaves, and autosaves.
- Chapters: campaign checkpoints and equipment kits.
- Gameplay: co-op, Double XP, running, and other optional features.
- Touch: button visibility, size, opacity, running distance, and pinch zoom.
Tap CREDITS to view community acknowledgements.
Saves
Save states are organized into drawers A, B, and C.

Each drawer contains:
- Eight manual save slots.
- Four quicksave slots.
- Three rotating autosave slots.
Autosaves are separate from manual saves and quicksaves. They wait for suitable moments after supported transitions and victories. Repeated nearby transitions are throttled to reduce duplicate checkpoints.

Autosaves remain experimental and should supplement manual saves.
Experimental local co-op
Enable Experimental co-op under Gameplay.

Press Start / Options / Menu on the controller intended for Player 2, then accept the join prompt.

Player 2 joins as Mess, with independent character attributes and inventory. Depending on the settings and situation, players can explore separately and participate in shared battles.
PlayStation-style controls
Equivalent button positions apply to Xbox, Switch, and generic controllers.
Input	Action
D-pad / Left stick	Move and navigate
Hold Cross / X while moving	Run
Cross / X	Confirm menus and dialogue
Square	Talk, check, and interact
Circle	Personal menu / Back
Triangle	Display party HP, PP, and money
Cross / X + R1	Photo pose
L3	Request teleport to the other player
P2 R3	Change Mess’s clothing colors
P2 Select / Share	Leave the cooperative session


Bindings can be customized. Options menus retain their standard confirm/back positions.

Bluetooth multiplayer and the complete cooperative campaign require broader physical-device testing. Doors, independent exploration, encounters, and scripted events may have remaining issues.
Performance
This build uses a smaller internal rendering canvas and reuses decompressed scenario data to reduce repeated processing in co-op. Output remains scaled to the phone display.

A specific FPS improvement is not guaranteed. Actual performance depends on the device, settings, and scene.
Cheats
The optional God Menu includes gameplay-altering tools and a toggle for the red hitkill button.

Cheats can disrupt story progression. Keep a separate save before experimenting.
Credits and acknowledgements
This edition exists because of years of community work.

Special recognition goes to:
- Brian Pugh and contributors — the native C implementation and supporting tools in BrianPugh/earthbound.
- Cameron Ross, Herringway, and the ebsrc contributors — inherited disassembly, documentation, and research through Herringway/ebsrc.
- CJ, Sean Staggs, PhoenixBound, Cooper Harasyn, Anonymous941, and lilliththecreative — additional author names recorded in the upstream revision’s history. Some names may be aliases of the same person.
- angelo_wf and LakeSnes contributors — SPC700/DSP audio.
- Sam Lantinga and SDL2 contributors — graphics, audio, windowing, and input.
- Brian Pugh and tamp contributors — compression.
- Dale Weiler and incbin contributors — data embedding tools.
- Alex Foffano, Jared Morgan, and the entire EarthBound Brasil translation team.
- FantasyAnime and its save authors, TheRunaway5, and the developers of the build tools used here.
- Every community programmer, researcher, translator, documenter, preservationist, tester, and player whose work helped keep EarthBound accessible.
Thank you to Nintendo, Shigesato Itoi, APE, HAL Laboratory, and the original development teams for creating EarthBound.

See [CREDITS.md](CREDITS.md) and the included licenses for expanded attribution and original notices.
AI assistance
OpenAI Codex was used extensively to assist with implementation, debugging, tests, builds, and documentation.

Edzito directed this edition’s features and integration. The original game, upstream code, libraries, and translations retain their original authorship.

AI assistance does not replace testing or the community’s contributions.
This project is made for the community, with affection for EarthBound and respect for everyone whose work made it possible. Thank you for sharing your knowledge, code, tools, translations, feedback, and love for this game.

— Edzito
