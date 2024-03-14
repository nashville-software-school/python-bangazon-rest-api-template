# Bangazon Platform API

## System Dependencies

1. Follow installation guide for installing [pipx](https://pipx.pypa.io/stable/installation/).
2. Run `pipx install poetry`.
3. Run the command below for your operating system.

### Mac OS

```sh
brew install libtiff libjpeg webp little-cms2
```

### Linux

```sh
sudo apt install libtiff5-dev libjpeg8-dev libopenjp2-7-dev zlib1g-dev \
    libfreetype6-dev liblcms2-dev libwebp-dev tcl8.6-dev tk8.6-dev python3-tk \
    libharfbuzz-dev libfribidi-dev libxcb1-dev
```

## Setup

1. Clone this repository and change to the directory in the terminal.
2. Run `poetry install`
3. Run `poetry shell`
4. Run migrations and install starter data with the `./seed_data.sh` script.
5. Open the project in VS Code if you haven't yet.
6. Ensure that the correct Python Interpreter is chosen in VS Code.
7. Start your debugger.

## Postman Request Collection

1. Open Postman
1. Click Import from the navbar
1. Choose the Link option
1. Paste in this URL:
    `https://www.getpostman.com/collections/c29b98258d312bf240b7`
1. Your should be prompted to import **Bangazon Python API**.
1. Click the Import button to complete the process.

To test it out, expand the Profile sub-collection, double-click on Login and send the request. You should get a response back that looks like this.

```json
{
    "valid": true,
    "token": "9ba45f09651c5b0c404f37a2d2572c026c146690",
    "id": 5
}
```
