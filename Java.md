Java
=====

Explode a War file

    WAR=<file>.war; mv $WAR $WAR.bak && mkdir $WAR && cd $WAR && cp ../$WAR.bak . && unzip $WAR.bak && rm -f $WAR.bak
