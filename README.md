# Secret-server-rs
The **secure Server** is a secure backend designed to manage user secrets (passkeys, OTPs) for authentication in Progessive Web Apps (PWAs). Ut ensures secure key storag, supports passkey-based authentication, and handles offline scenarios to provide a seamless user experience.

## Key Features
- **Key Pair Generation**: Each PWA generates its own key pair for authentication.
- **Secure Secret Storage**: Encrypted user secrets (PINs, passkeys) are securely backed up to the server.
- **Passkey Recovery**: Users can authenticate via passkeys, or recover secrets using their Pin if passkeys are unavailable.
- **TOTP Fallback**: Provides time-based OTPs as a secondary recovery method.
- **Offline Support**: Locally encrypted secrets can be accessed using a PIN in offline mode.

## Getting Started

### Prerequisites

- **Rust** (latest stable version)
- **SQLite** for local database storage

### Setup

1. **Clone the repository**:
   ```bash
   git@github.com:ADORSYS-GIS/Secret-server-rs.git
   ```
2. **Build the project**:
    ```bash
    cargo build
    ```
3. **Run the server**:
    ```bash
    cargo run
    ```
### Testing
To run the tests:
```bash
cargo test
```