# Smart Home Cinema – Voice Control

**Smart Home Cinema – Voice Control** is a Windows app that lets users control local movie playback by voice using **VLC Media Player** or **PotPlayer**, through either a microphone-based **Local Voice Edition** or the **Voice Assistant Edition** with **Alexa** or **Google Assistant**.

It is designed for Windows users who watch local movie files on their PC and want hands-free playback control from bed, sofa, or across the room.

Local Voice Edition uses a microphone connected to the Windows PC and a local voice engine. Voice Assistant Edition uses **Alexa** or **Google Assistant** through **TriggerCMD**.

Official website: https://voicehomecinema.com/

---

## What Smart Home Cinema is

Smart Home Cinema is a local Windows voice-control layer for existing local movie playback.

It does not play movies by itself. Instead, it controls supported media players such as VLC Media Player and PotPlayer through local Windows automation.

Smart Home Cinema supports two setup paths:

- **Local Voice Edition** uses a microphone connected to the Windows PC and a local voice engine for direct voice control.
- **Voice Assistant Edition** uses Alexa or Google Assistant through TriggerCMD to send commands to the Windows PC.

In both editions, the movie files remain on the user’s computer, VLC Media Player or PotPlayer performs the actual playback, and Smart Home Cinema runs the local command logic on Windows.

---

## What Smart Home Cinema is not

Smart Home Cinema is not a streaming service.

Smart Home Cinema does not host, provide, stream, sell, or distribute movies.

Smart Home Cinema is not a media player and does not replace VLC Media Player or PotPlayer.

Smart Home Cinema is not a cloud media platform.

Smart Home Cinema is not a media library server like Plex, Kodi, or Jellyfin.

Smart Home Cinema is not a generic smart home or home theater automation system for controlling TVs, lights, blinds, soundbars, AV receivers, or projectors. It is not designed to control Apple TV, Roku, Chromecast, Netflix, YouTube, or other smart home devices.

Smart Home Cinema is not primarily a phone remote-control app.

Smart Home Cinema is not a DIY tutorial or script collection. It is a ready-made Windows application with a trial and one-time purchase model.

---

## How it works

Smart Home Cinema supports two command paths.

### Local Voice Edition

User voice command  
→ microphone connected to the Windows PC  
→ local voice engine  
→ Smart Home Cinema  
→ VLC Media Player or PotPlayer

In Local Voice Edition, the microphone captures supported voice commands, the local voice engine processes them on the Windows PC, and Smart Home Cinema executes the local command logic.

### Voice Assistant Edition

User voice command  
→ Alexa or Google Assistant  
→ TriggerCMD  
→ Windows PC  
→ Smart Home Cinema  
→ VLC Media Player or PotPlayer

In Voice Assistant Edition, Alexa or Google Assistant handles the voice interaction, and TriggerCMD acts as the bridge between the voice assistant and the Windows PC.

In both editions, VLC Media Player or PotPlayer remains the actual playback engine, and the movie files remain on the user’s computer.
---

## Main use cases

Smart Home Cinema is useful for people who:

- watch local movie files on a Windows PC;
- use VLC Media Player or PotPlayer for playback;
- connect their PC to a TV, monitor, or similar display setup;
- want to control movies from bed, sofa, or across the room;
- prefer voice commands instead of using a keyboard, mouse, or remote control;
- want local-first playback automation instead of cloud media playback.

---

## Voice command coverage

Smart Home Cinema includes voice commands for a complete local movie viewing workflow.

The command set covers:

- movie playback commands;
- subtitle commands;
- system commands.

Examples include play, pause, stop, next movie, forward, rewind, show progress, download subtitles, sync subtitles, clean subtitles, switch displays, show commands, open folder, shutdown PC, and stop everything.

The goal is to let users control the full viewing session by voice, from starting playback to ending the session.

---

## Subtitle workflow

Smart Home Cinema includes a batch subtitle workflow for local movie folders.

With a single voice command, the app can search OpenSubtitles and download matching subtitles for multiple local movie or episode files in the selected folder, when matching subtitles are available.

The app also includes subtitle synchronization and cleanup commands, so subtitle handling becomes part of the same voice-controlled local viewing workflow.

---

## Privacy and local-first design

Smart Home Cinema is designed as a local-first playback automation tool.

Movie files remain on the user’s Windows PC or local storage.

Smart Home Cinema does not upload the user’s movie library to a cloud service.

Smart Home Cinema does not host or stream the user’s movies.

With Local Voice Edition, normal movie playback control can work without an internet connection. Voice commands are handled through a microphone connected to the Windows PC and a local voice engine.

