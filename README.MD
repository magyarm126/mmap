# Zig Maps

## Documentation
https://ziglang.org/

## Build

Build the wasm binary
```
cd src
zig build-exe math.zig -target wasm32-freestanding -fno-entry --export=add
```

Run in node sandbox
```
cd ../node-sandbox
docker compose up -d
docker exec -it node-sandbox bash
node test.js
exit
docker compose down
```