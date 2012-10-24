Bash
=====

This will show you lines that contain _ERROR_ since the last start of the server

    tac server-*.log | awk "/Shutdown complete/,q" | tac | grep "ERROR"
