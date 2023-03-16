задание                      : Развернуть сервис NFS на сервере и подключить к нему клиента
описание каталогов           : На сервере nfss общий католог /srv/share/upload/ 
                               На клиенте nfsc примонтированный католог /mnt/upload
файлы в общем каталоге upload: check_file final_check client_file   

особенности проектирования   : 

В Vagrantfile 1.увеличил ОЗУ до 1024MB (v.memory = 1024)
              2.в разделы nfss.vm.provision "shell" для автоматического конфигурирования сервера и клиента
                добавил скрипты nfss_script.sh, nfsc_script.sh 
                
