# Elevens-Lab-Activity7

1. What items would be necessary if you were playing a game of Elevens at your desk (not on the
computer)? List the private instance variables needed for the ElevensBoard class.
    All you need is cards
    Private cards
    Private values


2. Write an algorithm that describes the actions necessary to play the Elevens game.
	make a deck
        shuffle
	if(value1+ value2 == 11) then replace and deal 2x
	else if ( value1+value2+value3 =0) then replace and deal 3x
	else don't replace

3. Now examine the partially implemented ElevensBoard.java file found in the Activity7
Starter Code directory. Does the ElevensBoard class contain all the state and behavior
necessary to play the game?
	No it is missing methods like checking for pairs and seeing if another play is possible and checking the players move

4. ElevensBoard.java contains three helper methods. These helper methods are private
because they are only called from the ElevensBoard class.

a. Where is the dealMyCards method called in ElevensBoard?

When the board is created and when a new game is started




b. Which public methods should call the containsPairSum11 and containsJQK
methods?

Is legal and anotherPlayIsPossible.




c. It’s important to understand how the cardIndexes method works, and how the list that it
returns is used. Suppose that cards contains the elements shown below. Trace the execution
of the cardIndexes method to determine what list will be returned. Complete the diagram
below by filling in the elements of the returned list, and by showing how those values index
cards. Note that the returned list may have less than 9 elements.

![My image](https://bsimps3.github.io/Elevens-Lab-Activity7/cards.png)

0/6/2/1/4

d. Complete the following printCards method to print all of the elements of cards that are
indexed by cIndexes.
    public static printCards(ElevensBoard board) {
    List<Integer> cIndexes = board.cardIndexes();
    System.out.println(cIndexes);         
  
  
  
  
  
  
  
    }
  
  
  e. Which one of the methods that you identified in question 4b above needs to call the
      cardIndexes method before calling the containsPairSum11 and containsJQK
      methods? Why?
 anotherPlayIsPossible because the cards on the board need to be checked for possible sums and the null cards need to be removed for the other methods to work.
