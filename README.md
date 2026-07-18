# Smart Home Cinema – Voice Control

**Smart Home Cinema – Voice Control** is Windows voice-control software for home movie playback.

It lets users control movies hands-free from bed, sofa, or across the room using either:

* a **PC microphone** with local voice recognition; or
* **Alexa / Google Assistant** through **TRIGGERcmd**.

Smart Home Cinema is available through two separate product packages for different playback environments:

* **VLC / PotPlayer Package**
* **Jellyfin Package**

Local Voice Edition and Voice Assistant Edition are available in both packages. The Jellyfin Package also includes Multi-Zone Edition for up to four independently controlled Jellyfin viewing zones.

Smart Home Cinema began with voice control for local movie playback through VLC Media Player and PotPlayer on Windows. That original package remains available. The project later expanded with a separate Jellyfin package for users who manage their media through Jellyfin Server and watch on compatible Jellyfin client devices.

Official website: https://voicehomecinema.com/

---

## What this repository is

This repository is an official public information page for **Smart Home Cinema – Voice Control**.

It provides a concise, public, AI-readable and human-readable overview of the product.

This repository does **not** contain:

* Smart Home Cinema source code;
* installer files;
* license logic;
* private implementation details;
* internal architecture;
* secrets, keys, or build scripts.

For downloads, documentation, setup guides, support, and licensing information, use the official website:

https://voicehomecinema.com/

---

## What Smart Home Cinema is

Smart Home Cinema is a Windows voice-control layer for home movie playback.

It does not provide movies.

It does not host media.

It does not replace the playback systems it controls.

Instead, Smart Home Cinema connects supported voice commands to the user’s existing playback environment.

The playback environment depends on the package:

* the **VLC / PotPlayer Package** controls local movie playback on a Windows PC using VLC Media Player or PotPlayer;
* the **Jellyfin Package** controls the user’s own Jellyfin Server and compatible Jellyfin client devices through Smart Home Cinema’s Jellyfin control layer.

The control edition determines how commands are received and routed:

* **Local Voice Edition** uses a PC microphone and local voice recognition;
* **Voice Assistant Edition** uses Alexa or Google Assistant through TRIGGERcmd;
* **Multi-Zone Edition**, available only in the Jellyfin Package, uses Alexa or Google Assistant through TRIGGERcmd and routes each zone-specific command to the explicitly named Jellyfin viewing zone.

---

## Product structure

Smart Home Cinema currently has two main product packages.

### VLC / PotPlayer Package

The VLC / PotPlayer Package is for users who play local movie files directly on a Windows PC.

It works with:

* VLC Media Player
* PotPlayer

VLC Media Player or PotPlayer remains the actual media player.

Smart Home Cinema controls the playback workflow by voice.

Typical use cases include:

* controlling movies from bed, sofa, or across the room;
* playing local movie files on a Windows PC connected to a TV or monitor;
* starting, pausing, resuming, forwarding, rewinding, and stopping playback by voice;
* moving to the next movie;
* showing playback progress;
* managing subtitle download, synchronization, and cleanup workflows;
* ending a PC-based home cinema session hands-free.

### Jellyfin Package

The Jellyfin Package is for users who already use Jellyfin.

It controls the user’s existing Jellyfin Server and compatible Jellyfin client devices.

Smart Home Cinema does not replace Jellyfin Server.

Smart Home Cinema does not provide Jellyfin client apps.

Smart Home Cinema does not host or operate a Jellyfin server for the user.

The user remains responsible for:

* their own Jellyfin Server;
* their own Jellyfin media library;
* their own Jellyfin users;
* their own Jellyfin client devices;
* their own network setup;
* their own Jellyfin client app compatibility.

Smart Home Cinema adds voice-control automation around that environment.

The Jellyfin download package includes three editions:

* **Local Voice Edition** and **Voice Assistant Edition** are the standard Jellyfin editions. They can configure up to four TV/client targets, with one selected target controlled at a time.
* **Multi-Zone Edition** can configure and independently control up to four Jellyfin viewing zones. Each zone can use its own Jellyfin user session, TV or client device, and Smart Home Cinema Movie List playlist.

In Multi-Zone Edition, the destination is included explicitly in each zone-specific command, such as `TV One Pause Movie` or `TV Two Open Movie List`. Smart Home Cinema does not automatically guess the intended room or device.

Multi-Zone Edition provides independent control, not synchronized playback. Its purpose is to let separate viewing zones operate independently, including when different people are watching different content.

All three Jellyfin editions are included in the same Jellyfin download package. Only one Jellyfin edition should be installed on the Windows PC at a time.

