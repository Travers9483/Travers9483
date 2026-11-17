<div align="center">

<img src="assets/banner.svg" width="100%" alt="Hi, I'm Travers. Developer working on graphics and game tech, reverse engineering, web apps, Microsoft 365 and tooling.">

<br>

I like building things that feel fast and look good: **real-time graphics and game tech in C++**,
**reverse engineering and analysis**, **Microsoft 365 solutions**, and the **tools that tie it all together**.

Most of my work lives in private repositories, so this page is the overview:
what I build, how the pieces fit together, and what I'm working on now.

<br>

<img src="assets/stats.svg" width="100%" alt="At a glance: 70+ repositories, mostly private. 50+ games on one shared menu. 5 render backends, one codebase. 9 engine families written up. 200+ MCP tools for AI assistants.">

### ✨ What I work on

<img src="assets/work.svg" width="100%" alt="Graphics and GUI: NovaGui, my own immediate-mode GUI library with DirectX 9, 11, 12, OpenGL and Vulkan. Game tech and modding: overlays, trainers and VR mods for single-player and co-op games across nine engine families. Reverse engineering: understanding compiled code, tracing behaviour, inspecting game assets and documenting findings. Game-data visualisation: turning extracted game data into overlays and visual cues, like attack telegraphs. Developer tooling: debugging utilities, reusable components and integrations that cut repetitive work. AI-assisted dev tools: MCP servers that let AI assistants drive real debugging and analysis tools. Microsoft 365 and automation: SPFx web parts, Power Apps and Power Automate, plus scripts linking Microsoft 365 and creative apps. Web apps: fast static sites, interactive maps and review tools with Leaflet, Supabase and Netlify.">

### 🌟 Featured

</div>

<table>
<tr>
<td width="52%" valign="middle"><img src="assets/novagui.png" width="100%" alt="NovaGui design study: the Slate theme, a compact overlay panel with a live preview and frame-budget readout"></td>
<td valign="middle">

#### NovaGui

My own immediate-mode GUI library in C++17. One codebase renders through **DirectX 9, 11 and 12, OpenGL and Vulkan**, and a universal menu template (rails, collapsible cards, keybinds, profiles, UI scaling) gives every overlay I build the same look and feel. More than 50 of my projects build their menu on it.

**The challenge:** identical output across five renderers and every resolution from 720p to 4K, with animation that stays smooth inside someone else's frame budget.

</td>
</tr>
<tr>
<td width="52%" valign="middle"><img src="assets/mcp.svg" width="100%" alt="Diagram: an AI assistant talks to one MCP server, which drives IDA Pro, Ghidra, x64dbg, Cheat Engine, ReClass.NET, Wireshark, Fiddler and HTTP Debugger"></td>
<td valign="middle">

#### AI-assisted analysis tooling

A Model Context Protocol server that lets AI assistants work hands-on with real tools: decompiling in **IDA Pro** and **Ghidra**, stepping through code in **x64dbg**, reading live memory with **Cheat Engine** and **ReClass.NET**, and following traffic in **Wireshark** and **Fiddler**. It exposes more than 200 tools, including a patch-day check that re-finds every saved finding after a game updates.

**The challenge:** turning a dozen very different desktop tools into one consistent, safe interface an assistant can use reliably.

</td>
</tr>
<tr>
<td width="52%" valign="middle"><img src="assets/vr.svg" width="100%" alt="Diagram: the game renders the scene for both eyes, an OpenXR frame hook adds extra composition layers (the menu as a quad layer floating in the room, the overlay as a projection layer for each eye, a wrist HUD as a quad layer on the controller), and the VR compositor blends them in the headset"></td>
<td valign="middle">

#### NovaGui inside the headset

The same menu and overlay, drawn in VR. Nothing touches the game's own images: an **OpenXR** frame hook adds extra composition layers instead. The menu is a panel floating in the room, the overlay is a projection layer for each eye, and a wrist HUD rides on the controller. The motion controllers drive all of it.

**The challenge:** drawing each eye with the game's own pose and field of view for that exact frame, so every mark stays locked to the world.

</td>
</tr>
</table>

<div align="center">

### 🧩 More I've built

</div>

