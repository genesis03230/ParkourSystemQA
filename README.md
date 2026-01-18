# Advanced Parkour System – QA Manual Testing

## Project Overview
Advanced Parkour System is a third-person parkour and climbing demo developed in Unity, inspired by Mirror’s Edge.

- Engine: Unity 2023.2.20f1
- Platform: PC
- Game Type: Third-Person Parkour / Movement System
- Status: Playable Demo

This project was developed during the **Advanced Character Controller Bootcamp (MasterDevs, 2025)** and was recognized as the **best project of the bootcamp** for its originality and technical execution.

## Core Objective
The player must be able to freely traverse an urban rooftop environment using advanced parkour mechanics such as vaulting, climbing, wall-running, and jumping, without breaking gameplay flow or falling into unrecoverable states.

## QA Scope
The QA activities for this project focus on:
- Player movement stability and responsiveness
- Level boundaries and out-of-bounds prevention
- Physics interactions during jumps and falls
- Recovery systems after failed parkour actions
- Prevention of soft locks and unintended exploration states

## Known Risk Areas
- High-speed player movement combined with physics
- Jumping from elevated rooftops
- Level boundaries and collision limits
- Missing respawn or recovery logic after falling outside the intended area

## Visual QA Preview

The following preview demonstrates a critical issue identified during manual testing.  
In this scenario, the player can jump from a rooftop and fall outside the intended playable area, remaining alive without a respawn or recovery mechanism, resulting in an unintended game state.

![Player falling outside playable area](Evidence/bug_player_falls_outside_map.gif)

> Full reproduction steps, severity, and complete video evidence are documented in `Bug-Reports.md`.

## Test Artifacts
- 📄 [Manual Test Cases](Test-Cases.md)
- 🐞 [Bug Reports with Evidence](Bug-Reports.md)

