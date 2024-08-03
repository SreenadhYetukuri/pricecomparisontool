This Python code implements a simple price comparison tool with a graphical user interface (GUI) using Tkinter. Here's a breakdown of its functionality:

### Imports:

**1.tkinter**: Python's standard GUI (Graphical User Interface) library.</br>
**2.requests**: Library for making HTTP requests.</br>
**3.time**: Provides various time-related functions.</br>
**4.sqlite3**: Library for SQLite database operations.</br>


## Database Setup:

1.Establishes a connection to an SQLite database named price_data.db.</br>
2.Creates a table named prices if it doesn't exist, with columns for the product name, Amazon price, and Google price.</br>


## Database Functions:

insert_into_db: Inserts data into the SQLite database table.


### Search Functionality:

1.search: Gets the product name from the entry widget.</br>
2.Sends requests to a price comparison API (price-analytics.p.rapidapi.com) for Amazon and Google prices.</br>
3.Polls the API to get the results after a delay (120 seconds in this case).</br>
4.Updates the GUI labels with the retrieved Amazon and Google prices.</br>
5.Inserts the product name, Amazon price, and Google price into the SQLite database.</br>
6.Graphical User Interface (GUI):</br>

Creates a Tkinter window titled "Price Comparison".
Includes labels and an entry field for entering the product name.
Provides a "Search" button to trigger the search functionality.
Displays labels for showing the Amazon and Google prices.


## Main Loop:

Starts the Tkinter event loop to run the GUI application.


## Database Connection Closing:

Closes the connection to the SQLite database when the Tkinter event loop exits.
This code can be useful for users to quickly compare prices of a product on Amazon and Google within the specified country (in this case, India) and store the results for future reference. It provides a simple interface for conducting price comparisons efficiently.
![Screenshot (182)](https://github.com/Afzal4984/pricecomparisontool/assets/126193636/99e9a098-defe-414c-a6e7-edf6203f1fa6)
![Screenshot (184)](https://github.com/Afzal4984/pricecomparisontool/assets/126193636/9c5f8397-bec4-415b-bcb6-5d02786d78b9)





