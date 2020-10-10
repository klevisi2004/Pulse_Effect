# Pulse_Effect
#### How to download PulseEffects:
#### A Nice System-Wide PulseAudio Equalizer / Audio Effects App for linux

![capture](https://user-images.githubusercontent.com/62477193/95663492-2827d680-0b2f-11eb-9679-fa108c0243b6.png)

 Follow this steps:
### Warning: if any text has error in installation, just skip it
 
### 1. pactl unload-module module-switch-on-connect                                  

### 2. cp /etc/pulse/default.pa ~/.config/pulse                                     

    3. sed -i 's/load-module module-switch-on-                                       
                                                                                    
    4. connect/#load-module module-switch-on-                                         
                                                                                    
    5. connect/g' ~/.config/pulse/default.pa                                          

### 6. pactl unload-module module-device-manager                                    

### 7. echo "pactl unload-module module-device-manager                             
                                                                                    
    8. > /dev/null 2>&1" >> ~/.bashrc                                                 

### 9. /../src/pulse/operation.c:133, function pa_operation_get_state(). Aborting. 

### 10. dconf reset -f /com/github/wwmm/pulseeffects                                

### 11. flatpak install flathub                                                      
                                                                                   
    12. com.github.wwmm.pulseeffects                                                   

### 13. sudo add-apt-repository                                                      
                                                                                    
    14. ppa:mikhailnov/pulseeffects                                                   
                                                                                    
    15. sudo apt update                                                                                                                                                    
    16. sudo apt install pulseeffects pulseaudio --                                    
                                                                                    
    17. install-recommends                                                             
     
