# Starter Project DMX Control 3 WIP

## Disclaimer

This project and documentation are a work in progress. That’s why there is currently no project starter in this repository. I will add it when I have something ready.

## General

The starter project is used when creating a new project. The purpose of this project is to reduce redundant configuration and programming of repetitive functions.

To use this project, just import it into DMX Control 3 and clone a new version of it. I created this starter project based on my current knowledge and experience. I try to keep this guide up to date, but nothing is set in stone.

## Cuelists

### Unused Cuelists

Unused cues are not used when the project is run live. Cues in this section are not available in the Softdesk, Input Assignment, or Executors. They are **unused** for live usage and are just for saving and experimenting with cues.

### Live Cuelists

These are the cuelists **used** in Softdesk, Input Assignment, or Executors. Cues from here are meant for **live usage in production**. If you want to change a cuelist here, **do not delete** it. Just open the cuelist and make your changes.

If you want to save a cue from inside the cuelist for later use, copy it and paste it into an unused cuelist. If you want to use a cue you created earlier, simply copy it from an unused cuelist into your live cuelist where you need it.

## Device Groups

### Color Selection Groups

The project has **8 Color Selection Groups** (Reason: I use an [AKAI APC Mini MIDI Controller WIP](https://github.com/FlorianGericke/DMXControl-files/tree/main/dmxControl/midi_rule_sets/apc_mini_mk_2). This MIDI controller has 8 soft buttons in one row).

You can assign as many fixtures as you like to one Color Selection Group. The purpose of a group is to select one group and then apply a color to each fixture within that group. [More WIP](#Color-Selection-Groups-1)

## Executors

## Masters

## Parameters

## Input Assignment

### Color Selection Groups

## DMX Input

### General

The default project accepts DMX values from an external DMX controller. The input has its own universe, so that incoming and outgoing values are not mixed. The default project should be configured after loading.

### Setup DMX Interface and Input Universe

```
Interface        : DMX Control Projects Nodle 4
Interface Mode   : 6 - PC Out -> DMX Out & DMX In -> PC In
DMX-In Enabled   : True
DMX-In Address   : 2.1
```

## Project Structure

### Priorities

Each cuelist has a priority, which determines which cue can be played over another. How priorities are set has a big impact on how the show is controlled live. To maintain a structured system, I organize my priorities into groups. Each group has a range between 0 and 9 (higher numbers indicate higher priority).

```
[Group  0 => 000 - 009] First group is always empty!
[Group  1 => 010 - 019] Basic Cues
[Group  2 => 020 - 029] Block Parameters
[Group  3 => 030 - 039] Fixture Programs (S2L, ...)
[Group  4 => 040 - 049] All Fixture Cues
[Group  5 => 050 - 059] Blackout
[Group  6 => 060 - 069] Device Setup
[Group  7 => 070 - 079] Executor (Highlight)
[Group  8 => 080 - 089] Executor (Transition)
[Group  9 => 090 - 099] Flash Effects
[Group 10 => 100 - 109] Stage Light
```

### Masters

#### Parameter Master

#### Speed Master

