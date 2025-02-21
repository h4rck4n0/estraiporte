# estraiporte
estrae le porte trovate da nmap
esempio:
nmap <IP> -p- --open  -sS -min-rate 5000 -vvv-oG <porte>
nmap crea un file "porte" greppeabile (-oG) dove inserirà le porte trovate

Con 

estraiporte ti memorizza le porte nella clipboard, quindi con i 
tasti ctrl+shift+v ti incolla le porte

	estraiporte <nomefile>
 
 esempio:

 	estraiporte porte

Estrazione informazioni...

Indirizzo IP: <IP>
Porte aperte: 22,80

Porte copiate nel clipboard (ctrl+shift+v)

Quindi eseguendo un'altra scansione "22,80" sarà possibile incollarlo nel comando

nmap <IP> -p <qui premi i tasti ctrl+shift+v> -sCV ----> nmap <IP> -p 22,80 -sCV

Questo comando è utile quando nmap trova molte porte, così ci evita di scrivere a mano tutte le porte.


