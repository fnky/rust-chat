Chat in Rust
============

A scalable chat service using [WebSockets](https://www.websocket.org/), implemented in [Rust](http://rust-lang.org/).

## About

This repository is my personal implementation based on the blog post [Rust in Detail: Writing Scalable Chat Service from Scratch](http://nbaksalyar.github.io/2015/07/10/writing-chat-in-rust.html) by [Nikita Baksalyar](https://github.com/nbaksalyar) ([@nbaksalyar](https://twitter.com/nbaksalyar)).

The purpose is to learn Rust and a bit more about WebSockets. But mostly Rust.

## Usage

Clone the repository

```sh
$ git clone https://github.com/fnky/rust-chat.git
```

Use [Cargo](https://crates.io/) to install dependencies and run the project

```sh
$ cargo run
```
You can connect to the server from the browser using WebSockets

```js
var ws = new WebSocket('ws://127.0.0.1:10000');

if (ws.readyState === WebSocket.OPEN) {
    console.log('Connection is successful');
}
```

> This can be done in the developer tools (`F12`) of your favorite browser.

## Todo

- [ ] Refactor code into multiple files
- [ ] Seperate library code from application
- [ ] Implement secure authentication/authorization
