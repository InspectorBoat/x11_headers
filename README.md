# x11-headers packaged for the Zig build system

This is a Zig package which provides various X11 headers needed to develop and cross-compile e.g. GLFW applications. It includes development headers for:

* xkbcommon
* x11
* xcb
* xcursor
* xrandr
* xfixes
* xrender
* xinerama
* xi
* xscrnsaver
* xext
* xorgproto
* GLX

This was once maintained by Mach Engine, but was abandoned and moved to a personal repository, which was then deleted. This is a reupload, pulled from https://pkg.machengine.org/x11-headers/29aefb525d5c08b05b0351e34b1623854a138c21.tar.gz and modified to build with latest zig.

## Updating

To update this repository, run `./update.sh` followed by `./verify.sh` to verify the repository contents.

## Verifying repository contents

For supply chain security reasons (e.g. to confirm we made no patches to the code) we provide a `git diff` command you can run to verify the contents of this repository:

```sh
./verify.sh
```

If nothing is printed, there is no diff. Deleted files, and changes to `README.md`, `build.zig`, `.github` CI files and `.gitignore` are ignored.

## Issues

Issues are tracked in the [main Mach repository](https://github.com/hexops/mach/issues?q=is%3Aissue+is%3Aopen+label%3Ax11-headers).
