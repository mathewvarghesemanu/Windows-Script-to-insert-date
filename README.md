# Creating a script to insert the current date with autohotkey in windows

1. Visit https://www.autohotkey.com/ and download the software.

2. Express install autohotkey

3. Right click on desktop and select New>Autohotkey script

4. Rename it as insert_date.ahk

5. Remove the text already in the file and type in the below code


`^!d::
     FormatTime, CurrentDateTime,, dd/MM/yyyy
     SendInput, %CurrentDateTime%
Return
`

6. Save the file and double click on it to open this script in autohotkey. It’ll run in the background.

7. With the service running in the background, whenever you press Ctrl+Alt+D, the current date will be input in DD-MM-YY format
