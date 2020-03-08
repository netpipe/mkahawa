# mkahawa
Cyber Cafe Management App

use certificates.sh in the src directory to generate certificates


https://sourceforge.net/p/mkahawa/discussion/955736/thread/1619a50f/
Simplest answer:
-> Start mkahawa (server) with -nossl (/usr/bin/mkahawa -nossl) - I normally create a desktop launcher with this command

Simple answer:
-> Try putting the .pem file in / directory. ( sudo cp cert.pem / ) - This will require that you go to every client machine and install the .pem.

Complicated answer:
- start mkahawa-client  with -dir /home/.mkahawa (or any preferred directory ) option.
- ensure that only root can access /home/.mkahawa directory (sudo chmod 700 /home/.mkahawa )
- copy .pem files to /home/.mkahawa 



