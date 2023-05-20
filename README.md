# Yahoo Account Checker
base on https://github.com/TufayelLUS/Yahoo-Account-Checker, replace requests with playwright
exe is larger because of contains chrome

## install deps
```shell
pip install -r .\requirements.txt
```
## gen exe (powershell [ref](https://playwright.dev/python/docs/library#pyinstaller))
```shell
pip install -U pyinstaller
$env:PLAYWRIGHT_BROWSERS_PATH="0"
playwright install chromium
pyinstaller -F yahoo_checker.py
```
