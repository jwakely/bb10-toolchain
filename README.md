# bb10-toolchain

Work in progress!

You will need the lates BB NDK:
https://developer.blackberry.com/native/downloads/

And the build-essentials (gcc, flex, texinfo, etc...) package for your OS. Use your package manager-

-

The script probably won't be able to create the /opt/qnx800/target/qnx6/usr/ folder structure as a simple user, and you  definetely don't want to run this script as root.
As a workaround you can do the following:

1) open a Terminal
2) sudo mkdir -p /opt/qnx800/target/qnx6/usr/
3) sudo chown -R \`whoami\`:\`whoami\` /opt/qnx800

-

Consult the build.sh file for more information.

Have fun!
