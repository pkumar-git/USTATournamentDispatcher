# USTATournamentDispatcher
This UiPath application gets a list of tournaments from the USTA website http://playtennis.usta.com and 
dispatches each tournament URL in the list to the Orchestrator queue "USTATournaments", from where another
application - USTAGetTournamentDetailsFromQueue - retrieves each tournament URL and get details for each
and stores them in an Excel file.


Currently it retrieves only junior tournaments for the "18 and under" age division, though it is a straightforward 
change to retrieve any other/all age divisions.  It also retrieves all levels of tournaments, and again, it is a 
straightfoward change to retrieve only certain levels of tournaments.  Only tournaments whose registration status
is open are retrieved.

It requires the latest USTALibrary package to be available. It uses Chrome browser to access the USTA website.
