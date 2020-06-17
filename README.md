# COVIDChatBot
Repository for the team's hackathon entry, a simple chatbot that provides information and resources for COVID
import java.util.Scanner;
public class Resources{
   public static String Resources(){
      return "Which of the following resources would you like to know more about?";
   }
   public static void main(String[] args){
    
      Scanner scan = new Scanner(System.in);
       
        System.out.println("Hey there! I'm Codi, your new COVID-19 ResourceBot! What would you like me to provide?");
      System.out.println();
        
        System.out.println("For General Options, enter '1'"); 
        
        System.out.println("For Resources, enter '2'"); 
        System.out.println();
        System.out.println("Please enter your choice:");
        
        
        int choice = scan.nextInt();
        
        
     
        switch (choice) {
            case 1: System.out.println("General options:"); 
            System.out.println("1. How does the virus spread?");
            choice = scan.nextInt();
            if(choice == 1)
               System.out.println("like this");         
	   break;
            case 2: System.out.println("You chose 'Resources'!:");
            System.out.println("-------------------------------------");
           
            System.out.println("Enter the number of the resource you need!");
            System.out.println("1. Link to the CDC website");
            System.out.println("2. Link to find a testing location near you");
            System.out.println("3. Link to the CDC COVID-19 self-assessment"); 
            System.out.println("4. How to make your own face mask!");
            System.out.println();
            System.out.println("Please enter your choice:");
            int resourceNum = scan.nextInt();
            if(resourceNum == 1){
               System.out.println("Copy and paste the link below!");
               System.out.println("https://www.cdc.gov/coronavirus/2019-ncov/index.html");
               break;
               }
            else if(resourceNum == 2){
               System.out.println("Copy and paste the link below!");
               System.out.println("https://cvshealth.com/covid-19/testing-locations"); 
               break;
               }
            else if(resourceNum == 3){
               System.out.println("Copy and paste the link below!");
               System.out.println("https://landing.google.com/screener/covid19");   
               break;  
               }
            else if(resourceNum == 4){
               System.out.println("Copy and paste the link below!");
               System.out.println("https://youtu.be/tPx1yqvJgf4");  
               break;
               }
        }
    } 
} 
 
