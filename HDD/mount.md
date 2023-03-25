mount -t cifs -o username=alexey.ilin //kcell.kz/dfs/Workfiles/B2C/ /mnt/test2

mount -t cifs //vkc-ekps01/c$/Program\ Files/eKassir/PaySystem\ Server/logs -o soft,username=Admin,password=Aa12345678 /mnt/qwe

mount -t cifs //vkc-ekps01/c$/Program\ Files/eKassir/PaySystem\ Server/logs -o vers=3.0,username=Admin,password=Aa12345678,dir_mode=0777,file_mode=0777,serverino,sec=ntlmssp /mnt/qwe



mount -t smbfs //alexey.ilin:Zander123$@media/Stars_of_KCELL /mnt/test


mount -t cifs //alexey.ilin:Zander123$@media/Stars_of_KCELL /mnt/test


mount -t cifs -o username=alexey.ilin //media/Stars_of_KCELL /mnt/win_share


mount -t cifs -o username=alexey.ilin //media/Stars_of_KCELL /mnt/test
