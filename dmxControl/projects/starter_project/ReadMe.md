# Starter Project DMX Control 3 WIP

## Disclaimer
This project and documentation are a work in progress. That’s why there is currently no project starter in this repository. I will add it when I have something ready.

I build this Starte Projet for my AKAI APC mini midi Controler. When Using another 
changes in the Input Assignment will be nessary

## General
The starter project is used when creating a new project. The purpose of this project is to reduce redundant configuration and programming of repetitive functions.

To use this project, just import it into DMX Control 3 and clone a new version of it. I created this starter project based on my current knowledge and experience. I try to keep this guide up to date, but nothing is set in stone.

## Cuelists

### Unused Cuelists
Unused cues are not used when the project is run live. Cues in this section are not available in the Softdesk, Input Assignment, or Executors. They are **unused** for live usage and are just for saving and experimenting with cues.

### Live Cuelists
These are the cuelists **used** in Softdesk, Input Assignment, or Executors. Cues from here are meant for **live usage in production**. If you want to change a cuelist here, **do not delete** it. Just open the cuelist and make your changes.

If you want to save a cue from inside the cuelist for later use, copy it and paste it into an unused cuelist. If you want to use a cue you created earlier, simply copy it from an unused cuelist into your live cuelist where you need it.

### Executor Cues

