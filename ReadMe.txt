How To Build On WSL:

sudo meson build -D gallium-drivers=freedreno -D vulkan-drivers=freedreno -D tools=freedreno
cd build
sudo ninja -C . install

Then you can use ir3_compiler to compile shaders.