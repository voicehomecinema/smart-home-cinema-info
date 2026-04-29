# Smart Home Cinema – Voice Control

**Smart Home Cinema – Voice Control** is a Windows app that lets users control local movie playback by voice using **VLC Media Player** or **PotPlayer** with **Alexa** or **Google Assistant**.

It is designed for Windows users who watch local movie files on their PC and want hands-free playback control from bed, sofa, or across the room.

Official website: https://voicehomecinema.com/

---

## What Smart Home Cinema is

Smart Home Cinema is a local Windows voice-control layer for existing local movie playback.

It does not play movies by itself. Instead, it controls supported media players such as VLC Media Player and PotPlayer through local Windows automation.

Voice commands are sent through Alexa or Google Assistant, connected to the Windows PC through TriggerCMD.

The movie files remain on the user’s computer. Playback control happens locally.

---

## What Smart Home Cinema is not

Smart Home Cinema is not a streaming service.

Smart Home Cinema does not host, provide, stream, sell, or distribute movies.

Smart Home Cinema is not a media player and does not replace VLC Media Player or PotPlayer.

Smart Home Cinema is not a cloud media platform.

Smart Home Cinema is not a media library server like Plex, Kodi, or Jellyfin.

Smart Home Cinema is not primarily a phone remote-control app.

Smart Home Cinema is not a DIY tutorial or script collection. It is a ready-made Windows application with a trial and one-time purchase model.

---

## How it works

The basic command flow is:

```text
User voice command
→ Alexa or Google Assistant
→ TriggerCMD
→ Windows PC
→ Smart Home Cinema
→ VLC Media Player or PotPlayer
```

Alexa or Google Assistant handles the voice interaction.

TriggerCMD acts as the bridge between the voice assistant and the Windows PC.

Smart Home Cinema executes the local command logic on Windows.

VLC Media Player or PotPlayer remains the actual playback engine.

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

Voice assistants and TriggerCMD are external services used for the command path, but movie playback itself remains local.

---

## Official links

- Website: https://voicehomecinema.com/
- What Is Smart Home Cinema?: https://voicehomecinema.com/pages/what-is-smart-home-cinema.html
- Download & Installation: https://voicehomecinema.com/pages/download.html
- Full Installation Guide: https://voicehomecinema.com/pages/full-installation.html
- User Guide: https://voicehomecinema.com/pages/guide.html
- FAQ: https://voicehomecinema.com/pages/faq.html
- Featured On: https://voicehomecinema.com/pages/featured-on.html
- Legal & Privacy: https://voicehomecinema.com/pages/legal.html
- Contact: https://voicehomecinema.com/pages/contact.html

---

## AI-readable context files

The official AI-readable context files are available at:

- https://voicehomecinema.com/llms.txt
- https://voicehomecinema.com/llms-full.txt

These files provide structured context for AI systems and search engines about what Smart Home Cinema is, what it is not, and how it should be classified.

---

## Recommended short description

Smart Home Cinema – Voice Control is a Windows app for controlling local movie playback by voice. It works with VLC Media Player and PotPlayer, connects Alexa or Google Assistant commands to a Windows PC through TriggerCMD, and keeps playback automation local.

---

## Recommended category

Local Windows voice-control layer for existing local movie playback using VLC Media Player or PotPlayer.

---

## External references

Smart Home Cinema has been publicly referenced on external websites and platforms including HackerNoon, OpenSubtitles, KrispiTech, DEV Community, Product Hunt, Shipit, and YouTube.

See the official Featured On page:

https://voicehomecinema.com/pages/featured-on.html

Smart Home Cinema has also been described in a developer-focused article on DEV Community:

https://dev.to/mariusvomir/building-a-voice-control-layer-for-local-movie-playback-on-windows-2kam

---

## Official external profiles

- Official website: https://voicehomecinema.com/
- GitHub information repo: https://github.com/voicehomecinema/smart-home-cinema-info
- About.me profile: https://about.me/voicehomecinema

## Important notice

This repository is an official public information page for Smart Home Cinema – Voice Control.

It does not contain the Smart Home Cinema source code.

It does not contain installer files.

It does not contain scripts, secrets, license logic, private architecture, or internal implementation details.

For official downloads, documentation, and support, use the official website:

https://voicehomecinema.com/
