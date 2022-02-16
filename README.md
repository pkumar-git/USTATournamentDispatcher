# USTATournamentDispatcher
This UiPath application gets a list of tournaments from the USTA website http://playtennis.usta.com and 
dispatches each tournament URL in the list to the Orchestrator queue "USTATournaments", from where another
application - USTAGetTournamentDetailsFromQueue - retrieves each tournament URL and get details for each
and stores them in an Excel file.
