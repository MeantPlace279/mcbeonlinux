# Minecraft Bedrock on Linux

A complete guide to every known method of running Minecraft Bedrock Edition on Linux.

---

# Ranking (Top 3)

> The ranking is the opinion of this guide's author.

**1. 🥇 [BedrockOnLinux](#method-6-bedrockonlinux)**

**2. 🥈 [mcpelauncher](#method-1-mcpelauncher)**

**3. 🥉 [Flarial Client](#method-7-flarial-client)**

# Method 1: mcpelauncher 

The original launcher and the foundation of nearly every Android-based Bedrock launcher on Linux. It requires owning Minecraft through Google Play and automatically downloads the APK using your Google account.

> [!WARNING]
> ChristopherHX (maintainer of mcpelauncher) [stated](https://discord.com/channels/429580677617418240/429580677617418243/1475181891043725404) on the [official Discord](https://discord.gg/UkXJMCcxhr) on **22 February 2026**:
>
> > "Yes we are sitting on top a cave full of tnt, you have no long term update warranties. Update delays / stops could happen at any point of time, since the DRM has been enabled."

### Features

- Requires owning Minecraft on Google Play; uses your own purchased copy of Minecraft. 
- Downloads the APK directly from Google Play.
- Custom APKs are **NOT** supported. ❌
- The first launcher ever to run Minecraft Bedrock on Linux.
- DRM support: ✅ ([What does this mean?](#what-does-drm-support-mean-in-android-based-methods))

### Resources

- [Repository](https://github.com/minecraft-linux/mcpelauncher-manifest)
- [Documentation](https://mcpelauncher.readthedocs.io/en/latest/getting_started/index.html)
- [Tutorial](https://youtu.be/rg_OH-nmoeQ?si=RNMzFO5ml4G2WJbF)

---

# Method 2: Trinity Launcher

> [!WARNING]
> The highest supported Minecraft version on **x86_64** systems with this launcher is **1.26.52.3**.

A modern launcher built on top of the standard mcpelauncher utilities. It adds version management together with integrated mod and texture pack support.

### Features

- Uses `mcpelauncher-client`
- Uses `mcpelauncher-extract`
- Supports custom APKs
- Built with C++
- Built-in version management
- DRM support: ❌ ([What does this mean?](#what-does-drm-support-mean-in-android-based-methods))

### Resources

- [Repository](https://github.com/Trinity-LA/Trinity-Launcher)
- [Documentation](https://trinitylauncher.vercel.app/)
- [Tutorial](https://youtu.be/ZMAamMBm8Go?si=qwZ7xOhtclxPyDw7)

---

# Method 3: Cianova Launcher

Developed by `craftplaga`, a member of the [*Las Tortuguitas de Ezku*](https://discord.com/invite/las-tortuguitas-de-ezku-1214414622111567892) Discord community.

A Python launcher featuring a graphical interface built with CustomTkinter.

> [!NOTE]
> The `PlaGaPlusDev` and `CianovaTeam` GitHub accounts redirect to the same project, so the repository may appear under either name.

### Features

- Uses `mcpelauncher-client`
- Uses `mcpelauncher-extract`
- Supports official Google Play APKs
- Supports custom APKs
- Built with Python
- Offers to install the DRM mod (`mcpelauncher-updates`) when it is missing
- DRM support: ✅ ([What does this mean?](#what-does-drm-support-mean-in-android-based-methods))

### Resources

- [Website](https://cianovalauncher.org)
- [Repository](https://github.com/PlaGaPlusDev/CianovaLauncher-mcpelauncher)
- [Tutorial](https://youtu.be/-tl4ZSJ3DSE?si=-xfBd_xV1Of5XfHI)

---

# Method 4: GenovaLauncher

A graphical Minecraft Bedrock launcher for Linux built with Python and PySide6 (Qt6).

### Features

- Automatic mcpelauncher binary detection.
- Install versions from APK files or Google Play
- Built-in version management.
- Resource packs, behavior packs, skins, and worlds management.
- Integrated mod browser.
- Independent profiles.
- Customizable appearance and launch options.
- GameMode and Zink support.
- DRM support: ✅ ([What does this mean?](#what-does-drm-support-mean-in-android-based-methods))

### Installation

#### Portable Release

```sh
wget https://github.com/Ars-byte/GenovaLauncher-launcher/releases/latest/download/GenovaLauncher-v1.0.0.tar.gz

tar xzf GenovaLauncher-v1.0.0.tar.gz && cd GenovaLauncher-v1.0.0

./GenovaLauncher.sh
```

### Resources

- [Website](https://ars-byte.github.io/genovalauncher-website/pages/docs.html)
- [Repository](https://github.com/Ars-byte/GenovaLauncher-launcher)

---

# Method 5: Iosel Edition

A modified AppImage fork of mcpelauncher.

It claims to remove the dependency on the Flatpak runtime and was reportedly created by a contributor associated with the Trinity project.

### Features

- Supports custom APKs
- Standalone AppImage
- No Flatpak runtime required
- DRM support: ❌ ([What does this mean?](#what-does-drm-support-mean-in-android-based-methods))

### Resources

- [Repository](https://github.com/IoselDev/Minecraft-Bedrock-Linux-Iosel-Edition)
- [Tutorial](https://youtu.be/BAZqN_NhIj4?si=eEuOY4TvDeE_VpWQ)

---

# Method 6: BedrockOnLinux

A launcher that runs the **Windows version of Minecraft Bedrock Edition directly on Linux** using your own Microsoft account and licence.

Unlike Methods 1–5, this does **not** use the Android version of Minecraft or `mcpelauncher-client`.

### Features

- Runs the Windows version of Minecraft Bedrock.
- Supports clients via DLL.
- Real Microsoft/Xbox sign-in.
- Friends, public servers and Realms.
- Marketplace support.
- Supports Minecraft Preview.
- Supports older Minecraft versions.
- Controller support.
- Steam Deck support.
- Available as AppImage, `.deb`, `.rpm`, Flatpak and Nix.

### Requirements

- 64-bit Linux.
- A Vulkan-capable GPU and working drivers.
- A Microsoft account that owns Minecraft.
- A few GB of free disk space.

### Resources

- [Repository](https://github.com/Wyze3306/BedrockOnLinux)

---

# Method 7: Flarial Client

A launcher that also runs Minecraft for Windows (Bedrock Edition) on Linux using Wine/Proton and provides access to the Flarial Client.

This method uses the Windows version of Minecraft Bedrock and requires a Microsoft account that owns Minecraft for Windows.

### Features

- Runs the Windows version of Minecraft Bedrock.
- Integrates Wine setup into the launcher.
- Supports Microsoft account sign-in.
- Provides access to the Flarial Client.
- Downloads and manages supported Minecraft versions through the launcher.
- Opens the Flarial menu in-game using the `K` key.

### Requirements

- 64-bit x86 Linux.
- Working Vulkan graphics drivers.
- A Microsoft account that owns Minecraft for Windows (Bedrock).

### Installation

Open a terminal and run the following command as your normal user. **No `sudo` is required.**

```sh
curl -fsSL https://cdn.flarial.xyz/launcher/linux/install.sh | sh
```

### Resources

- [Website](https://flarial.xyz/download/?p=linux#installation)
- [Repository](https://github.com/flarialmc/linux)

---

# Method 8: GDK Version via ProtonGDK

The methods mentioned above (BedrockOnLinux and Flarial Client) are understood to use this approach behind the scenes.

Minecraft Bedrock on Windows has transitioned from UWP to GDK.

This method runs the native Windows GDK version through ProtonGDK together with proxy workarounds.

### Features

- Runs the actual Windows PC version.
- Does not rely on Android.
- Lengthy setup.
- Recommended only if Android-based methods fail.

### Resources

- [Video Tutorial](https://youtu.be/m76O2cRIEnM?si=YV2dxJpvLTYKtIDh)
- [Text Tutorial](https://github.com/inbob1/mcbe-on-linux)

---

# Method 9: Windows Virtual Machine

Run Windows inside a virtual machine and play Minecraft Bedrock normally.

### Features

- Native Windows version
- Works reliably
- Higher resource usage
- Best used as a last resort

---

# Android Dependency

> [!IMPORTANT]
> All Android-based methods listed above (Methods 1–5, including mcpelauncher itself) ultimately depend on `mcpelauncher-client` and `mcpelauncher-extract` from the `mcpelauncher-manifest` project. If that project ever becomes unavailable, every Android-based launcher listed above will eventually stop working.

---

# What does DRM support mean in Android-based methods?

DRM stands for Digital Rights Management.

Newer Minecraft Bedrock APKs distributed through Google Play are protected by Google Play's DRM and integrity checks (the `mcpelauncher-manifest` project cites Google Advanced Integrity Protection).

Because of this, `mcpelauncher-client` from the `mcpelauncher-manifest` project can't run these newer versions on its own.

The `mcpelauncher-updates` mod is what makes them run. It carries the per-version patches and compatibility code the newer builds need.

That's why it's often called the DRM support mod.

### How DRM support is judged

- ✅ The launcher works with the `mcpelauncher-updates` mod and keeps providing newer Minecraft versions.

- ❌ The launcher can't use the mod, or it has stopped providing newer versions.

---

# Outdated Methods

## Waydroid

Waydroid previously ran Minecraft inside a complete Android environment.

Recent Minecraft versions become stuck at the loading screen, making this method unusable.

---

## CCMC Launcher by Crow_Rei34

CCMC Launcher worked similarly to Trinity by extracting and launching custom APKs.

The GitHub repository has since been deleted or made private.

The [Codeberg](https://codeberg.org/Crow_Rei34/CC-MC) repository is still available.

It is believed to have been discontinued when Trinity Launcher was introduced, as both projects shared a developer (JavierC).

<img width="698" height="904" alt="image" src="https://github.com/user-attachments/assets/b993b443-6ff6-4c29-ad14-813fe320a887" />


### Historical Tutorials (Portuguese)
- [Tutorial 1](https://youtu.be/4K1X8PafWf0?si=jZe4X5xsA9nplT5h)
- [Tutorial 2](https://youtu.be/VfVwqMcKhy0?si=_C70rhEyabASEKgb)
- [Tutorial 3](https://youtu.be/sYvpEpwin6k?si=sD631OfATfYwzbH1)
