### Vorbereitung
- Schauen, ob Präsentation noch da ist
    - Server starten
    - my_device über Device Manager starten und App öffnen
    - my_device_1 über Debugger starten
    - Emulatoren verstecken
### Server
- MafiaShared
    - .NET Standard Library
    - Über diese Klassen wird der Datenaustausch stattfinden
- AspMafiaServer
    - Startup
        - ConfigureServices
            - SignalR Service wird hinzugefügt
		- Configure
			- Hub wird hinzugefügt
    - ChatHub
        - Erfüllt die .NET Core API
        - Kurz Mehtoden druchgehen
    - applicationhost.config zeigen
		- "C:\Dev\Git\Mafia-project\AspMafiaServerSolution\.vs\config\applicationhost.config" öffnen
		- Nach 127.0.0.1 suchen
### Client
- ChatViewModel
    - OnInitialize
        - _connection.On
            - ChatMessageExtensions
    - ChangeGroup
        - JoinGroup
        - LeaveGroup
    - SendMessageToGroup
## LiveDemo !!!