# Dockerfile-Powershell

At work, I'm going to do some work on Windows, which includes building
some software under Jenkins control. At the actual compilation level
tools like CMake and Make are used to control the compilation
process. To execute the nightly compilation jobs under Linux Jenkins
typically some Shell script are used to provide the glue between
Jenkins and the compilation.

The already existing jobs for Windows Jenkins use `cmd.exe` for the
glue scripts between Windows Jenkins and the compilation. `cmd.exe` is
simply to alien to get anything done. Therefore my intention is to use
Powershell for the new glue script I need to created, which I'm
vaguely familar with.

Therefore I had the idea to check out the recently announced multi
platform version of Powershell.

I had some trouble to compile everything required for Powershell on
Arch Linux (all required packages are exist in AUR).

I've build this dockerfile to create a container image with
Powershell. I am very curious if I can build some scripts, which can
easily moved from Linux to Windows.

Zsh is my favoured shell, therefore the docker image is setup to
include `oh-myzsh` for the initialization and customization.

<!--
Local variables:
mode: gfm
End:
-->
