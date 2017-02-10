---
layout: essay
type: essay
title: Coding Standards are Important!
date: 2017-02-09
labels:
  - Coding standards

---



I think it is extremely important to have good coding standards. Having a consistant format makes your code easier to read and therefore understand. This helps not only you stay organized but also helps anyone else who is reading your code understand what you are doing. 

```
void Placer(Member[] PartMem, int[] Sizes, String[] Titles){
if(Current<16 && Current > -1){	//
	
int npos = PartMem[Current].nPositions;	 //number of total positions the currently-being-placed member has
int[] Positions = PartMem[Current].Positions; //Array of those positions x through xi
int whatpos=0;

for(int i = 0; i < npos; i++){ //For every position the Current member has...
	
whatpos = Positions[i];

	if(CheckList[whatpos]==false){ //if there is no one in position xi, assign to position xi
		Blank[whatpos] = PartMem[Current].memberName;
//System.out.println("Available positions for "+PartMem[Current].memberName+" at "+whatpos);
		CheckList[whatpos] = true;	
		PartMem[Current].Assign();
		PartMem[Current].Good(i);
		
	} else {PartMem[Current].NotGood(i);}
	//otherwise repeat for the next position	
}
//now if all positions have been checked
	//If no assignments have been made, back up a step
	if(PartMem[Current].Assigned==false){
//System.out.println("No path for "+PartMem[Current].memberName);	
		PartMem[Current].Unassign();
		for(int r=0; r<npos; r++){
			if(PartMem[Current].GoodPositions[r] == 1){
				CheckList[PartMem[Current].Positions[r]]=false;
			}
		}
		Current--;
//System.out.println("UP ONE LEVEL TO "+Current);	
		
	}	
}
```
One thing that I am not so keen on in coding standards is restrictions having lines in between lines of code. Sometimes I find this makes the code harder to read, particularly when there is a lot going on. Especially since the opening braces are also supposed to be on the same line as the statement it applies to, rather than a line of its own. 
