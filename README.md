# learn-ziglang

## Install ziglang compiler

```
$ zig_version=0.7.1

$ sudo apt install xz-utils

$ cd ~/Downloads
$ curl -LO https://github.com/ziglang/zig/releases/download/${zig_version}/zig-linux-x86_64-${zig_version}.tar.xz

$ sudo tar -C /usr/local -xf zig-linux-x86_64-${zig_version}.tar.xz
$ sudo mv /usr/local/zig-linux-x86_64-${zig_version} /usr/local/zig
$ sudo chown -R $(id -u):$(id -g) /usr/local/zig
$ rm zig-linux-x86_64-${zig_version}.tar.xz

$ nano ~/.bashrc
export PATH=/usr/local/zig:$PATH
$ source ~/.bashrc
$ zig version
```
