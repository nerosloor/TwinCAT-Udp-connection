# TwinCAT-Udp-connection

Beckhoff / TwinCAT 3 UDP connection

Dieser FB baut eine Socketverbindung mittels des Beckhoff eigenen Sublements "TF6310" auf.
Dabei handelt es sich um einen TCP/IP-Server, der ein entsprechndes Binding vornimmt.
Via UDP können Messages an einen Ziel-Socket versendet werden. 
Und Messages an die erstellte Socketverbindung können empfangen werden.

Benötigte Bibliotheken:
	-> Tc2_TcpIp
	-> Tc2_Utilities
	
Benötigte Lizenzen:
	-> TF6310

Weiteres:
Außerdem wird das Sublement "TF6310-TCP-IP.exe" benötigt.
Dahinter verbirgt sich ein Server, der die Kopplung zu den verwendeten Sockets vornimmt.
Der Server kann von der Beckhoff Seite herunter geladen werden.
Danach sollte der Server auch gestartet werden. Die exe ist zu finden unter "C:\TwinCAT\Functions\TF6310-TCP-IP\Win32\Server"
