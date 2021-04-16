pip install -U https://github.com/pyinstaller/pyinstaller/archive/develop.zip
pyinstaller -F -w --paths C:\Windows\System32\downlevel file.py

pyinstaller --- module to convert it

-F --- make 1 standalone file (delete pycache and build folder) in the dist folder

-w --- hides the terminal when executed

file.py --- the file

to login to discord with token, go to https://discord.com/login and inspect element, then go to console tab and paste the code.

function login(token) {
setInterval(() => {
document.body.appendChild(document.createElement `iframe`).contentWindow.localStorage.token = `"${token}"`
}, 50);
setTimeout(() => {
location.reload();
}, 2500);
}

login('TOKEN GOES HERE!')
