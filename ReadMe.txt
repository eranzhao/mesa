How To Build On WSL:

sudo apt install bison byacc clang cmake flex gzip libdrm-amdgpu1 libdrm-dev libdrm-intel1 libwayland-dev libwayland-egl-backend-dev libwrap0 libx11-dev libx11-xcb-dev libxcb-dri2-0-dev libxcb-dri3-dev libxcb-glx0-dev libxcb-present-dev libxcb-shm0-dev libxext-dev libxfixes-dev libxrandr-dev libxshmfence-dev libxxf86vm-dev llvm-dev meson ninja-build pkg-config python3 wayland-protocols wsl-setup x11proto-xext-dev

sudo pip3 install mako

sudo meson build -D gallium-drivers=freedreno -D vulkan-drivers=freedreno -D tools=freedreno
cd build
sudo ninja -C . install

Then you can use ir3_compiler to compile shaders.
