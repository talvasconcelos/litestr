# Nostr Standalone Client

A simple, standalone Nostr client that works by just running an HTML file. This client allows you to read Nostr notes locally without needing any server-side setup.

## Features

- **Lightweight**: Runs entirely in the browser with no server-side dependencies.
- **Nostr Protocol**: Connects to Nostr relays and fetches notes.
- **Simple UI**: Built with Pico CSS for a clean and minimal interface.
- **Persistent Settings**: Stores the public key in local storage to persist sessions.

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, etc.)

### Setup

1. **Download the HTML File**: Download the `index.html` file from the repository.
2. **Open the File**: Simply open the HTML file in your web browser.
3. **Add Public Key**: Click on the "Add Pubkey" button in the navigation bar to enter your Nostr public key (`npub...` format). This key is stored locally in your browser's local storage.

## Usage

- **Viewing Notes**: Once the public key is set, the client will connect to Nostr relays and display the notes from followed profiles.
- **Updating Notes**: The client automatically fetches new notes from the Nostr relays.
- **Adjust Settings**: The public key can be updated or removed via the modal dialog.

## Technical Overview

- **HTML/CSS**: The UI is built using HTML and styled with [Pico CSS](https://picocss.com/).
- **JavaScript**: Uses the [Nostr Tools](https://github.com/fiatjaf/nostr-tools) library for interacting with Nostr protocol and relays.
- **Local Storage**: Public keys are saved in the browser's local storage for persistent settings across sessions.

## Nostr Relays

The client connects to the following relays by default:

- `wss://relay.nostr.band/`
- `wss://nostr-pub.wellorder.net/`
- `wss://relay.damus.io/`

These relays are used to fetch notes from profiles you follow.

## Development

To modify the client:

1. Clone the repository.
2. Open the HTML file in a code editor.
3. Modify as needed, and test by opening the HTML file in your browser.

### Future Improvements

- Improve error handling and feedback for the user.
- Expand the UI with more interactive features.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests for improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Nostr Tools](https://github.com/fiatjaf/nostr-tools) for the core functionality.
- [Pico CSS](https://picocss.com/) for the lightweight CSS framework.

---

Enjoy using the Nostr Standalone Client!
