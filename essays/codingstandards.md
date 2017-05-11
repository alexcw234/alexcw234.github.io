---
layout: essay
type: essay
title: Coding Standards are Important!
date: 2017-02-09
labels:
  - Coding standards

---

I believe that it is extremely important to have good coding standards. Having a consistant format makes your code easier to read and therefore understand. This helps not only you stay organized but also helps anyone else who is reading your code understand what you are doing.

I am especially aware of this as it applies to javascript, as I wrote in my [javascript reflection essay](https://alexcw234.github.io/essays/javascript1.html), bad coding standards was a huge reason for why I had such a bad first impression of the language. 

As another example, this is a small segment of a java program I wrote during the summer after I took ICS 111, before I knew anything about coding standards. It was supposed to find the possible permutations when placing 24 objects into 16 slots based on the objects' properties.

```
void Placer(Member[] PartMem, int[] Sizes, String[] Titles){
if(Current<16 && Current > -1){	int npos = PartMem[Current].nPositions;
int[] Positions = PartMem[Current].Positions;
int whatpos=0;
for(int i = 0; i < npos; i++){ 
whatpos = Positions[i];
if(CheckList[whatpos]==false){ Blank[whatpos] = PartMem[Current].memberName;
	CheckList[whatpos] = true;	
	PartMem[Current].Assign();
	PartMem[Current].Good(i);
} else {PartMem[Current].NotGood(i);}	
}
if(PartMem[Current].Assigned==false){
	PartMem[Current].Unassign();
	for(int r=0; r<npos; r++){
		if(PartMem[Current].GoodPositions[r] == 1){
			CheckList[PartMem[Current].Positions[r]]=false;
		}
	}
	Current--;	
}
}
```
In this example it's difficult to look at this and figure out what was going on. If I had written this using a structured format, while it would have still taken time to understand since it has been so long, at least I would have a starting point. It would be even easier to understand if I had made comments in the code.

Even though I understand the value of coding standards, I sometimes find myself getting mixed up and writing inconsistantly, especially in regards to whether to put braces on a new line or on a preceding line, or what way of declaring variables and arrays I should be using. The style I naturally gravitate towards tends to vary depending on the language as well. Perhaps then, this is a reason why I like Python as a language, as it tends to enforce a certain style.

As it is difficult to keep track of all the rules of a coding standard, I have found that it is definitely helpful to have something a coding standard checker like ESLint (along with and IDE like IntelliJ) to keep track of my code and let me know when I have been inconsistant. Through using ESLint over a period of months, I have found that it has helped me to eliminate certain habits and inconcistanclies I have in coding. For example, I often can't decide how to place my braces and how many spaces to make my tabs. This leads me to putting an open brace on the separate line from a function declaration in one part of my code, while putting it in-line elsewhere.

However, there are certain rules that I cannot seem to get used to. For example, needing to name a function that is called only as a parameter for another function. To me, it often seems unneccessary and only clutters up the display. Another thing that I am not so keen on in coding standards is restrictions having lines in between lines of code. Sometimes I find this makes the code harder to read, particularly when there is a lot going on. Especially since the opening braces are also supposed to be on the same line as the statement it applies to, rather than a line of its own. 

Even with the handfull of rules I don't agree with, having a coding style enforced is extremely beneficial to writing consistent and easy-to-understand code. Although I personally could do without some of the "convenience" features of an IDE––the autoclosing of quotes and brackets for instance––the benefits of ESLint cannot be ignored.




