# PWA to encrypt and decrypt text

![R2P in action](https://raw.githubusercontent.com/saldoukhov/media/main/r2p/r2p_demo.gif)

This is a very simple progressive web app that has zero dependencies and is easy to audit.
The goal is to give the user a tool to encrypt or decrypt textual data, that can be sent or stored separately.

Remember that for decryption you need to know the passphrase used to encrypt the text.

Do not store the passphrase next to the encrypted text.

For sensitive data use longer passphrase (random password 18+characters of 6+ words).

When you type the passphrase, the app gives you three words which are the "fingerprint" of the passphrase.
The "fingerprint" is useful to make sure you typed the right passphrase without revealing the passphrase. 
Also, if you store the fingerprint next to the encrypted text it will help you remember the passphrase you used.
It is impossible to reconstruct the passphrase from the fingerprint.

Split and join give you the possibility to protect your data (encrypted or unencrypted) 
by splitting it into 2 pieces that should be stored separately.

---
To install, you need to serve the app. 
Download the code, serve it locally with some static server (f.e. https://github.com/http-party/http-server)
then make it public on the internet (f.e. https://ngrok.com), access the url, 
install the app (f.e. on phone add it from browser to desktop). 
Then you can stop ngrok and your local server, app will still be available.

You can also use or install the app from the page published by this repository https://saldoukhov.github.io/r2p
but in this case you take the risk of the code being changed in the background without you noticing.
Also, if this repository goes down, and you lose the device with this app installed, 
you will have hard time decrypting your secrets. 
So the best practice would be to store this code in your own domain.
