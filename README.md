# kernel
64-bit OS Kernel

prints OK for now

still in 32 bit need to change to 64 bit

developed in windows10 <br />
steps: <br />
.install docker<br />
  .should be running in linux containers<br />
.install qemu<br />
  .create PATH variable for qemu<br />
.open the project in vs code<br />
.give the command to create the docker img 'docker build buildenv -t <tag_name_for_ur_virtual_env>'<br />
. in terminal give the command 'docker run --rm -it -v "$(pwd):/root/env" <tag_name_for_ur_virtual_env>'<br />
.inside the shell give make command to build the iso file<br />
  .make build-x86_64<br />
.exit the shell<br />
.in therminal give the command 'qemu-system-x86_64 -cdrom dist/x86_64/kernel.iso' to see the output<br />
