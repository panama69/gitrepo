# gitrepo

 
To start the container (we will add the network flag so other container can access to such as Jenkins)<br>
                docker run -d -p 2222:22 --name gitRepoServer panama69/gitrepo<br>
The do the following from Windows or Ubuntu which has git installed<br>
                git clone ssh://root@<docker server ip/hostname>:2222/opt/gitrepo/deleteme<br>
                cd deleteme<br>
                git checkout message.txt (and add/delete something from the file)<br>
                git commit message.txt –m “Hg Se”<br>
                git push<br>
 
Your first time you will see something like this:<br>
c:\Temp\flynn>git clone ssh://192.168.28.130:2222/opt/gitrepo/deleteme<br>
Cloning into 'deleteme'...<br>
The authenticity of host '[192.168.28.130]:2222 ([192.168.28.130]:2222)' can't be established.<br>
ECDSA key fingerprint is 28:02:43:fd:c8:29:5e:92:a6:84:e0:97:3d:7b:60:c1.<br>
Are you sure you want to continue connecting (yes/no)? yes<br>
This is ok.<br>
<br>
The password is hpe
