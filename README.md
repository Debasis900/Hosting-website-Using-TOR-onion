# Hosting-a-website-with-TOR

- Install tor in your Linux machine.
- Make a directory and cd into that directory.
- Then Edit torrc file present in /etc/tor/.
- Uncomment the lines which says *HiddenServiceDir* and *HiddenServicePort*.
- Then Change the port address from 80 to 8080 as we are hosting a HTML website.
- After that save the file.
- Then type *python3 -m http.server --bind 127.0.0.1 8080*.
- After this run tor as sudo.
- Once the service is started cd into the *HiddenServiceDir* inside that directory you will see a file name *hostname*.
- Copy that .onion link and your are ready to go.
