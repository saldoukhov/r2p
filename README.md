# PWA to encrypt and decrypt text

This is a very simple progressive web app that has zero dependencies and is easy to audit.
The goal is to give the user a tool to encrypt or decrypt textual data, that can be sent or stored separately

Remember that for decryption you need to know the passphrase used to encrypt the text

Do not store the passphrase next to the encrypted text

For sensitive data use longer passphrase (random password 18+characters of 6+ words)

When you type the passphrase, the app gives you three words which are the "fingerprint" of the passphrase.
The "fingerprint" is useful to make sure you typed the right passphrase without revealing the passphrase. 
Also, if you store the fingerprint next to the encrypted text it will help you remember the passphrase you used.
It is impossible to reconstruct the passphrase from the fingerprint. 

---
To install, you need to serve the app. 
Serve it locally with some static server (f.e. https://github.com/http-party/http-server)
then make it public on the internet (f.e. https://ngrok.com), access the url, 
install the APP (f.e. on phone add it from browser to desktop). 
Then you can stop ngrok and your local server, app will still be available.