<table>
<tr>
<td width="50%" valign="top">

**One core, six games**<br>
A shared trainer core for a six-game series on one engine family. The menu, overlay, settings and keybinds are written once, and each game supplies only its own addresses and hooks.

</td>
<td width="50%" valign="top">

**Engine notes and playbook**<br>
A knowledge base that carries lessons from one project to the next: notes on nine engine families, a 16-part discovery playbook, and a method guide whose first rule is that a finding must hold on two independent instances.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**NovaWall**<br>
A default-deny, per-application firewall for Windows, built on the Windows Filtering Platform with a NovaGui window. Arm it and nothing reaches the network until you allow it.

</td>
<td width="50%" valign="top">

**VEGAS NVENC fix**<br>
A small C++ fix that restores NVIDIA hardware encoding in VEGAS Pro 17 to 22, after newer drivers removed the presets those versions ask for. One click to install or remove.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**LinkForge**<br>
A script for Adobe InDesign that sends every linked image to Photoshop to resize and convert, relinks the document, and restores frame scaling so the layout looks identical.

</td>
<td width="50%" valign="top">

**SharePoint and Teams tools**<br>
An SPFx web part that shows any HTML template from a document library in an auto-resizing iframe, and a Power Apps proof of concept that publishes alerts as real-time Teams notifications through Power Automate.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**Review Map**<br>
A community map for location reviews: Leaflet on the front, Supabase with row-level security behind it, social login, video embeds and an admin moderation panel, hosted on Netlify.

</td>
<td width="50%" valign="top">

**Circle of Doom**<br>
A single-player arena-survival game for the browser, drawn on HTML5 Canvas, with a closing safe circle, upgrade drafts and boss encounters.

</td>
</tr>
</table>

<div align="center">

### 🧰 Tech I use

<img src="assets/stack.svg" width="100%" alt="Working with: languages C++, C#, TypeScript, JavaScript, PowerShell, Python, Lua, HLSL. Graphics and VR: DirectX 9 to 12, OpenGL, Vulkan, OpenXR. Game engines: Unreal 4 and 5, Unity, Frostbite, 4A Engine, CryEngine, Decima, Saber Swarm, Volition CTG, RAGE. Reverse engineering: IDA Pro, Ghidra, x64dbg, Cheat Engine, ReClass.NET, Process Hacker. Network and debugging: Wireshark, Fiddler, HTTP Debugger. Web: HTML and CSS, Node.js, Leaflet, Supabase, Netlify. Microsoft 365: SharePoint (SPFx), Power Apps, Power Automate, Microsoft Teams. Creative and video: Photoshop, InDesign, After Effects, VEGAS Pro, OBS Studio. Dev tools: Visual Studio, VS Code, Git, GitHub, Claude and MCP. Exploring: DirectX 12 internals, game telegraphs, model geometry, id Tech, Dunia, Source.">

### 🚀 Right now

<img src="assets/now.svg" width="100%" alt="Right now: refining NovaGui and the menu template behind 50+ projects; bringing new engines onto the template: id Tech, Dunia and RAGE; exploring game telegraphs, model geometry and visualisation; connecting AI assistants to debugging and analysis tools through MCP; building SharePoint components and workflow automation.">

</div>

<table>
<tr>
<td width="50%" valign="top">

### 🧠 How I work

I use AI heavily for prototyping and development, often several agents in parallel, alongside hands-on debugging, testing and reverse engineering. I enjoy working through unfamiliar systems, figuring out what's actually happening, and iterating until the result works.

- **Evidence first.** Every finding is labelled as proven in the running game, built but unconfirmed, or untested.
- **Built to survive updates.** Signatures instead of fixed addresses, and tooling that re-checks saved findings after a patch.

Along the way I keep short technical write-ups: the problem, what I tried, and what I learned.

</td>
<td width="50%" valign="top">

### 🤝 Open to

Microsoft 365 development, internal tools, workflow automation and developer tooling.

Always happy to compare notes on C++ interfaces, graphics and AI-assisted development.

</td>
</tr>
</table>

<div align="center">

<br>

<img src="assets/footer.svg" width="100%" alt="Thanks for stopping by">

</div>
