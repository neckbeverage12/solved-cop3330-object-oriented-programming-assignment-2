Download Link: https://assignmentchef.com/product/solved-cop3330-object-oriented-programming-assignment-2
<br>
<strong>Assignment Scope</strong>

<ol>

 <li>Add member variables to classes</li>

 <li>Generate getters/setters for member variables</li>

 <li>Write custom constructors</li>

 <li>Add method signatures to an interface</li>

 <li>Implement an interface so that methods are declared as abstract</li>

 <li>Implement abstract methods in inherited classes</li>

 <li>Write methods to accomplish specific tasks for a class</li>

 <li>Create enumerations as constants</li>

 <li>Compile and run a project</li>

 <li>Compress a project and submit to Webcourses</li>

 <li>Decompress compressed project and verify it is a Netbeans project</li>

</ol>




<strong>References</strong>

<ol>

 <li>docx</li>

 <li>Setting up a project in Netbeans.docx</li>

 <li>Netbeans right click menu help.docx</li>

</ol>

<strong> </strong>

<strong>Deliverables</strong>

To complete this assignment you must submit your <strong>compressed Netbeans project </strong>to Webcourses.

<strong> </strong>

<strong>Tasks</strong>

<table width="667">

 <tbody>

  <tr>

   <td colspan="2" width="667"><strong>Activity</strong></td>

  </tr>

  <tr>

   <td width="181"><strong>Euchre project</strong></td>

   <td width="486">Create a new Java Application project named Euchreallowing Netbeans IDE to create the main class called Euchre.java</td>

  </tr>

  <tr>

   <td width="181"><strong>Euchre class</strong></td>

   <td width="486">Update main() method to do the following:1.      Instantiate an instance of class Game calling the no-argument constructor</td>

  </tr>

  <tr>

   <td width="181"><strong>constants</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Constants class</strong></td>

   <td width="486">Add the following:1.      A constant for the number of AI players set to the value of 32.      A constant for the number of cards in a Euchre deck set to the value of 243.      A constant for the number of cards each player is dealt set to the value of 54.      A constant for the number of rounds in a hand set to the value of 55.      An enumeration for the color of cards so it includes: RED and BLACK6.      An enumeration for the suit of cards so it includes: CLUBS, DIAMONDS, HEARTS, SPADES7.      An enumeration for the face value of cards so it includes: NINE, TEN, JACK, QUEEN, KING, ACE</td>

  </tr>

  <tr>

   <td width="181"><strong>core package</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>AiPlayer class</strong></td>

   <td width="486">Implement methods inherited from class Player:1.      public Card playCard();2.      public int makeTrump();</td>

  </tr>

  <tr>

   <td width="181"><strong>Card class</strong></td>

   <td width="486">1.      Add member variables (Hint: you will have to explicitly import each enumeration, example: import constants.Constants.Color; ):a.       Data type enumeration Face to represent the face value of the cardb.      Data type enumeration Suit to represent the suit of the cardc.       Data type enumeration Color to represent the color of the card2.      Generate getters/setters for member variables</td>

  </tr>

  <tr>

   <td width="181"><strong>Deck class</strong></td>

   <td width="486">1.      Add member variablea.       Data type Set&lt;Card&gt; to represent the deck of cards2.      Generate getter/setter for member variables</td>

  </tr>

  <tr>

   <td width="181"><strong>Game class</strong></td>

   <td width="486">1.      Add member variablesa.       Data type enumeration Suit to represent the trump suite of Euchreb.      Data type class Player to represent the lead player for each handc.       Data type class Player to represent the dealer for each handd.      Data type class Player to represent which player won the current trick/hande.       Data type int to represent the current round of the gamef.        Data type ArrayList&lt;Team&gt; to represent the two teams of the gameg.      Data type class Deck to represent the deck of cards for the gameh.      Data class Scanner to get information from the user2.      Generate getters/setters for the member variables3.      Write a custom constructor thata.       Has no parametersb.      Calls method createTeams() which will be defined within this classc.       Calls method outputTeams() which will be defined within this class4.      Write method createTeams() thata.       Has no parametersb.      Has return type voidc.       Instantiate the member variable of type ArrayList&lt;Team&gt;d.      Instantiates two instances of class Teami.      one for TeamOneii.      one for TeamTwoiii.      set names for each team as appropriateiv.      add each instance to the ArrayList&lt;Team&gt; member variablee.       Instantiate the member variable of class Scanner passing “System.in” as the argument to the constructorf.        Using System.out.println() static method, prompt the user for the human player’s nameg.      Instantiate an instance of class String set equal to the reference object of class Scanner using its method .next()h.      Instantiate an instance of class HumanPlayeri.        Call method .setName() on the reference object of class HumanPlayer passing the value stored in the variable from step g. abovej.        Add the reference object of class HumanPlayer to the instance of class Team representing Team Onek.      Write a for loop to generate three AiPlayer instancesi.      Generate a unique name for each AiPlayer and call method .setName() passing the unique name as an argumentii.      Add one AiPlayer instance to the instance of class Team representing Team Oneiii.      Add the other two AiPlayer instances to the instance of class Team representing Team Two5.      Write method outputTeams() so thata.       It has no parametersb.      Has a return type of voidc.       Uses an enhanced for loop to loop through the collection of member variable of type ArrayList&lt;Team&gt;1.      Calls method outputTeam() in class Team</td>

  </tr>

  <tr>

   <td width="181"><strong>HumanPlayer class</strong></td>

   <td width="486">Implement methods inherited from class Player:1.      public Card playCard();2.      public int makeTrump();</td>

  </tr>

  <tr>

   <td width="181"><strong>IPlayer interface</strong></td>

   <td width="486">Add method signatures:1.      public Card playCard();2.      public void makeTrump();</td>

  </tr>

  <tr>

   <td width="181"><strong>Player class</strong></td>

   <td width="486">1.      Add member variables:a.       Data type String to represent player name2.      Generate getters/setters for the member variables3.      Declare abstract the methods inherited from interface IPlayera.           public abstract Card playCard();b.          public abstract int makeTrump();</td>

  </tr>

  <tr>

   <td width="181"><strong>Team class</strong></td>

   <td width="486">1.      Add member variablesa.       Data type ArrayList&lt;Player&gt; to represent a teamb.      Data type int to represent the team’s scorec.       Data type int to represent the team’s tricks taken for each handd.      Data type String to represent the team’s name2.      Generate getters/setters for the member variables3.      Write a custom constructor that instantiates the member variable ArrayList&lt;Player&gt;4.      Write method outputTeams() so thata.       It has no parametersb.      Has a return type of voidc.       Outputs the current Team’s named.      Uses an enhanced for loop to loop through the collection of class Team’s member variable ArrayList&lt;Player&gt;i.      Outputs the current Player’s name</td>

  </tr>

  <tr>

   <td width="181"><strong>userinterface package</strong></td>

   <td width="486"> Create package userinterface</td>

  </tr>

  <tr>

   <td width="181"><strong>Euchre application</strong></td>

   <td width="486"> </td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 1</strong></td>

   <td width="486">Test Case 1 passes</td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 2</strong></td>

   <td width="486">Test Case 2 passes</td>

  </tr>

  <tr>

   <td width="181"><strong>Test Case 3</strong></td>

   <td width="486">Test Case 3 passes</td>

  </tr>

  <tr>

   <td width="181"><strong> </strong></td>

   <td width="486">Source compiles with no errors</td>

  </tr>

  <tr>

   <td width="181"><strong> </strong></td>

   <td width="486">Source runs with no errors</td>

  </tr>

  <tr>

   <td width="181"><strong> </strong></td>

   <td width="486">Source includes comments</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong>Perform the following test cases</strong>

<table>

 <tbody>

  <tr>

   <td colspan="3" width="638"><strong>Test Cases</strong></td>

  </tr>

  <tr>

   <td width="166"><strong> </strong></td>

   <td width="166"><strong>Action</strong></td>

   <td width="307"><strong>Expected outcome</strong></td>

  </tr>

  <tr>

   <td width="166"><strong>Test Case 1</strong></td>

   <td width="166"><strong>Project view</strong></td>

   <td width="307">Completed project view should look like figure 1</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 2</strong></td>

   <td width="166"><strong>Run application</strong></td>

   <td width="307">The console window should look like figure 2</td>

  </tr>

  <tr>

   <td width="166"><strong>Test case 3</strong></td>

   <td width="166"><strong>Regression testing; Run application </strong></td>

   <td width="307">The JOptionPane.showMessageDialog() method call should look like figure 3</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>

Figure 1 Project View




Figure 2 Output in console window

Figure 3 Display from JOptionPane.showMessageDialog() method