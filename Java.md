# Java

Explode a War file

    WAR=<file>.war; mv $WAR $WAR.bak && mkdir $WAR && cd $WAR && cp ../$WAR.bak . && unzip $WAR.bak && rm -f $WAR.bak
    
Add GC Logging

    -verbose:gc -Xloggc:<log dir>/gc.log.<app name>.`date +%Y%M%d%H%M%S` -XX:+PrintGCDateStamps -XX:+PrintGCDetails
    
Core Dump

    jmap -dump:format=b,file=/tmp/filename <pid>