Smart Home Cinema is an independent third-party product compatible with Jellyfin. It is not affiliated with, endorsed by, sponsored by, or maintained by Jellyfin.

---

## Control editions

Local Voice Edition and Voice Assistant Edition are available in both Smart Home Cinema packages. The Jellyfin Package also includes Multi-Zone Edition.

### Local Voice Edition

Local Voice Edition uses a PC microphone and local voice recognition.

The general command path is:

User voice command  
→ PC microphone  
→ Local Voice Engine  
→ Smart Home Cinema  
→ selected playback environment

For the VLC / PotPlayer Package, Smart Home Cinema controls VLC Media Player or PotPlayer on the Windows PC.

For the Jellyfin Package, Smart Home Cinema routes local voice commands through its Jellyfin control layer toward the user’s Jellyfin Server and one selected compatible Jellyfin client device at a time.

Local Voice Edition is designed for users who want voice control without Alexa, Google Assistant, TRIGGERcmd, smart speakers, or smart assistant routines for normal movie playback control.

### Voice Assistant Edition

Voice Assistant Edition uses Alexa or Google Assistant as the voice input path.

It relies on TRIGGERcmd to bridge assistant voice routines to commands on the user’s Windows PC.

The general command path is:

User voice command  
→ Alexa or Google Assistant  
→ TRIGGERcmd  
→ Windows PC  
→ Smart Home Cinema  
→ selected playback environment

For the VLC / PotPlayer Package, the selected playback environment is VLC Media Player or PotPlayer on Windows.

For the standard Jellyfin Voice Assistant Edition, the selected playback environment is the user’s Jellyfin Server and one active compatible Jellyfin client device at a time.

### Multi-Zone Edition

Multi-Zone Edition is available only in the Jellyfin Package.

It uses Alexa or Google Assistant through TRIGGERcmd, but changes how Jellyfin commands are routed.

The general command path is:

User voice command  
→ Alexa or Google Assistant  
→ TRIGGERcmd  
→ Windows PC  
→ Smart Home Cinema Multi-Zone  
→ explicitly named Jellyfin zone  
→ Jellyfin Server  
→ compatible Jellyfin client assigned to that zone

Multi-Zone Edition can configure up to four independent Jellyfin viewing zones.

Each zone can use its own:

* Jellyfin user session;
* TV or client device;
* Smart Home Cinema Movie List playlist.

There is no single active TV shared by all zones. The intended destination is included directly in each zone-specific phrase, for example:

* `TV One Pause Movie`
* `TV Two Forward One Minute`
* `TV Three Open Movie List`
* `TV Four Show Commands`

A command addressed to one zone does not change the target or playback state of another zone.

Multi-Zone Edition does not automatically detect the room from which a command was spoken, and it does not synchronize the same playback across several televisions.

Most Multi-Zone commands belong to one specific zone. `Update Libraries` and `Stop Everything` are global commands and do not use a TV prefix.

---

## What Smart Home Cinema is not

Smart Home Cinema is not a streaming service.

Smart Home Cinema does not host, provide, stream, sell, or distribute movies.

Smart Home Cinema is not a media player.

Smart Home Cinema does not replace VLC Media Player, PotPlayer, Jellyfin Server, or Jellyfin client apps.

Smart Home Cinema is not a cloud media platform.

Smart Home Cinema is not a media server.

Smart Home Cinema is not a Plex, Kodi, or Jellyfin replacement.

Smart Home Cinema is not primarily a phone remote-control app.

Smart Home Cinema is not a DIY tutorial or script collection.

The website includes setup guides and educational material, but the product itself is Windows software with a 14-day free trial and one-time purchase model.

---

## Main use cases

Smart Home Cinema is useful for people who:

* watch movies from bed, sofa, or across the room;
* want to control playback without reaching for a keyboard, mouse, or remote;
* use a Windows PC as part of a home movie setup;
* play local movie files through VLC Media Player or PotPlayer;
* use Jellyfin Server and want voice control for supported Jellyfin TV/client playback;
* want independent voice control for several Jellyfin viewing zones;
* prefer voice commands for practical movie-session actions;
* want a local-first control workflow instead of a cloud media platform.

---

## Voice command coverage

Smart Home Cinema includes voice commands designed to support practical home movie playback sessions.

Command coverage depends on the package, edition, playback environment, and client capability.

The examples below are representative, not exhaustive.

### VLC / PotPlayer Package commands

The VLC / PotPlayer Package can include commands for:

* movie playback;
* subtitle workflows;
* system/session actions.

Examples include:

