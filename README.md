command /duyuruyap [<text>]:
    aliases: /dy
    permission: admin.duyuruyap
    trigger:
        if arg 1 is set:
            send " &6[&bDuyuru&6] &7%arg 1%" to all players
        if arg 1 is not set:
            send " &8&l[&eDuyuru&8&l] &4HATA: &cBir mesaj girmediniz!" to player
command /adminchat [<text>]:
    aliases: /ac, /as, /ys
    trigger:
        loop all players:
            if loop-player has the permission "admin.sohbeti":
                send " &8&l[&3&lADMINCHAT&8&l] &a%player%&8> &6%arg 1%" to loop-player
            if arg 1 is not set:
                send " &8&l[&3&lADMINCHAT&8&l] &4&lBir mesaj girmediniz!" to loop-player

