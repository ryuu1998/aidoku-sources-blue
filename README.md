# Weebdex Aidoku Extension

This is an [Aidoku](https://aidoku.app) extension for [Weebdex](https://weebdex.org), implemented in Rust.

## Features

- **Browse & Search**: Explore the latest, popular, and new manga listings.
- **Manga Details**: view descriptions, status, and metadata.
- **Chapter Support**: Full chapter list with volume and upload date information.
- **Image Gallery**: High-quality page loading from Weebdex nodes.
- **Deep Linking**: Open Weebdex manga URLs directly in Aidoku.

## Installation

To add this source to Aidoku, you can add this repository's source list:

1. Copy the **Raw URL** of `index.min.json` from this repository.
   - Example: `https://raw.githubusercontent.com/YourUsername/YourRepoName/main/index.min.json`
2. Open Aidoku and go to **Settings > Browse > Source Lists**.
3. Tap **Add Source List** and paste the URL.
4. Tap **Add**, then find **Weebdex** in your Browse tab.

## Building from Source

If you want to build the extension yourself:

1. Install [Rust](https://rustup.rs).
2. Add the WASM target:
   ```bash
   rustup target add wasm32-unknown-unknown
   ```
3. Build the project:
   ```bash
   cargo build --release --target wasm32-unknown-unknown
   ```
4. Find the `.wasm` file in `target/wasm32-unknown-unknown/release/weebdex.wasm`.

## Credits

- Built with [aidoku-rs](https://github.com/Aidoku/aidoku-rs).
- Content provided by [Weebdex](https://weebdex.org).
