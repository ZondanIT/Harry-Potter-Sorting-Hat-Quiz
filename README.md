# Harry-Potter-Sorting-Hat-Quiz

#include <iostream>
 
int main() {
 
  // int

  int gryffindor = 0;
  int hufflepuff = 0;
  int ravenclaw = 0;
  int slytherin = 0;
 
 int answer1, answer2, answer3, answer4;

  // welcome msg
  std::cout << "===============\n";
  std::cout << "Hey there, you started The Sorting Hat Quiz! \n"; //start
  std::cout << "===============\n\n";


  // ~~~~~~~~~~ Question 1 ~~~~~~~~~~

  std::cout << "Q1) When I'm dead, I want people to remember me as:  \n";
  std::cout << "1) The Good \n";
  std::cout << "2) The Great \n";
  std::cout << "3) The Wise \n";
  std::cout << "4) The Bold \n \n";
  std::cin >> answer1;

// ~~~~~~~~~~ Condition ~~~~~~~~~~
  
if (answer1 == 1){
  hufflepuff++;
} else if( answer1 == 2){
  slytherin++;
} else if( answer1 == 3){
  ravenclaw++;
} else if( answer1 == 4){
  gryffindor++;
} else{
  std::cout << "Invalid input \n \n";
};

  // ~~~~~~~~~~ Question 2 ~~~~~~~~~~

std::cout << "Q2) Dawn or Dusk? \n";
std::cout <<"1) Dawn \n";
std::cout <<"2) Dusk \n";
std::cin >> answer2;

// ~~~~~~~~~~ Condition ~~~~~~~~~~

if (answer2 == 1){
  gryffindor++;
  ravenclaw++;
} else if(answer2 == 2){
  hufflepuff++;
  slytherin++;
} else{
  std::cout << "Invalid input. \n \n ";
};

  // ~~~~~~~~~~ Question 3 ~~~~~~~~~~

std::cout << "Q3) Which kind of instrument most pleases your ear? \n";
std::cout << "1) The Violin \n";
std::cout << "2) The Rumpet \n";
std::cout << "3) The Piano \n";
std::cout << "4) The Drum \n";
std::cin >> answer3;

// ~~~~~~~~~~ Condition ~~~~~~~~~~

if(answer3 == 1){
  slytherin++;
} else if(answer3 == 2){
  hufflepuff++;
} else if(answer3 == 3){
  ravenclaw++;
} else if(answer3 == 4){
  gryffindor++;
} else{
  std::cout << "Invalid input \n \n";
};

  // ~~~~~~~~~~ Question 4 ~~~~~~~~~~

std::cout << "Q4) Which road tempts you most? \n";
std::cout << "1) The wide, sunny grassy lane \n";
std::cout << "2) The narrow, dark, lantern-lit alley \n";
std::cout << "3) The twisting, leaf-strewn path through woods \n";
std::cout <<"4) The cobbled street lined (ancient buildings) \n";
std::cin >> answer4;

// ~~~~~~~~~~ Condition ~~~~~~~~~~

if(answer4 == 1){
  hufflepuff++;
} else if(answer4 == 2){
  slytherin++;
} else if(answer4 == 3){
  gryffindor++;
} else if (answer4 = 4){
  ravenclaw++;
} else{
  std::cout << "Invalid input. \n \n";
};

// 

int max = 0;
std::string house;

if (gryffindor > max){
  max = gryffindor;
  house = "Gryffindor";
}
if(hufflepuff > max){
  max = hufflepuff;
  house = "Hufflepuff";
}
if(ravenclaw > max){
  max = ravenclaw;  
  house = "Ravenclaw";
}
if (slytherin > max){
  max = slytherin;
  house = "Slytherin";
}

std::cout << " House: "<< house << "! \n";

return 0;
};



