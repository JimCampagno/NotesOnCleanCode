# NotesOnCleanCode


#Chapter 4 - Comments

* Comments are a necessary evil.
* The proper use of comments is to compensate for our **failure**.  
* Every time you write a comment, you should grimace and feel the **failure** of your ability of expression.  
* Programmers can't realistically maintain them.  
* Available energy should go toward making the code so clear and expressive that it does not need the comments in the first place.  
* Truth can only be found in one plade: **the code**.

##Explain Yourself In Code  
  
```
//Example in OBJ-C - BAD use of comments.
FISEmployee *employee = [FISEmployee new];  
employee.age = 26;
employee.yearsWithTheSchool = 2;
employee.favoriteColor = @"red";

//Is Employee elgigible for being considered cool?
if ((employee.age < 40 &&
     employee.yearsWithTheSchool > 5 &&
   ![employee.favoriteColor isEqualToString:@"red"]))
```  
Create a function that says the same thing as the comment you want to write.  For example:  
  
```
if (employee.isConsideredCool)  
```  
* The only truly good comment is the comment you found a way **not** to write.  
  
##Good Comments  
* Legal Comments  
* Informative Comments
* Clarification  
* Warning of Consequences  
* TODO Comments
* Amplification  

##Bad Comments  
* Mumbling  
* Redundant Comments  
* Misleading Comments  
* Mandated Comments  
* Journal Comments  
* Noise Comments  
* Scary Noise  
* Don't use a comment when you can use a function or a variable  
* Position Markers  
* Closing Brace Comments  
* Attributions and Bylines  
* Commented-Out-Code  
* HTML Comments  
* Nonlocal Information  
* Too Much Information  
* Inobvious Connection  
* Function Headers  
  
**QUESTION:** When you're about to step away from a problem you're in the middle of, do you write lenghty comments (possibly dated) of the problem at hand and what your thought is at the moment in how you feel it should be tackled?  
  
#Chapter 5 - Formatting  
  
* Take care that your code is nicely formatted.  
* Choose a set of simple rules that govern the format of your code.  **Consistently** apply those rules.  
* Your style and discipline survives, even though your code does not.  
* Small files are usually easier to understand than large files are.  
* The source file should be like a **newspaper article**.  
* Detail should increase as we move downward, until at the end we find the lowest level functions and details in the source file.  
  
**Vertial Openness** - Each blank line is a visual cue that identifies a new and separate concept.  
**Vertical Density** - Lines of code that are tightly related should appear vertically close.  
**Vertical Distance** - Concepts that are closely related should be kept vertically close to each other.  We want to avoid forcing our readers to hop around through our source files and classes.  
**Variable Declarations** - Variables should be declaared as close to their usage as possible. *Instance variables* should be declared at the top of the class because they are used by many, if not all, of the methods of the class.  
**Dependent Functions** - If a function calls another, they should be vertically close and the caller should be above the callee.  
**Conceptual Affinity** - Affinity *might* be cause because a group of functions perform a similiar operation.  
**Vertical Ordering** - Function call dependencies should point in a downward direction.  A function that is called should be below a function.  
**Horizontal Openness and Density** - Use horizontal white space to associate things that are strongly related and dissasociate things that are more weakly related.  Surround assignment operators with white space to accentuate them.  
**Horizontal Alignment** - Use unaligned declarations and assisgnments.  If there are long lists that need to be aligned, the problem is the length of the lists, not the lack of alignment.  
     


   