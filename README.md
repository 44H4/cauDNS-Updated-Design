credit to omadaDNS and caub

Works with Securly, GoGuardian, CKAuth, and more!

# How to use
Type this into your url bar:
`data:text/html, <script src='https://caudns.vercel.app/jszip.js' defer></script> <script src='https://caudns.vercel.app/filesaver.js' defer></script> <script src='https://caudns.vercel.app/main.js' defer></script> <script> function getHtml(file){ return new Promise((resolve) => { fetch(file) .then((response) => { return response.text(); }) .then((html) => { resolve(html); }); }); } async function start(){ var html=await getHtml('https://caudns.vercel.app/data.txt'); html=html.toString(); console.log(html); document.body.innerHTML=html; } start(); </script>`

or, just host this repo on any static hosting provider!
