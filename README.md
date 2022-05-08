# pstv

What Smart Contracts (Really) Do
Even in just these first few pages, you may have encountered some wildly new concepts. But there’s one term which will continue to pop up in Ethereum, and that is the notion of a smart contract: some business logic that runs on the network, semi-autonomously moving value and enforcing payment agreements between parties. Smart contracts are often equated to software applications, but this a reductive
analogy; they’re more like the concept of classes in conventional object-oriented programming. When developers speak of “writing smart contracts,” they are typically referring to the practice of writing code in the Solidity language to be executed on the Ethereum network. When the code is executed, units of value may be transferred as easily as data. As stated in this chapter already, the promise of digital money is immense. But how does it work, exactly? How can data act like money in a decentralized system? The answer to that question depends on how technical you are. So let’s take a fairly
in-depth example.
Objects and Methods for Value In computing, an object is usually a little chunk of data—information—encapsulated in a particular structure or format. Often this data has associated instructions called methods indicating how the object can be used or accessed. Now let’s imagine the information held in this object is valuable to someone, and this person would be willing to pay to trigger a method which displays it. In the example below, let’s imagine a user wants to pay a small fee to use a cake
recipe he or she discovered online. This recipe is the data object in our example. At the most literal level, the characteristics of the cake object, called attributes, are stored along with the methods at a certain address in the computer’s memory. The object below represents the attributes of a cake, and contains a method whereby
the computer can display instructions for how to combine these ingredients to make the cake. Storing the information in this way makes it easy for the program and the programmer to swap in and out the attributes without needing to change the code for the display instructions. In other words, objects are modular chunks of information which can be combined and recombined to suit. This will be important to remember in later chapters when we discuss the anatomy of the blocks that comprise the blockchain. In JavaScript, you can write a cake object as follows:
var cake = {
firstIngredient: "milk", secondIngredient: "eggs",
thirdIngredient: "cakemix", bakeTime: 22
bakeTemp: 420 mixingInstructions: function() {
return "Add " this.firstIngredient + " to " + this.secondIngredient + " and stir with " + this.thirdIngredient + " and bake at " + bakeTemp + " for " + bakeTime + " minutes." ; }
}; This is an example of how computers “move” data around to display useful results
to their human users. In Ethereum, you can write functions that send money around, just as this little object’s method called mixingInstructions, when executed, can display the mixing instructions for a cake.


