[Based on](https://agniva.me/wasm/2018/05/17/wasm-hard-way.html)

- [0](https://danieloskarsson.github.io/wasm-minimal/level0/hello.html): `emcc hello.c -o hello.js`
- [1](https://danieloskarsson.github.io/wasm-minimal/level1/hello.html): `emcc hello.c -o hello.wasm -Os -s SIDE_MODULE=1`
- [2](https://danieloskarsson.github.io/wasm-minimal/level2/hello.html): `emcc hello.c -o hello.wasm -Os`
- [3](https://danieloskarsson.github.io/wasm-minimal/level3/hello.html): `wat2wasm hello.wat`
- [4](https://danieloskarsson.github.io/wasm-minimal/level4/hello.html): `emcc hello.c -o hello.wasm -Os && emcc hello.c -Os -Wseparate-asm -s WASM=0 -o hello.asm.js`

Serve with `emrun --no_browser --port 8000 .`

[Also visit](https://gist.github.com/kripken/59c67556dc03bb6d57052fedef1e61ab)