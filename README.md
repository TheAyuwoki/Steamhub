Installing custom boot animation
#################################
1. copy Steamhubv3.webm to  /home/deck/.local/share/Steam/steamui/movies/ 
2. open terminal inside the folder an run "truncate -s 1840847 Steamhubv3.webm"
3. delete deck_startup.webm and rename Steamhubv3.webm to deck_startup.webm
4. reboot

Getting fullscreen animation
############################
1. Navigate to /home/deck/.local/share/Steam/steamui/css/
2. duplicate library.css
3. open the duplicated library.css with an editor oof your choice 
4. search for video{flex-grow:0;width:300px; height:300px; z-index:10} and change it to 
   video{flex-grow:1;width:100%; height:100%; z-index:10}  
5. save & exit
6. right click on the original library file -> properties and note the file size (for example 1.2MiB 1.234.234) #I dont have my deck here rn why i cant give you the exact file size
7. open terminal inside the folder an run "truncate -s 1.234.234 library.css" #replace 1.234.234 with your noted size
8. delete library.css and rename the duplicated to library.css
9. reboot
