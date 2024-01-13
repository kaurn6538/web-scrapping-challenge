# Instructions for creating the PATH for getting chromedriver to work

## Example executable path and browser variables for MAC

executable_path = {'executable_path': '/usr/local/bin/chromedriver'}
browser = Browser('chrome', **executable_path)

## Windows Download and Path Instructions

1. Download ChromeDriver:
2. You can download the appropriate version of ChromeDriver from here. Make sure that the version of ChromeDriver you download corresponds to the version of Chrome installed on your machine.
3. Place ChromeDriver in a Recognized Location:
4. You have several options here:
    Place the chromedriver.exe file in a directory that's already in your system's PATH, such as C:\Windows\System32.
    Add the directory containing chromedriver.exe to your system's PATH.
    Specify the path to ChromeDriver directly in your code.
5. Specifying the Path in Your Code:
6. If you want to specify the path directly in your code without modifying the system's PATH, you can do so by providing the path to the chromedriver.exe file when initializing your browser.
7. Here's an example:
8. from splinter import Browser executable_path = {'executable_path': 'C:\path\to\chromedriver.exe'} browser = Browser('chrome', **executable_path)
9. Replace C:\path\to\chromedriver.exe with the actual path to the chromedriver.exe file on your machine.
Now, when you run your code, it should be able to find ChromeDriver and you shouldn't see the error message.

*     chromedriver.chromium.orgchromedriver.chromium.org
*     ChromeDriver - WebDriver for Chrome - Downloads

*     Current Releases
*     If you are using Chrome version 115 or newer, please consult the Chrome for Testing availability dashboard. This page provides convenient JSON endpoints for specific ChromeDriver version downloading.
## Example executable path for Windows

* executable_path = {'executable_path': 'J:\UNC Bootcamp\Chrome Driver\chromedriver-win64\chromedriver.exe'}
browser = Browser('chrome', **executable_path)
* REMINDER: with Windows you may have to use the \ in place of your \ in your executable_path.
