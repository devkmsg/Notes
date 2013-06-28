# Bash

This will show you lines that contain _ERROR_ since the last start of the server

    tac server-*.log | awk "/Shutdown complete/,q" | tac | grep "ERROR"


The will show you a long file listing ordered by time with the oldest on the bottom - this is useful if you have a directory with a very large number of files

    ls -latr
