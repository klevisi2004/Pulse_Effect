# Pulse_Effect
#### How to download PulseEffects:
#### A Nice System-Wide PulseAudio Equalizer / Audio Effects App for linux

![capture](https://user-images.githubusercontent.com/62477193/95663492-2827d680-0b2f-11eb-9679-fa108c0243b6.png)

 Follow this steps:
 
-------------------------------------------------------------------------------------
 ### 1. pactl unload-module module-switch-on-connect                                 | 
|------------------------------------------------------------------------------------|
 ### 2. cp /etc/pulse/default.pa ~/.config/pulse                                     |
|                                                                                    |
|     sed -i 's/load-module module-switch-on-                                        |
|                                                                                    |
|     connect/#load-module module-switch-on-                                         |
|                                                                                    |
|     connect/g' ~/.config/pulse/default.pa                                          |
|------------------------------------------------------------------------------------|
 ### 3. pactl unload-module module-device-manager                                    |
|------------------------------------------------------------------------------------|
 ### 4. echo "pactl unload-module module-device-manager                              |
|                                                                                    |
|     > /dev/null 2>&1" >> ~/.bashrc                                                 |
|------------------------------------------------------------------------------------|
  ### 5. /../src/pulse/operation.c:133, function pa_operation_get_state(). Aborting. |
|------------------------------------------------------------------------------------|
  ### 6. dconf reset -f /com/github/wwmm/pulseeffects                                |
|------------------------------------------------------------------------------------|
 ### 7. flatpak install flathub                                                      |
|                                                                                    |
|     com.github.wwmm.pulseeffects                                                   |
|------------------------------------------------------------------------------------|
 ### 8. sudo add-apt-repository                                                      |
|                                                                                    |
|     ppa:mikhailnov/pulseeffects                                                    |
|                                                                                    |
|     sudo apt update                                                                |
|                                                                                    |
|     sudo apt install pulseeffects pulseaudio --                                    |
|                                                                                    |
|     install-recommends                                                             |
'_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_'

