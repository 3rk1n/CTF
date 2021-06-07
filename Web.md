## Stay Away Creepy Crawlers
Find the flag where they keep the creepy crawlers away.</br>
http://167.71.246.232/</br>
Alternate: http://167.71.246.232:8080/</br>

To find the subdirectory, use ***dirb***</br>
dirb http://167.71.246.232/</br>
http://167.71.246.232/robots.txt

**flag{mr_roboto}**

## Source of All Evil
Find the flag here:</br>
http://167.71.246.232/</br>
Alternate: http://167.71.246.232:8080/</br>

Check out the source code and the flag is in comment line

![image](https://user-images.githubusercontent.com/50519199/120961131-de4acb00-c765-11eb-8df0-34beec1faab9.png)

**flag{best_implants_ever}**

## Can't Find It
Find the flag here:</br>
http://167.71.246.232/</br>
Alternate: http://167.71.246.232:8080/</br>

Check out the source code and there is a subdirectory as ***images***

![image](https://user-images.githubusercontent.com/50519199/120961266-27028400-c766-11eb-9a22-a6ba1309d8ef.png)

http://167.71.246.232/images/ under this directory, we have the list of index for images subdirectory.

![image](https://user-images.githubusercontent.com/50519199/120960978-95931200-c765-11eb-9fba-c2bbc6ef92ca.png)

In this sub-directoy, try to list unlisted subdirectory.</br>
http://167.71.246.232/images/flag

**flag{404_oh_no}**

## Show Me What You Got
Find the "indexes" flag here: http://167.71.246.232/</br>
Alternate: http://167.71.246.232:8080/

We knew that ***images*** subdirectory has two different file.

![image](https://user-images.githubusercontent.com/50519199/120960978-95931200-c765-11eb-9fba-c2bbc6ef92ca.png)

http://167.71.246.232/images/aljdi3sd.txt read the file.

**flag{disable_directory_indexes}**

## Header For You Inspiration
Find the flag here: http://167.71.246.232/</br>
Alternate: http://167.71.246.232:8080/

Send the request to Burp Suite and check out the response.

![image](https://user-images.githubusercontent.com/50519199/120962118-c7a57380-c767-11eb-839a-f7b3cf769cf4.png)

**Alternate:**
Check out the source code and taka a look **Header**

![image](https://user-images.githubusercontent.com/50519199/120962344-397dbd00-c768-11eb-99a8-4fcd7cd83b99.png)

**flag{headersftw}**

## Ripper Doc
Find the flag in the ripper doc list.</br>
http://167.71.246.232/</br>
Alternate: http://167.71.246.232:8080/

http://167.71.246.232:8080/certified_rippers.php check out this directory.

![image](https://user-images.githubusercontent.com/50519199/120962550-9f6a4480-c768-11eb-9a00-a5d5eafd4582.png)

Send the request to Burp Suite.</br>
There is ``Cookie: authenticated=false`` change it ``Cookie: authenticated=true``

![image](https://user-images.githubusercontent.com/50519199/120962470-79dd3b00-c768-11eb-8814-1031378d7189.png)

**flag{messing_with_cookies}**
