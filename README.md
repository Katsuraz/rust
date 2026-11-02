# RustCraft — Milestone 1

An original Minecraft-inspired voxel sandbox written in Rust with Macroquad.

## Features
- Generated hills and trees with six block types
- First-person camera, WASD movement, jumping, gravity, sprinting and collisions
- Left-click mining, right-click placement, block targeting
- Six-slot hotbar, mouse wheel selection
- Toggleable creative flight, world reset, FPS and coordinates

## Build on Windows 10/11
1. Install Rust from https://rustup.rs/ (install C++ build tools if prompted).
2. Extract this ZIP.
3. Open a terminal in the `rustcraft` folder (the folder containing `Cargo.toml`).
4. Run `cargo run --release`.
5. The compiled executable will be `target/release/rustcraft.exe`.

Internet is needed on first build to download Macroquad dependencies. This environment did not have the Rust compiler, so the project has not been compile-tested here.

## Controls
- Click game window: capture mouse
- Escape: release mouse
- WASD: move
- Mouse: look
- Space: jump (or ascend in fly mode)
- Left Shift: sprint
- Left Control: descend while flying
- Left mouse: break block
- Right mouse: place selected block
- 1–6 or mouse wheel: select block
- F: toggle flying
- R: regenerate world (discards edits)

## Limitations
This is a first milestone, not a full Minecraft clone. Terrain is finite, blocks are untextured, and world edits are not saved. It has no crafting, mobs, survival systems, multiplayer, or advanced chunk meshing yet. Rendering individual visible cubes is deliberately simple and will require greedy meshing and chunk streaming for larger worlds.

## Roadmap
1. Chunked world storage, face culling and greedy meshes
2. Save/load, improved terrain noise and biomes
3. Texture atlas, inventory and crafting
4. Survival systems, lighting, caves and ores
5. Entities, AI, farming and structures
6. Redstone-inspired logic, networking and modding APIs

RustCraft is an independent original project. No Minecraft assets or code are included.
