# gl

Experiments - not licensed for reuse (yet)

## Plan

The concept here is a chess GUI of my own design and which I won't detail.

The GUI is built with a game engine (babylon.js is the leading candidate).

The game-engine UI talks to a Web Worker that connects to a local server
using websockets.

The local server is a line-at-a-time HTTP server, which I will probably
write in Golang, for the UCI chess engine control language.

Behind the thin HTTP-to-UCI translater is an instance of Stockfish.

