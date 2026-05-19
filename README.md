# Final-project
# 1. Program Overview
This is Stonks! Stonks is a Java-centered program in for people who are just beginning stocks and want a simple navigation system. 

This program is useful because for people who are just getting into stock trading, many applications are extremely confusing and have a high learning curve before using it. Through Stonks, we bypass this issue with a simple user interface. 

# 2. Feature List
Overall, we were able to achieve many of the core goals we had in mind. Here are a few of the large features of Stonks:

- Add and remove any valid stocks to a personal list
- Live price changes over time
- Save function to keep stocks chosen in previous sessions
- Input lower/upper bounds to alert user if their stock has changed price

There were a few changes we had to make due to complexity and time constraints. When we decided to switch from a GUI to running through terminal, we took out the ability to toggle between light and dark mode. Similarly, we could not implement interactive buttons, but we used the switch function to have the user choose their actions. We also decided to omit the filter system due to prioritizing our time towards making a more quality interface.

# 3. Known Bugs / Limitations
Due to using a free API key, there was a limitation we faced while coding. First, the API allowed a limited number of data calls a day, restricting how many times we could test our code out. This would make it look like our code was not functioning well even though it worked as intended. Also we originally had a plan of including some sort of visualization through a graph. Unfortunately we could not get enough data points because of the API limit and it would be more complicated to include visualizations in the terminal. We realize the data visualization was one of the biggest topics we wanted to implement in our program, so instead we worked more on formatting the terminal outputs through text and design.

# 4. Step-By-Step User Guide

- Launching the program:
    - Type in terminal: javac Main.java.   --> java Main
    - Or you can use the run button provided at the top of the application.
- Interacting with the terminal:
    - Input a number on the keyboard corresponding with the action.
- What each option does/means:
    - "1" will output the stocks the user has chosen in a formatted text. It will display the current price of the stock, high and low prices, as well as the overall change in price. 
        ![alt text](image.png) 
    This is what the formatted output looks like. There is a N/A because the API has ran out of times to retrieve data for the day.
    - "2" will output a textbox to prompt the user to type a valid stock to track. The user can add multiple by separating them with a comma.
    - "3" allows the user to remove a stock in their personal portfolio by inputting the stock name in the textbox.
    - "4" will prompt the user with three textboxes to choose a stock to set a lower bound and an upper price bound to track the stock. If the stock price goes 
    outside of this range, the program will tell the user.
    - "5" allows the user to check if there are any drastic price changes that have gone outside of the lower and upper bounds set.
    - "6" allows the user to save the changes they made in their portfolio in a local file. This ensures they can continue their session into the follow time.
    - "7" displays a formatted response showing the history of all of the actions the user made since the beginning of the session. It displays what action they made as well as the time they did it.
    ![alt text](image-1.png)
    This is what the formatted response looks like
    - "8" allows the user to refresh all of the stocks in the personal portfolio. This allows the user to get the most recent prices, but it contributes to the daily usage limit.
    - "9" displays the status of the cache that has accumulated over program usage. 
    - "10" allows the user to safely exit the program.