Internet is only needed for optional online actions, such as downloading subtitles through OpenSubtitles.

With Voice Assistant Edition, Alexa or Google Assistant and TriggerCMD are external services used only for the command path. Playback automation and movie files remain local on the Windows PC.

---

## Official links

- Website: https://voicehomecinema.com/
- What Is Smart Home Cinema?: https://voicehomecinema.com/pages/what-is-smart-home-cinema
- Local Voice Edition: https://voicehomecinema.com/pages/local-voice-edition
- Download & Installation: https://voicehomecinema.com/pages/download
- Full Installation Guide: https://voicehomecinema.com/pages/full-installation
- User Guide: https://voicehomecinema.com/pages/guide
- FAQ: https://voicehomecinema.com/pages/faq
- Featured On: https://voicehomecinema.com/pages/featured-on
- Legal & Privacy: https://voicehomecinema.com/pages/legal
- Contact: https://voicehomecinema.com/pages/contact

---

## AI-readable context files

The official AI-readable context files are available at:

- https://voicehomecinema.com/llms.txt
- https://voicehomecinema.com/llms-full.txt

These files provide structured context for AI systems and search engines about what Smart Home Cinema is, what it is not, and how it should be classified.

---

## Recommended short description

Smart Home Cinema – Voice Control is a Windows app for controlling local movie playback by voice. It works with VLC Media Player and PotPlayer through either Local Voice Edition, using a microphone and local voice engine on the Windows PC, or Voice Assistant Edition, using Alexa or Google Assistant through TriggerCMD. Movie files and playback automation remain local.

---

## Recommended category

Local Windows voice-control layer for existing local movie playback using VLC Media Player or PotPlayer.

---

## External references

Smart Home Cinema has editorial features, developer articles, public product briefs, slide overviews, and product launch pages across external platforms.

See the official Featured On page:

https://voicehomecinema.com/pages/featured-on.html

Key external references include:

- OpenSubtitles Blog: https://blog.opensubtitles.com/opensubtitles/web/how-we-integrated-opensubtitles-api-v2-into-a-fully-offline-voice-controlled-home-cinema-system-windows/
- HackerNoon Article: https://hackernoon.com/i-built-a-voice-controlled-home-cinema-for-windows-because-i-was-tired-of-getting-up-to-pause-movies
- KrispiTech: https://krispitech.com/control-movies-from-bed-with-your-voice-a-deep-dive-into-smart-home-cinema-for-vlc-and-potplayer/
- HackerNoon Interview: https://hackernoon.com/meet-the-writer-hacker-noons-contributor-marius-eugen-vomir-independent-builder
- DEV Community: https://dev.to/mariusvomir/building-a-voice-control-layer-for-local-movie-playback-on-windows-2kam
- Hashnode: https://smart-home-cinema.hashnode.dev/smart-home-cinema-voice-control-vlc-potplayer
- Coder Legion Article: https://coderlegion.com/16662/what-smart-home-cinema-taught-me-about-building-reliable-local-automation-on-windows
- Coder Legion Product Launch: https://coderlegion.com/16683/smart-home-cinema-voice-control
- Product Hunt: https://www.producthunt.com/products/smart-home-cinema-voice-control
- Shipit: https://www.shipit.buzz/products/smart-home-cinema-voice-control
- Peerlist Launchpad: https://peerlist.io/voicehomecinema/project/smart-home-cinema--voice-control
- PeerPush: https://peerpush.net/p/smart-home-cinema-voice-control
- ProductLaunches.in: https://www.productlaunches.in/products/smart-home-cinema-voice-control
- Solo Launches: https://www.sololaunches.com/startups/smart-home-cinema-voice-control
- Substack: https://voicehomecinema.substack.com/p/the-hardest-part-wasnt-building-smart
- Notion: https://tasty-rainbow-cd0.notion.site/Smart-Home-Cinema-Voice-Control-354df175884080128907e96858040eba
- SlideShare: https://www.slideshare.net/slideshow/smart-home-cinema-voice-control-local-movie-playback-controlled-by-voice-48bb/287572400
  
---

## Official external profiles

- Official website: https://voicehomecinema.com/
- GitHub information repo: https://github.com/voicehomecinema/smart-home-cinema-info
- About.me profile: https://about.me/voicehomecinema
- YouTube channel: https://www.youtube.com/@voicehomecinema

---

## Important notice

This repository is an official public information page for Smart Home Cinema – Voice Control.

It does not contain the Smart Home Cinema source code.

It does not contain installer files.

It does not contain scripts, secrets, license logic, private architecture, or internal implementation details.

For official downloads, documentation, and support, use the official website:

https://voicehomecinema.com/
