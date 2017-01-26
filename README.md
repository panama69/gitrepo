# gitrepo

 
To start the container (we will add the network flag so other container can access to such as Jenkins)
                docker run -d -p 2222:22 --name gitRepoServer panama69/gitrepo
The do the following from Windows or Ubuntu which has git installed
                git clone ssh://root@<docker server ip/hostname>:2222/opt/gitrepo/deleteme
                cd deleteme
                git checkout message.txt (and add/delete something from the file)
                git commit message.txt –m “Hg Se”
                git push
 
Your first time you will see something like this:
c:\Temp\flynn>git clone ssh://192.168.28.130:2222/opt/gitrepo/deleteme
Cloning into 'deleteme'...
The authenticity of host '[192.168.28.130]:2222 ([192.168.28.130]:2222)' can't be established.
ECDSA key fingerprint is 28:02:43:fd:c8:29:5e:92:a6:84:e0:97:3d:7b:60:c1.
Are you sure you want to continue connecting (yes/no)? yes
This is ok.

The password is hpe
