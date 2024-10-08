---
sidebar_position: 1
---

# Introduction

Welcome to the Pure Fabric Modding API! This is meant to be a easy-to-learn, extensive, and permissive API libary that allowd developers to modify Minecraft beyond it's normal limits, while still keeping true to Minecraft.

Pure Fabric uses Fabric as it's Mod Loader, and greatly improves upon the Fabric API, hence the name "Pure Fabric".

## How It Works

Pure Fabric treats Minecraft as a game engine, allowing you to build apon it, without the need of using another game engine. You can then start creating componenets such as your shaders, items, blocks, models, ect...

It also takes parts of the Forge API, making it more powerful than most Fabric Libaries, while still (somewhat) keeping its optimization.

While treating Minecraft as a game engine, it is still important to remember Minecraft is clunky and unoptimized, so we highgly recommend adding optimizations, and not going overboard.

## Quick Start

### Prerequisites

- A basic knowledge of Java, and how Minecraft Modding works.
- You have an offical version of Minecraft: Java Edition, that is not hacked.

### Adding VIA Gradle

```js
repositories {
    maven { url "https://maven.skrillx13.me/" }
    maven { url "https://maven.pure-fabric.com/releases/" }
}

dependencies {
    [...]
    modApi("me.skrillx13:pure-fabric:ABC") {
        exclude(group: "net.fabricmc.fabric-api")
    }
}
```