# Restaurant Review - README

Welcome to the **Restaurant Review** project repository! This decentralized application (Dapp) stores restaurant reviews added by users in a permissionless manner. Users of this Dapp are allowed to add reviews containing the title, description, location and rating for a given restaurant and also update it's review (not currently available in the application GUI).

## Table of Contents

- [Restaurant Review - README](#restaurant-review---readme)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Features](#features)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
  - [Usage](#usage)
  - [Solana Programs](#solana-programs)
  - [Frontend](#frontend)
  - [License](#license)

## Overview

The **Restaurant Review** provides a simple interface for interacting with a Solana program deployed on devnet. Reviews are categorized by title and the user wallet adding it.

## Features

- Add Restaurant reviews, categorized by title and user (public key)
- Update proprietary reviews (not currently available in the GUI)
- Visualize past reviews from all users in the GUI

## Getting Started

Follow these steps to set up the project locally and start submitting decentralized restaurant reviews.

### Prerequisites

1. Node.js: Ensure Node.js is installed. Download it from [nodejs.org](https://nodejs.org/).
2. Cargo: Ensure cargo is installed, the rust language package manager and development toolbox.

### Installation

1. Clone the repository:

```bash
  git clone https://github.com/yuriarthf/solana-bootcamp-final-project.git
```

2. Install cargo dependencies:

```bash
  cargo install
```

3. Navigate to frontend directory:

```bash
 cd ./frontend
```

4. Install NPM dependencies for the frontend

```bash
 yarn install
 or
 npm install
```

## Usage

1. Navigate to frontend directory:

```bash
 npm start
```

2. Start the development server:
   
```bash
 npm dev
```

3. Open your web browser and navigate to `http://localhost:3000` to access the DApp.

4. Connect your Solana wallet (e.g., Phantom, Solflare) to the DApp.

6. Add your restaurant reviews

## Solana Programs

The Solana program behind this project can be found in the `./src` folder, which consists of 3 `.rs` (rust) files.

- `lib.rs`: Program entrypoint and operation related functions.
- `instruction.rs`: Logic for deserializing instruction data sent to the program.
- `state.rs`: Restaurant review PDA format (**AccountState**) and custom errors.

## Frontend

The DApp frontend is built using modern web technologies including React.js. It provides an intuitive and interactive user interface for decentralized restaurant reviewing.

- **React.js**: Powers the DApp's user interface.
- **@solana/web3.js**: The Solana JavaScript API for program interaction.
- **Multiwallet**: Phantom and Solflare wallet compatibility.

## License

This project is licensed under the [MIT License](LICENSE).