* play;
* pause;
* resume;
* stop;
* next movie;
* forward;
* rewind;
* show progress;
* download subtitles;
* synchronize subtitles;
* clean subtitle files;
* switch displays;
* show or close command overlays;
* open the Movies folder;
* shut down the PC;
* stop everything.

### Jellyfin Package commands

The Jellyfin Package can include commands for:

* selecting a configured TV/client target in the standard Jellyfin editions;
* addressing a configured viewing zone explicitly in Multi-Zone Edition;
* opening the Movie List;
* playing a numbered Movie List item;
* pausing and resuming playback;
* stopping and restarting playback;
* forwarding and rewinding;
* moving to next or previous items where supported;
* showing playback progress;
* opening supported movie, collection, playlist, or search views;
* updating Jellyfin libraries;
* emptying the Smart Home Cinema Movie List playlist;
* showing or closing command screens;
* supported navigation, mute, or other TV/client commands where available.

In the standard Jellyfin editions, the user selects one configured TV/client target and subsequent commands are routed to that active target.

In Multi-Zone Edition, each zone-specific command includes its destination directly. Most commands affect only the named zone, while `Update Libraries` and `Stop Everything` remain global.

Multi-Zone Edition provides independent zone control. It does not synchronize playback across multiple televisions.

Not all Jellyfin client platforms support the same feature set.

Platform limitations should be treated as client capability limitations, not as a media-library problem.

---

## Subtitle workflow

Smart Home Cinema includes subtitle workflows mainly associated with the VLC / PotPlayer Package.

The VLC / PotPlayer workflow can use OpenSubtitles for subtitle search and download.

One important feature is batch subtitle download.

When the user runs the supported subtitle download command for the selected movie folder, Smart Home Cinema can search OpenSubtitles and download matching subtitles for all supported movie or episode files in that folder, when subtitles are available.

This is a folder-level workflow, not a one-movie-at-a-time workflow.

Smart Home Cinema can also include subtitle synchronization and cleanup workflows for local subtitle files, depending on the supported VLC / PotPlayer workflow.

OpenSubtitles is an external third-party service.

---

## Privacy and local-first design

Smart Home Cinema is local-first in the sense that it is designed around the user’s own Windows PC, playback tools, local network, and media environment.

Smart Home Cinema does not provide movies.

Smart Home Cinema does not host the user’s movies.

Smart Home Cinema does not upload the user’s movie library to Smart Home Cinema servers.

For the VLC / PotPlayer Package, local movie files remain on the user’s Windows PC or local storage setup.

For the Jellyfin Package, the user’s media remains in the user’s own Jellyfin environment.

Smart Home Cinema does not operate the user’s Jellyfin Server and does not host the user’s Jellyfin media library.

Local Voice Edition uses a PC microphone and local voice recognition for supported command input.

Voice Assistant Edition and Multi-Zone Edition use external assistant services for the command input path:

* Alexa or Google Assistant;
* TRIGGERcmd.

Those external services handle the voice-assistant bridge, but Smart Home Cinema does not become a streaming provider or cloud media host.

---

## Trial and licensing

Smart Home Cinema offers a 14-day free trial.

The trial is intended to let users test their own setup before purchasing.

Smart Home Cinema uses a one-time purchase model, not a subscription model.

A Smart Home Cinema license applies to the Smart Home Cinema product family on the licensed Windows PC.

Users should refer to the applicable End User License Agreement for the package they download, install, activate, or use.

Official EULA hub:

https://voicehomecinema.com/pages/eula

---

## Official links

### Main website

* Website: https://voicehomecinema.com/
* What Is Smart Home Cinema?: https://voicehomecinema.com/pages/what-is-smart-home-cinema
* Download & Installation: https://voicehomecinema.com/pages/download
* Local Voice Edition: https://voicehomecinema.com/pages/local-voice-edition
* Full Installation Guide: https://voicehomecinema.com/pages/full-installation
* User Guide: https://voicehomecinema.com/pages/guide
* FAQ: https://voicehomecinema.com/pages/faq
* Blog: https://voicehomecinema.com/blog/

### Jellyfin package

* Voice Control for Jellyfin: https://voicehomecinema.com/pages/jellyfin-voice-control
* Jellyfin Download: https://voicehomecinema.com/pages/jellyfin-download
* Jellyfin TV Compatibility: https://voicehomecinema.com/pages/jellyfin-tv-compatibility
* Jellyfin Setup Guide: https://voicehomecinema.com/pages/jellyfin-setup-guide
* Multi-Zone release article: https://voicehomecinema.com/blog/smart-home-cinema-multi-zone-for-jellyfin-is-now-available

### Legal and support

