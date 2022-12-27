# Fork Engine Specification (Revision 1.0, 2022.12.27)

1. [Introduction](#introduction)
2. [Prerequisite](#prerequisite)
3. [Limitations](#limitations)
4. [Modules](#modules)
    1. [Game Framework](#game-framework)
        1. [Graphics](#graphics)
        2. [Input](#input)
        3. [Sound](#sound)
        4. [File IO](#file-io)
    2. [Game Engine](#game-engine)
    3. [Game Logic](#game-logic)
        1. [Application](#application)
        2. [Assets](#assets)
        3. [Behavior](#behavior)
        4. [Interaction](#interaction)

# Introduction

This book introduced the design of Fork Engine. It will be active until Fork Engine is released.

Fork Engine is a new game engine that includes framework, engine and the main logic of game.

# Prerequisite

The specification and implementation of Fork Engine is given by **XenFork Union**.

Fork Engine *will be* implemented with Java 21 *or* 25.

Fork Engine *will be* implemented with OpenGL 3.2.

# Limitations

Fork Engine *will be* open-source with .

# Modules

We separate Fork Engine into three submodules.

The relationship of the submodules are introduced with this table:

<table style="text-align:center;">
<tr>
    <th>Logic</th>
    <td>Application</td>
    <td>Assets</td>
    <td>Behavior</td>
    <td>Interaction</td>
</tr>

<tr>
    <th rowspan="2">Engine</th>
    <td rowspan="2">Game Loop</td>
    <td>Asset Manager</td>
    <td>Load/Save</td>
    <td>Physics Engine</td>
</tr>
<tr>
    <td>Model & Mesh</td>
    <td>User Interface</td>
    <td>Network</td>
</tr>

<tr>
    <th rowspan="2">Framework</th>
    <td>Graphics</td>
    <td>Sound</td>
    <td>Input</td>
    <td>File IO</td>
</tr>
<tr>
    <td colspan="4">Hardware</td>
</tr>
</table>

## Game Framework

### Graphics

**Graphics** allows you to render things.

#### Batch

#### Font

### Sound

### Input

**Input** allows you to access keyboard and mouse.

### File IO

## Game Engine

## Game Logic

### Application

A base application that provides the implementation of [Engine](#game-engine) module. It will invoke the Engine module
to start the game loop.

### Assets

### Behavior

### Interaction
