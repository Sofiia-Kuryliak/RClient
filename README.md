# Client RMI (Course Work)

CClient is a chat client with simple UI, that can send and receive messages of a certain type (texts or files) from the server. 
In this case for sending and receiving message used RMI - method of communication for building distributed systems.

Command Name |Structure of the command|Example|
-------------|------------------------|-------|
Ping|#ping: <br> #p|#p|
Echo|#ec: ; <br> #echo: ; <br> #ec: (some text); <br> #echo: (some text);|#ec: hello;|
Generation random file|#g: p-(URL dir to gen.) n-(name gen. file); <br> #generation: path-(URL dir to gen.) nameFile-(name gen. file);| #g: p-F:\TestSort n-rand.txt;|
Process|#pr: r-(URL dir with name randomFile) s-(URL dir with name sortFile); <br> #process: randomFile-(URL dir with name randomFile) sortFile-(URL dir with name sortFile);| #pr: r-F:\TestSort\rand.txt s-F:\TestSort\sort.txt;|
