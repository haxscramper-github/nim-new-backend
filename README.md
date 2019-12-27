# Nim New Backend Template

- Template to create a new Backend for Nim, based on the JavaScript Backend.
- As minimalistic as possible to focus on codegen.


# Use

```
$ git clone https://github.com/juancarlospaco/nim-new-backend.git
$ cd nim-new-backend
```

- Hack code.

```console
$ git clone https://github.com/nim-lang/Nim.git
$ cp --verbose --force nim-new-backend/ Nim/
# cd Nim
$ sh ./build_all.sh
$ koch boot
$ echo "echo 42" > hello_world.nim
$ bin/nim js -d:release -d:danger hello_world.nim
```

- Open `hello_world.js`.
- Hack code until you get valid code generated.

```console
$ koch boot
$ bin/nim js -d:release -d:danger hello_world.nim
```

**Optional:**
Rename `hello_world.js` to the proper file extension you are compiling to,
example `mv hello_world.js hello_world.py`.


# FAQ

- Why not use Git SubRepos or Git SubTrees or Git SubModules?.

If you know Git SubRepos and Git SubTrees and Git SubModules,
you wont need this simplified repo.
