# Rhuan Alves Inocêncio

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rhuaninocencio)
[![NuGet](https://img.shields.io/badge/NuGet-004880?style=for-the-badge&logo=nuget&logoColor=white)](https://www.nuget.org/profiles/rhuan09)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rhuanalvesinocencio@gmail.com)

**Software engineer working in C# and .NET, mostly on the layer underneath other people's
software** — native Windows integration, file formats, and tooling that has to be correct
before it is convenient.

The thing I care about most is the boundary. A library that reads a file someone downloaded,
or a server that hands an AI agent control of a desktop, is holding untrusted input either
way. I would rather state the threat model and design against it than leave it implied.

---

## Projects

### 🤖 [HeyAI](https://github.com/Rhuan09/HeyAI)

**A typed, policed MCP surface onto native Windows APIs — with a permission model, not just
a PowerShell hole.**

An MCP server that lets an agent read what is playing, control media, manage windows and
read the screen through native WinRT, behind a deny-by-default allowlist, per-invocation
risk classification, and an append-only audit log the agent cannot reach. Actions marked
critical are never approved automatically; untrusted screen reads lock them out for a
window afterwards.

`C#` · `.NET 10` · `WinRT` · `Win32` · `MSIX`

### 📦 [SafeTensors.NET](https://github.com/Rhuan09/SafeTensors.NET) · [![NuGet](https://img.shields.io/nuget/v/SafeTensors.NET.svg)](https://www.nuget.org/packages/SafeTensors.NET)

**Zero-copy reader and writer for the SafeTensors tensor format, without a deep learning
runtime attached.**

Opens a multi-gigabyte model checkpoint for the cost of parsing its header, then hands out
tensors as spans over the mapped pages. 150 KB, no dependencies, Native AOT compatible,
and it treats every checkpoint as the untrusted download it usually is — overlapping byte
ranges, shapes that overflow, and shard names that escape the model directory are all
rejected before a single byte is handed out.

`C#` · `netstandard2.0` · `net8.0` · `net10.0` · `Native AOT`

### 🏥 [Clinica_Vet](https://github.com/Rhuan09/Clinica_Vet)

Veterinary clinic management desktop application — patient records, appointments and
inventory, built on MVVM with local persistence.

`C#` · `WinUI 3` · `XAML` · `SQLite` · `EF Core`

### 🏛️ [TCC-Ilha_Anchieta](https://github.com/Rhuan09/TCC-Ilha_Anchieta)

Undergraduate capstone: an interactive 3D reconstruction of Ilha Anchieta's architectural
heritage and terrain, with standalone Windows and macOS builds.

`C#` · `Unity` · `URP`

### 🛒 [AStarSuperMarket](https://github.com/Rhuan09/AStarSuperMarket)

A\* pathfinding over retail floor topology, with custom graph models, an admissible
heuristic, and a browser visualisation.

`C#` · `ASP.NET Core` · `HTML5 Canvas`

### 📱 [Apt293](https://github.com/Rhuan09/Apt293)

Household budgeting and shared expense tracking, with reactive state management and
categorised fixed/variable auditing.

`Flutter` · `Dart` · `BLoC`

---

## What I reach for

**Daily** — C#, .NET, WinUI 3 and the Windows App SDK, WinRT and Win32 interop,
ASP.NET Core, Entity Framework Core, GitHub Actions.

**Regularly** — Flutter and Dart, TypeScript, SQL against PostgreSQL and SQLite, Unity.

**Currently interested in** — the Model Context Protocol and the security model it needs
to have, local LLM tooling, and .NET as a place to actually run inference rather than
just orchestrate it.

---

## Contact

**Brazil** · [LinkedIn](https://www.linkedin.com/in/rhuaninocencio) ·
[rhuanalvesinocencio@gmail.com](mailto:rhuanalvesinocencio@gmail.com)
