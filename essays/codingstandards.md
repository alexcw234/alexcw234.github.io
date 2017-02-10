---
layout: essay
type: essay
title: Coding Standards are Important!
date: 2017-02-09
labels:
  - Coding standards

---



I think it is extremely important to have good coding standards. Having a consistant format makes your code easier to read and therefore understand. This helps not only you stay organized but also helps anyone else who is reading your code understand what you are doing.

For an example, this is a small segment of a java program I wrote during the summer after I took ICS 111, before I knew anything about coding standards. It was supposed to find the possible permutations when placing 24 objects into 16 slots based on the objects' properties.

```
void Placer(Member[] PartMem, int[] Sizes, String[] Titles){
if(Current<16 && Current > -1){	
int npos = PartMem[Current].nPositions;
int[] Positions = PartMem[Current].Positions;
int whatpos=0;
for(int i = 0; i < npos; i++){ 
whatpos = Positions[i];
	if(CheckList[whatpos]==false){ 
		Blank[whatpos] = PartMem[Current].memberName;
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
	else if(PartMem[Current].Assigned==true){
		for(int i=0; i< npos; i++){
			int[] tempGoodPositions = PartMem[Current].GoodPositions;
			if(PartMem[Current].GoodPositions[i] == 1){
				for(int v=0; v<npos; v++){
					if(PartMem[Current].GoodPositions[v] == 1 && v != i){
						CheckList[Positions[v]]=false;
					}
				}
				Blank[PartMem[Current].Positions[i]] = PartMem[Current].memberName;
				Current++;
				Placer(PartMem, Sizes, Titles);
				
				for(int v=0; v<npos; v++){
					if(tempGoodPositions[v] == 1){
						CheckList[Positions[v]]=true;
					}
				}
				}		
			}
		if(Current<16){
			PartMem[Current].Unassign();
			for(int r=0; r<npos; r++){
				if(PartMem[Current].GoodPositions[r] == 1){
					CheckList[PartMem[Current].Positions[r]]=false;
				}
			}
			if(Current-1 > -1){
			Current--;	
		} 
		}
	}	
}
else {
	int membercount = 0;
	for(int t=0; t<Titles.length; t++){
		System.out.print(Titles[t]+": ");
		for(int m = membercount; m<membercount+Sizes[t];m++){
			System.out.print(Blank[m]+" ");
		}
		membercount = membercount + Sizes[t];
		System.out.println("");
}
Current--;
RosterCount++;
}
}
}
```
One thing that I am not so keen on in coding standards is restrictions having lines in between lines of code. Sometimes I find this makes the code harder to read, particularly when there is a lot going on. Especially since the opening braces are also supposed to be on the same line as the statement it applies to, rather than a line of its own. 
