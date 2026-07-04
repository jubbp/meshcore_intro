---
title: Get Connected
permalink: /get-connected/
description: "Step-by-step onboarding for Bunbury MeshCore with two paths: use the network quickly or build and flash your own node."
---

<!-- markdownlint-disable MD033 MD012 MD032 -->

{% include nav.html %}

## Get Connected

<p class="lede">
Choose the path that matches you best. You can either build your own node, or start by using the network with minimal setup.
</p>

<section class="stream-split" aria-label="Choose your path">
  <article class="card stream-card">
    <p class="eyebrow">Stream 1</p>
    <h2>I just want to use the network</h2>
    <p>
      Best for everyday users who want practical communication options first, with the smallest possible learning curve.
    </p>
    <a class="button button-primary" href="#just-use">Go to user steps</a>
  </article>

  <article class="card stream-card">
    <p class="eyebrow">Stream 2</p>
    <h2>I want to build a node</h2>
    <p>
      Best for makers and tinkerers who want to flash hardware, choose a node role, and actively help grow the Bunbury mesh.
    </p>
    <a class="button button-primary" href="#build-node">Go to maker steps</a>
  </article>
</section>

<section class="stream-detail-grid">
  <div class="stream-detail-card card" markdown="1">

## Stream 1: Just use the network {#just-use}

### 1. Install the companion app

You can start with the app and a simple node setup, without becoming a hardware builder on day one.

- iOS: [MeshCore iOS app](https://apps.apple.com/us/app/meshcore/id6742354151?platform=iphone)
- Android: [MeshCore Android app](https://play.google.com/store/apps/details?id=com.liamcottle.meshcore.android)

The app lets you message, view nearby activity, and manage compatible nodes with a guided interface.

### 2. Ready-made / pre-flashed node option

There is currently **no regular local Bunbury retail source** for ready-made MeshCore hardware.

Most people either:

- buy compatible hardware online and flash it to MeshCore, or
- ask for one-on-one help to buy the right device and get it configured.

Important: much of the hardware sold online is marketed for Meshtastic. That is usually fine, but it still needs to be flashed to **MeshCore firmware** before use on this network.

If none are available right now, use [Contact Us]({{ '/contact/' | relative_url }}) and ask for the easiest current path.

### 3. What you can do now vs later

What you can do quickly:

- Join conversations
- Send and receive short messages
- Learn the basics of how local mesh comms feels in practice

What usually needs a maker-built node:

- Setting up repeater infrastructure
- Running a room server role
- Advanced remote management and tuning

### 4. Bespoke help for your case

If your use case is unique (family safety, community group, local event, emergency prep), use the [Contact Us]({{ '/contact/' | relative_url }}) form and we can suggest a practical setup.

  </div>

  <div class="stream-detail-card card" markdown="1">

## Stream 2: Build a node {#build-node}

### 1. Recommended hardware

There is currently **no consistent local Bunbury hardware seller**, so plan to buy online.

- Primary pick: **Heltec V3 (WiFi LoRa 32 V3)**
- Typical cost: around **AUD $45-$80** depending on source and shipping
- Good starter search links:
  - [AliExpress: Heltec WiFi LoRa 32 V3](https://www.aliexpress.com/wholesale?SearchText=Heltec+WiFi+LoRa+32+V3)
  - [AliExpress: LILYGO LoRa32 boards](https://www.aliexpress.com/wholesale?SearchText=LILYGO+LoRa32)
  - [Heltec official product page](https://heltec.org/project/wifi-lora-32-v3/)

Before ordering, check the [MeshCore Flasher](https://meshcore.io/flasher) supported device list so you do not buy unsupported hardware.

If you are unsure what to buy locally, use [Contact Us]({{ '/contact/' | relative_url }}) and ask for the latest Bunbury-tested options.

### 2. Flashing steps (and common gotchas)

1. Connect your Heltec V3 by USB data cable.
2. Open the official [MeshCore Flasher](https://meshcore.io/flasher).
3. Pick the exact board model, then select firmware type.
4. Flash and wait for completion before unplugging.

Most online devices arrive preloaded for Meshtastic or with vendor demo firmware. That is normal. You can still use them, but they must be reflashed to MeshCore first.

Common gotchas:

- Missing USB serial drivers can prevent the board from showing up.
- Charge-only USB cables look connected but do not pass data.
- Make sure you select the correct firmware variant for your intended role (Companion vs Repeater vs Room Server).

### 3. Choose a role: client / repeater / room server

- **Client (Companion):** personal use and messaging.
- **Repeater:** extends local coverage by relaying traffic.
- **Room Server:** hosts shared room-style posting and coordination.

If these roles are new to you, read [What Is MeshCore?]({{ '/what-is-meshcore/' | relative_url }}) first, then return here.

### 4. Join the Bunbury mesh (local settings)

Use the current Bunbury baseline settings when you onboard:

- Channel name: **Bunbury** (confirm latest local standard)
- Region / frequency plan: **Australia AU915** unless advised otherwise
- Node naming convention: **Suburb-Name-Number** (example: `Withers-Chris-01`)

Settings can change as the network evolves, so verify current values through the local team before final deployment.

### 5. CLI cheat-sheet reference

Use the existing CLI reference instead of duplicating commands here:

- [MeshCore CLI reference](https://github.com/fdlamotte/meshcore-cli)

### 6. Where to get help

- Start with the [Contact Us]({{ '/contact/' | relative_url }}) page for local onboarding help.
- Ask for the current Bunbury community channel details.
- Ask to be pointed to NewsWest items and local updates relevant to MeshCore.

  </div>
</section>