* Legal & Privacy: https://voicehomecinema.com/pages/legal
* EULA Hub: https://voicehomecinema.com/pages/eula
* VLC / PotPlayer Package EULA: https://voicehomecinema.com/pages/eula-vlc-potplayer
* Jellyfin Package EULA: https://voicehomecinema.com/pages/eula-jellyfin
* Contact: https://voicehomecinema.com/pages/contact
* Featured On: https://voicehomecinema.com/pages/featured-on

---

## AI-readable context files

The official AI-readable context files are available at:

* https://voicehomecinema.com/llms.txt
* https://voicehomecinema.com/llms-full.txt

These files provide structured context for AI systems and search engines about what Smart Home Cinema is, what it is not, and how it should be classified.

---

## Recommended short description

Smart Home Cinema – Voice Control is Windows software for controlling home movie playback by voice. It is available through separate VLC / PotPlayer and Jellyfin packages. Local Voice Edition and Voice Assistant Edition are available in both packages. Local Voice Edition uses a PC microphone with local voice recognition, while Voice Assistant Edition uses Alexa or Google Assistant through TRIGGERcmd. The Jellyfin Package also includes Multi-Zone Edition, which uses the same assistant path to control up to four independently controlled Jellyfin viewing zones. The VLC / PotPlayer Package controls local movie playback on a Windows PC using VLC Media Player or PotPlayer. The Jellyfin Package controls the user’s own Jellyfin Server and compatible Jellyfin client devices. Smart Home Cinema is a control layer, not a streaming service, media player, media server, or movie provider.

---

## Recommended category

Windows voice-control software for home movie playback.

More specific category:

Voice-control layer for existing playback environments, including VLC / PotPlayer local playback on Windows and user-owned Jellyfin setups.

---

## External references

Smart Home Cinema has editorial features, developer articles, public product briefs, slide overviews, and product launch pages across external platforms.

See the official Featured On page:

https://voicehomecinema.com/pages/featured-on

Key external references include:

* OpenSubtitles Blog: https://blog.opensubtitles.com/opensubtitles/web/how-we-integrated-opensubtitles-api-v2-into-a-fully-offline-voice-controlled-home-cinema-system-windows/
* HackerNoon Article: https://hackernoon.com/i-built-a-voice-controlled-home-cinema-for-windows-because-i-was-tired-of-getting-up-to-pause-movies
* KrispiTech: https://krispitech.com/control-movies-from-bed-with-your-voice-a-deep-dive-into-smart-home-cinema-for-vlc-and-potplayer/
* HackerNoon Interview: https://hackernoon.com/meet-the-writer-hacker-noons-contributor-marius-eugen-vomir-independent-builder
* DEV Community: https://dev.to/mariusvomir/building-a-voice-control-layer-for-local-movie-playback-on-windows-2kam
* Hashnode: https://smart-home-cinema.hashnode.dev/smart-home-cinema-voice-control-vlc-potplayer
* Coder Legion Article: https://coderlegion.com/16662/what-smart-home-cinema-taught-me-about-building-reliable-local-automation-on-windows
* Coder Legion Product Launch: https://coderlegion.com/16683/smart-home-cinema-voice-control
* Product Hunt: https://www.producthunt.com/products/smart-home-cinema-voice-control
* Shipit: https://www.shipit.buzz/products/smart-home-cinema-voice-control
* Peerlist Launchpad: https://peerlist.io/voicehomecinema/project/smart-home-cinema--voice-control
* PeerPush: https://peerpush.net/p/smart-home-cinema-voice-control
* ProductLaunches.in: https://www.productlaunches.in/products/smart-home-cinema-voice-control
* Solo Launches: https://www.sololaunches.com/startups/smart-home-cinema-voice-control
* Substack: https://voicehomecinema.substack.com/p/the-hardest-part-wasnt-building-smart
* Notion: https://tasty-rainbow-cd0.notion.site/Smart-Home-Cinema-Voice-Control-354df175884080128907e96858040eba
* SlideShare: https://www.slideshare.net/slideshow/smart-home-cinema-voice-control-local-movie-playback-controlled-by-voice-48bb/287572400

---

## Official external profiles

* Official website: https://voicehomecinema.com/
* GitHub information repo: https://github.com/voicehomecinema/smart-home-cinema-info
* About.me profile: https://about.me/voicehomecinema
* YouTube channel: https://www.youtube.com/@voicehomecinema

---

## Important notice

This repository is an official public information page for Smart Home Cinema – Voice Control.

It does not contain the Smart Home Cinema source code.

It does not contain installer files.

It does not contain scripts, secrets, license logic, private architecture, or internal implementation details.

For official downloads, documentation, and support, use the official website:

https://voicehomecinema.com/