#### Transitions
Here you can define 8 different transition cues.  
Transition cues have a higher priority than Highlights.  
[Look at Transition Executors](#Transition-Executers)

#### Highlights
Here you can define 8 different highlight cues.  
Highlight cues have a lower priority than Transitions.  
[Look at Highlight Executors](#Highlight-Executors)

### Basic Cues

#### General
These cues are more specific to the fixtures used in this project.  
Important parameter: [Faders](#Parameters) for these cues.  

| Fader | Fader Description |
| ----- | ----------------- |
|       |                   |

#### Movement
Use Frequency based on SpeedMaster 01 ({SpeedMaster 1: /15})
#### Positions
#### Light Chaser

### Device Setup Executer Cues

#### General
These cues are more specific to the fixtures used in this project.  
Important parameter: [Faders](#Parameters) for these cues.  

| Fader | Fader Description |
| ----- | ----------------- |
|       |                   |

#### Gobos
#### Prism
#### Strobe

### Blackout Cues

#### General
These cues are more specific to the fixtures used in this project.  

### Flash Cues

#### General
These cues are more specific to the fixtures used in this project.  


## Device Groups

### Color Selection Groups
The project has **8 Color Selection Groups** (Reason: I use an [AKAI APC Mini MIDI Controller WIP](https://github.com/FlorianGericke/DMXControl-files/tree/main/dmxControl/midi_rule_sets/apc_mini_mk_2). This MIDI controller has 8 soft buttons in one row).

You can assign as many fixtures as you like to one Color Selection Group. The purpose of a group is to select one group and then apply a color to each fixture within that group. [More WIP](#\[Color-Selection-Group\]-Handle-Color-Change-Page)

## Executors

### Transition Executers
Transition Executers have a higer Priority then Highlight Executers. These are for Build Up or situations you want to overlay somthing over you current Output. 
When a Transition Executer is aktive you can prepare the paramters for the drop, maybe using a highlight executer. When then the Transition executer is stopped the Highlight effect will be visible.


### Highlight Executors
Highlight Executers have a lower Priority then the Transition Executers.
Place drops or other special Highlight here. When a transition is canceld ther active Highlight will fire up !

### Configure Higlight or Transition Executers
#### Fader is Intensity (Default)
When the Fader should control the Intensity activate the Intensity Assignments on the 
'[ Softdeskt ] Softdesk 2 Transition Executers' Bank in the InputAssignment.
Deaktivate the Parameter Master Assignments. Only One Should be used
Activate Auto Go anf Auto Stop

#### Fader is ParameterMaster (Input Assignment)
When the Fader should control a fader aktivate the Temp Fader Assignments on the 
'[ Softdeskt ] Softdesk 2 Transition Executers' Bank in the InputAssignment.
Deaktivate the Default. Only One Should be used
Deaktivate Auto Go anf Auto Stop

### Device Setup Cues

## Masters

### Parameter Master

| Channel             | Conifg                             |
| ------------------- | ---------------------------------- |
| ParameterMaster 001 |                                    |
| ParameterMaster 002 |                                    |
| ParameterMaster 003 |                                    |
| ParameterMaster 004 |                                    |
| ParameterMaster 005 |                                    |
| ParameterMaster 006 |                                    |
| ParameterMaster 007 | LED FR Device Strobe               |
| ParameterMaster 008 |                                    |
| ParameterMaster 009 |                                    |
| ParameterMaster 010 |                                    |
| ParameterMaster 011 |                                    |
| ParameterMaster 012 |                                    |
| ParameterMaster 013 |                                    |
| ParameterMaster 014 |                                    |
| ParameterMaster 015 |                                    |
| ParameterMaster 016 |                                    |
| ParameterMaster 017 | LED FR Highlight Strobe            |
| ParameterMaster 018 |                                    |
| ParameterMaster 019 |                                    |
| ParameterMaster 020 |                                    |
| ParameterMaster 021 |                                    |
| ParameterMaster 022 |                                    |
| ParameterMaster 023 |                                    |
| ParameterMaster 024 |                                    |
| ParameterMaster 025 |                                    |
| ParameterMaster 026 |                                    |
| ParameterMaster 027 | LED BA Device Strobe               |
| ParameterMaster 028 |                                    |
| ParameterMaster 029 |                                    |
| ParameterMaster 030 |                                    |
| ParameterMaster 031 |                                    |
| ParameterMaster 032 |                                    |
| ParameterMaster 033 |                                    |
| ParameterMaster 034 |                                    |
| ParameterMaster 035 |                                    |
| ParameterMaster 036 |                                    |
| ParameterMaster 037 | LED BA Highlight Strobe            |
| ParameterMaster 038 |                                    |
| ParameterMaster 039 |                                    |
| ParameterMaster 040 |                                    |
| ParameterMaster 041 |                                    |
| ParameterMaster 042 |                                    |
| ParameterMaster 043 |                                    |
| ParameterMaster 044 |                                    |
| ParameterMaster 045 |                                    |
| ParameterMaster 046 | MOV Device Prism Rotation Speed    |
| ParameterMaster 047 | MOV Device Strobe                  |
| ParameterMaster 048 | MOV Device Gobo Shake Intensity    |
| ParameterMaster 049 |                                    |
| ParameterMaster 050 |                                    |
| ParameterMaster 051 |                                    |
| ParameterMaster 052 |                                    |
| ParameterMaster 053 |                                    |
| ParameterMaster 054 |                                    |
| ParameterMaster 055 |                                    |
| ParameterMaster 056 | MOV Highlight Prism Rotation Spped |
| ParameterMaster 057 | MOV Highlight Strobe               |
| ParameterMaster 058 | MOV Highlight Gobo Shake Intensity |
| ParameterMaster 059 |                                    |
| .                   | .                                  |
| .                   | .                                  |
| .                   | .                                  |
| ParameterMaster 100 | Transiton Executer Fader Value 0   |
| ParameterMaster 101 | Transiton Executer Fader Value 1   |
| ParameterMaster 102 | Transiton Executer Fader Value 2   |
| ParameterMaster 103 | Transiton Executer Fader Value 3   |
| ParameterMaster 104 | Transiton Executer Fader Value 4   |
| ParameterMaster 105 | Transiton Executer Fader Value 5   |
| ParameterMaster 106 | Transiton Executer Fader Value 6   |
| ParameterMaster 107 | Transiton Executer Fader Value 7   |
| ParameterMaster 108 | Transiton Executer Fader Value 8   |
| ParameterMaster 109 |                                    |
| ParameterMaster 110 |                                    |
| ParameterMaster 110 | Highlight Executer Fader Value 0   |
| ParameterMaster 110 | Highlight Executer Fader Value 1   |
| ParameterMaster 110 | Highlight Executer Fader Value 2   |
| ParameterMaster 110 | Highlight Executer Fader Value 3   |
| ParameterMaster 110 | Highlight Executer Fader Value 4   |
| ParameterMaster 110 | Highlight Executer Fader Value 5   |
| ParameterMaster 110 | Highlight Executer Fader Value 6   |
| ParameterMaster 110 | Highlight Executer Fader Value 7   |
| ParameterMaster 110 | Highlight Executer Fader Value 8   |
|                     |                                    |


### Speed Master

| Executer        | Default CueList                          |
| --------------- | ---------------------------------------- |
| SpeedMaster 001 | Main Speed                               |
| SpeedMaster 105 | Transition Executer 5 Knight Rider Speed |
|                 |                                          |

## Input Assignment

### [Color Selection Group]  - Handle Color Change Page

#### Color Selection Groups
![overview](.\img\ia-color-selection-group-overview.png)

#### Device Buttons select Color Selection Groups
![select-color-selection-groups](.\img\ia-color-selection-group-2-device-selection-buttons.png)

#### Device Buttons select Color for the selected Group
![select-color](.\img\ia-color-selection-group-3-color-selection-buttons.png)

#### Set Up Predefined Colors 
![predefined colors ](.\img/ia-color-selection-group-4-predefined-colors.png)




## DMX Input

### Fixture Config Channels

#### Fixture 01 (LED FR)

| Channel | Conifg                                            |
| ------- | ------------------------------------------------- |
| 2.011   | Conifg 1                                          |
| 2.012   | Conifg 2                                          |
| 2.013   | Conifg 3                                          |
| 2.014   | Conifg 4                                          |
| 2.015   | Conifg 5                                          |
| 2.016   | Conifg 6                                          |
| 2.017   | Conifg 7 => LED FR Dev Strobe Exevuter (11.1)     |
| 2.018   | Conifg 8 =>  LED FR Sound 2 Light Exevuter (13.1) |
|         |                                                   |


#### Fixture 02 (LED BA)

| Channel | Conifg                                           |
| ------- | ------------------------------------------------ |
| 2.031   | Conifg 1                                         |
| 2.032   | Conifg 2                                         |
| 2.033   | Conifg 3                                         |
| 2.034   | Conifg 4                                         |
| 2.035   | Conifg 5                                         |
| 2.036   | Conifg 6                                         |
| 2.037   | Conifg 7 => LED BA Dev Strobe Exevuter (11.2)    |
| 2.038   | Conifg 8 => LED Ba Sound 2 Light Exevuter (13.2) |
|         |                                                  |

#### Fixture 03 (MOV)

| Channel | Conifg                                        |
| ------- | --------------------------------------------- |
| 2.051   | Conifg 1                                      |
| 2.052   | Conifg 2                                      |
| 2.053   | Conifg 3 => MOV Dev Prism Rotaion (12.3)      |
| 2.054   | Conifg 4 => MOV Dev Gobo Shake (12.4)         |
| 2.055   | Conifg 5 => MOV Dev MOV Speed (12.5)          |
| 2.056   | Conifg 6                                      |
| 2.057   | Conifg 7 => MOV Dev Strobe Exevuter (11.3)    |
| 2.058   | Conifg 8 => MOV Sound 2 Light Exevuter (13.3) |

#### Fixture 04 (REVO)

| Channel | Conifg                                |
| ------- | ------------------------------------- |
| 2.071   | Conifg 1                              |
| 2.072   | Conifg 2                              |
| 2.073   | Conifg 3                              |
| 2.074   | Conifg 4                              |
| 2.075   | Conifg 5                              |
| 2.076   | Conifg 6                              |
| 2.077   | Conifg 7 => Strobe                    |
| 2.078   | Conifg 8 => Sound 2 Light Sensibility |

#### Fixture 05 (Mega Strobe)

| Channel | Conifg                                |
| ------- | ------------------------------------- |
| 2.091   | Conifg 1                              |
| 2.092   | Conifg 2                              |
| 2.093   | Conifg 3                              |
| 2.094   | Conifg 4                              |
| 2.095   | Conifg 5                              |
| 2.096   | Conifg 6                              |
| 2.097   | Conifg 7 => Mega Strobe               |
| 2.098   | Conifg 8 => Sound 2 Light Sensibility |


### Fixture Highlights Config Channels

#### Fixture 01 (LED FR)

| Channel | Conifg                                |
| ------- | ------------------------------------- |
| 2.021   | Conifg 1                              |
| 2.022   | Conifg 2                              |
| 2.023   | Conifg 3                              |
| 2.024   | Conifg 4                              |
| 2.025   | Conifg 5                              |
| 2.026   | Conifg 6                              |
| 2.027   | Conifg 7 => Strobe                    |
| 2.028   | Conifg 8 => Sound 2 Light Sensibility |


#### Fixture 02 (LED BA)

| Channel | Conifg                                |
| ------- | ------------------------------------- |
| 2.041   | Conifg 1                              |
| 2.042   | Conifg 2                              |
| 2.043   | Conifg 3                              |
| 2.044   | Conifg 4                              |
| 2.045   | Conifg 5                              |
| 2.046   | Conifg 6                              |
| 2.047   | Conifg 7 => Strobe                    |
| 2.048   | Conifg 8 => Sound 2 Light Sensibility |

#### Fixture 03 (MOV)

| Channel | Conifg                                |
| ------- | ------------------------------------- |
| 2.061   | Conifg 1                              |
| 2.062   | Conifg 2                              |
| 2.063   | Conifg 3 => Prism Rotaion             |
| 2.064   | Conifg 4 => Gobo Shake                |
| 2.065   | Conifg 5 => MOV Spead                 |
| 2.066   | Conifg 6                              |
| 2.067   | Conifg 7 => Strobe                    |
| 2.068   | Conifg 8 => Sound 2 Light Sensibility |

#### Fixture 04 (REVO)

| Channel | Conifg                                |
| ------- | ------------------------------------- |
| 2.081   | Conifg 1                              |
| 2.082   | Conifg 2                              |
| 2.083   | Conifg 3                              |
| 2.084   | Conifg 4                              |
| 2.085   | Conifg 5                              |
| 2.086   | Conifg 6                              |
| 2.087   | Conifg 7 => Strobe                    |
| 2.088   | Conifg 8 => Sound 2 Light Sensibility |

#### Fixture 05 (Mega Strobe)

| Channel | Conifg                                |
| ------- | ------------------------------------- |
| 2.101   | Conifg 1                              |
| 2.102   | Conifg 2                              |
| 2.103   | Conifg 3                              |
| 2.104   | Conifg 4                              |
| 2.105   | Conifg 5                              |
| 2.106   | Conifg 6                              |
| 2.107   | Conifg 7 => Strobe                    |
| 2.108   | Conifg 8 => Sound 2 Light Sensibility |


### Highlight Executer Faders

Fader Value 0 => Scene off
Fader Value 1 => Scene On

| Channel | Fader                |
| ------- | -------------------- |
| 2.131   | Highlight Executer 1 |
| 2.132   | Highlight Executer 2 |
| 2.133   | Highlight Executer 3 |
| 2.134   | Highlight Executer 4 |
| 2.135   | Highlight Executer 5 |
| 2.136   | Highlight Executer 6 |
| 2.137   | Highlight Executer 7 |
| 2.138   | Highlight Executer 8 |

### Scene And Aux Aktivation Channels

Fader Value 0 => Scene off
Fader Value 1 => Scene On

| Channel | Fader                |
| ------- | -------------------- |
| 2.151   | Scene 1 FR Blackout  |
| 2.152   | Scene 2 BA Blackout  |
| 2.153   | Scene 3 MOV Blackout |
| 2.154   | Scene 4 Mov Prism On |
| 2.155   | Scene 5              |
| 2.156   | Scene 6              |
| 2.157   | Scene 7              |
| 2.158   | Scene 8              |
| 2.159   | AUX 1                |
| 2.161   | Scene 9              |
| 2.162   | Scene 10             |
| 2.163   | Scene 11             |
| 2.164   | Scene 12             |
| 2.165   | Scene 13             |
| 2.166   | Scene 14             |
| 2.167   | Scene 15             |
| 2.168   | Scene 16             |
| 2.169   | AUX 2                |








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
Each cuelist has a priority, which determines which cue can be played over another. How priorities are set has a big impact on how the show is controlled live. To maintain a structured system, I organize my priorities into groups. Each group has a range between 0 and 9. The default priority always ends on 4 (14, 24, 34, 44, 64, ...).  
This ensures that there is always room for a higher or lower priority within a group  
(higher numbers indicate higher priority).


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


