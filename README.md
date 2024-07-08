# Extism Plug-In: Hello World

## Introduction

Welcome to the **Hello World** Extism plug-in! This plug-in is written in Go and compiled to WebAssembly using TinyGo. It provides a simple function that takes an input string (typically someone's name) and returns a greeting message. This plug-in serves as an example of how to interact with extism plug-ins using the Extism CLI.

## Getting Started

### Prerequisites

Before you can use this plug-in, ensure you have the following installed:

- **TinyGo**: A Go compiler for WebAssembly.
- **Extism CLI**: The command-line interface for managing and running Extism plug-ins.

### Installation

#### Install TinyGo

Follow the installation instructions for your operating system from the [TinyGo website](https://tinygo.org/getting-started/).

#### Install Extism CLI

Follow the installation instructions from the [Extism documentation](https://extism.dev/docs/cli/installation).

## Building the Plug-In

1. **Clone the Repository**

   Clone this repository to your local machine:

   ```sh
   git clone https://github.com/yourusername/hello-world-plugin.git
   cd hello-world-plugin


2. **Build the Plug-In**

    Use TinyGo to compile the Go source code into a WebAssembly module:

    ```sh
    tinygo build -o plugin.wasm -target=wasi main.go


## Using the Plug-In

1. **Calling the Plug-In with Extism CLI**

    Use the below run command to test the plug in

    ```sh
    extism call plugin.wasm greet --input "{your name goes here}" --wasi
