# Starter Project DMX Control 3 WIP

# Disclaimer
This Project and Doku is Work In Progress. Thats why Currently is no Project Starter Project in this git, I will add when I have have smth.

## General
The Starter Project is use when Creating a new Project.
Purpose of this Project is to reduce redundant Configuration and Programming of repetitive function
To use this Prohject Just import it to DMX Control 3 and clone a new Version of it.
I create this Starter Projekct with my Current Knowlade and Experice. I try to keep this guid up to date
But nothing is set in Stone.



## Culists

### Unused Cuelists
Unused Cues are not used when the project is used Live.
Cues here are not Availabel in the Softdesk, Input Assignment or Executors.
There **unused** for Live usage. These Cues are just for saving and experimanting with cues.

### Live Cuelists
These are the CueLists **used** Softdesk, Input Assignment or Executors. Cues from here are made 
for **Live ussage in Production**. If you want to change a cuelist here **do not delete** it. Just open the cuelist
and made yoour changes. When you like to save a cue from Inside the culist for later usage copy it and paste it into 
an unused Cuelist.  If you like to use a cue you create it from before just copy it from an unused cue list into your Live Culist where 
you need it.

## Device Groups

### Color Selection Groups
The Project has **8 Color Selection Groups** (Reason: I use a [AKAI APC Mini Mide Controller WIP](https://github.com/FlorianGericke/DMXControl-files/tree/main/dmxControl/midi_rule_sets/apc_mini_mk_2)
this midi Controler has 8 softuttons in one row)
You can assign as Meny Fixture you like to on Color Selection Group.
Purpose of on Group is to select one Group and then Apply a color to each fixture of this Group. [more WIP](#Color-Selection-Groups-1)

## Executers

## Masters

## Parameters

## Input Assignment

### Color Selection Groups
 
## DMX Input 

### General

The Defalut Project Accept DMX Values from an external DMX Controler.
The Input is has its own Universe, so that In and Out going Values are not mixed.
The efault project shloud be confggured after loading.
	
### SetUp DMX Interface and Input Universe

	Interface	: Dmx Control Projects Nodle 4
	Interface Mode	: 6 - PC Out -> DMX Out & DMX In -> PC In
	DMX-In Enabled 	: True
	DMX-In Addres	: 2.1
	
## Project Structure

### Prioritys
Each Cue List has an Priority and with these you can set up wich cue can be played over another. How the Priorites are set has a big impakt to the way the Show is contolled Live. To have some sort of System how the Prioitys are used I strucktured mz Priorites in Groups. Each group has a range of between 0 and 9 (higer number means higer priority)

	[Group  0 => 000 - 009] First Group is always Empty !
	[Group  1 => 010 - 019] Basic Cues
	[Group  2 => 020 - 029] Block Parameters
	[Group  3 => 030 - 039] Fixture Programms (S2L,...)
	[Group  4 => 040 - 049] All Fixture Cues
	[Group  5 => 050 - 059] Blackout
	[Group  6 => 060 - 069] Device Setup
	[Group  7 => 070 - 079] Executer (Highlight)
	[Group  8 => 080 - 089] Executer (Transition)
	[Group  9 => 090 - 099] Flash Effects
	[Group 10 => 100 - 109] Stage Light


### Masters

#### ParameterMaster
#### SpeedMaster
