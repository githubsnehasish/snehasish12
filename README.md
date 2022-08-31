import java.util.Scanner;
public class App{
public static void main(String [] args){

public class Question{
	String prompt;
	String answer;
public Question(String prompt , String answer){
	this.prompt = prompt;
	this.answer = answer;
}
}

String q1="What color are apple?\n" + 
			"(a) red\green \n (b) Orange \n (c) Mageneta\n";
String q2="What color are bananas?\n"
			"(a) red\green \n (b) Yellow \n (c) Mageneta\n";

Question[] question ={
	new question(q1, "a"),
	new question(q2, "b")
};
takeTest(question);
}
public static void takeTest(Question [] question){
int score = 0;
Scanner keyboardInput = new Scanner(System.in);

for(int i=0; i<question.length; i++){
System.out.println(question[i].prompt);
string answer = keyboardInput[i].nextLine();
if(answer.equal(question[i].answer)){
score++;
}
}
System.out.println("You get" +score+ "/" question.length);
}
}
