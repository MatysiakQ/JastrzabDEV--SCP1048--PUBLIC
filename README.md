# SCP-1048 (Builder Bear)

<div align="center">

![C#](https://img.shields.io/badge/C%23-.NET%20Framework%204.8-512BD4?style=for-the-badge)
![EXILED](https://img.shields.io/badge/EXILED-Custom%20Plugin-green?style=for-the-badge)
![Unity](https://img.shields.io/badge/Unity-Game%20Engine-black?style=for-the-badge)
![Mirror](https://img.shields.io/badge/Mirror-Networking-orange?style=for-the-badge)
![ProjectMER](https://img.shields.io/badge/ProjectMER-Schematics-blue?style=for-the-badge)

**Commercial SCP: Secret Laboratory Custom Role Showcase**

</div>

---

# Overview

SCP-1048 (Builder Bear) is a commercial custom role plugin developed for SCP: Secret Laboratory using C# and the EXILED plugin framework.

The project introduces a fully playable SCP-1048 entity featuring custom animations, audio integration, gameplay abilities, synchronized schematic representation, and server-side gameplay logic.

This repository serves as a technical showcase of the project.

> Source code is private due to commercial and intellectual property reasons.

---

# Features

## Custom SCP-1048 Role

- Custom SCP role implementation
- Automatic round-start spawning system
- Custom health and combat configuration
- Custom spawn broadcast

## Ability System

### Dash Ability

- Configurable cooldown
- Configurable damage
- Collision detection
- Impact handling
- Temporary movement boost
- Temporary stun after impact

### Wave Emote

- Dedicated player-triggered emote
- Animation playback
- Audio playback

## Animation System

Supported animation states:

- Idle
- Walk
- Attack
- Dash
- Dash Impact
- Wave
- Death

## Audio System

- Spatial audio playback
- Random ambient sounds
- Attack sounds
- Dash sounds
- Death sounds
- Greeting sounds
- Configurable audio volume

## Administration Commands

RemoteAdmin commands:

```text
scp1048 give <player>
scp1048 remove <player>
```

## Player Controls

Custom keybind integration through Server Specific Settings:

- Dash
- Wave Emote

---

# Tech Stack

## Core

- C#
- .NET Framework 4.8

## SCP:SL Frameworks

- EXILED
- Exiled.CustomRoles
- Exiled.Events

## Game Engine

- Unity

## Multiplayer

- Mirror

## Object & Schematic Systems

- ProjectMER

## Audio

- AudioPlayerApi

## Utility Libraries

- MEC

---

# Architecture

The plugin is organized around four primary components:

## Plugin

Responsible for:

- plugin initialization
- event registration
- custom role registration
- keybind registration

## Custom Role

Responsible for:

- SCP-1048 role lifecycle
- player setup
- spawning logic
- cleanup logic

## Controller

Responsible for:

- animation control
- ability execution
- audio playback
- schematic synchronization
- cooldown management

## Event Handlers

Responsible for:

- round events
- damage handling
- death handling
- disconnect handling
- ragdoll management

---

---

# Project Gallery

## Gameplay Screenshots

### Screenshot 1

![Screenshot 1](images/misiek2.png)

### Screenshot 2

![Screenshot 2](images/misiek1png)

### Screenshot 3

![Screenshot 3](images/misiek3.png)

---

# Demonstration

## Video Showcase

[Watch Gameplay Demo](YOUR_YOUTUBE_LINK_HERE)

---

# Development Journey

This project was created as a commercial custom role solution for SCP: Secret Laboratory.

The main development goals included:

- creating a fully playable SCP-1048 role
- integrating a custom schematic-based character representation
- implementing synchronized animations
- creating unique gameplay abilities
- integrating custom audio systems
- supporting multiplayer gameplay environments

The project also involved the creation and integration of a dedicated SCP-1048 schematic/model used by the role.

---

# Installation

## Requirements

- SCP: Secret Laboratory Dedicated Server
- EXILED
- ProjectMER
- AudioPlayerApi

## Plugin Installation

Place:

```text
SCP1048Plugin.dll
```

inside:

```text
EXILED/Plugins
```

## Additional Assets

Required assets include:

```text
Audio/
SCP-1048 schematic files
```

---

# Configuration

Example configurable settings:

```yaml
SpawnChance
Health

PrimaryAttackDamage

DashDamage
DashCooldown
DashDuration
DashStunDuration

AudioVolume

EnableRandomSounds
RandomSoundIntervalMin
RandomSoundIntervalMax
```

---

# API Overview

## RemoteAdmin Commands

### Spawn SCP-1048

```text
scp1048 give <player>
```

### Remove SCP-1048

```text
scp1048 remove <player>
```

---

# Technical Highlights

## Custom Role Lifecycle

Custom role registration and removal using EXILED CustomRoles.

## Schematic-Based Character Representation

Uses ProjectMER schematics for custom SCP visual representation.

## Animation State Management

Server-side animation control through schematic animation controllers.

## Spatial Audio System

AudioPlayerApi integration with configurable volume and event-driven playback.

## Coroutine-Based Systems

Uses MEC coroutines for:

- delayed execution
- cooldown logic
- audio scheduling
- cleanup operations

## Event-Driven Gameplay

Extensive usage of:

- player events
- round events
- combat events
- death events

---

# Testing

Not publicly available.

Testing details are not included in this repository.

---

# CI/CD

Not present in repository.

---

# Security Features

Role assignment and ability execution are controlled through server-side plugin logic.

No additional security mechanisms are publicly documented.

---

# Future Improvements

Potential future improvements:

- additional abilities
- expanded emote system
- additional SCP-1048 variants
- visual effect enhancements
- configurable animation packs
- extended administration tooling

---

# What I Learned

This project provided practical experience with:

- C#
- Unity ecosystem integrations
- EXILED plugin development
- multiplayer gameplay systems
- event-driven architecture
- custom role development
- animation control systems
- audio integration
- coroutine-based programming
- configuration-driven systems
- game entity lifecycle management

---

# Source Code Availability

Source code is private due to commercial and intellectual property reasons.

This repository serves as a portfolio and technical showcase of the project.

---

# Authors

**Adam Jastrzębski**

Software Developer

[![GitHub](https://img.shields.io/badge/GitHub-MatysiakQ-181717?style=for-the-badge&logo=github)](https://github.com/MatysiakQ)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Adam_Jastrzębski-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/adamjastrzebski/)

[![Portfolio](https://img.shields.io/badge/Portfolio-adamjastrzebski.bio-4CAF50?style=for-the-badge&logo=googlechrome)](https://adamjastrzebski.bio/)

[![ko-fi](https://img.shields.io/badge/ko--fi-buy-ff5f5f?logo=ko-fi&style=for-the-badge)](https://ko-fi.com/jastrzabdev)

---

# Acknowledgements

- SCP: Secret Laboratory
- EXILED Framework
- ProjectMER
- Mirror Networking
- AudioPlayerApi
- Unity

---
