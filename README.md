# using-macos
Error:
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun

Solution:
xcode-select --install

Error: 
Warning: /usr/local/Frameworks isn't writable.

This can happen if you "sudo make install" software that isn't managed by
by Homebrew. If a formula tries to write a file to this directory, the
install will fail during the link step.


Solution:
chown -R `whoami` /usr/local/*

