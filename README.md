# py-chat

Chat in Python.
Interops with Rust.

## Setup & Building

```bash
pip3 install componentize-py
git clone https://github.com/hosted-fornet/py-chat.git

cd py-chat/src/
componentize-py -d wit/ -w process componentize lib -o lib.wasm
cp lib.wasm ../pkg/
cd ../
uqdev start-package --url http://localhost:8080
```

## Usage

```
/m our@chat:chat:uqbar {"Send": {"target": "foo.uq", "message": "poggers"}}
```
