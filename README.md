# About

A small utility program I wrote to manage lightning address payments to my node.

# Setup

1. Create a application macaroon
```shell
lnd $ lnd-cli bakemacaroon invoices:read invoices:write address:read address:write --save_to ./app.macaroon
```
2. Create a python virtual env
```shell
lnd $ python3 -m venv .env
```

3. Source the environment
```shell
lnd $ source .env/bin/activate
```

4. Install dependencies
```shell
lnd $ pip install -r requirements.txt
```

5. Run the server
```shell
lnd $ ./lnurl --server
```
