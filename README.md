# JAVAS34
public class Student1
{ 		
	int rollno;
	String name;
	int Nsubjects;
	float percentage;
	int marks[]; // till here i done
	public static void main(String[] args)
    {	
		Student(int rno,String n,int nsub;) 
		int rollno=rno; 
		String name=n;
		int Nsubjects=nsub;
    }
    public void getMarks(int nosub )
    {
    marks=new int[nosub];
    BufferedReader br= new BufferedReader (new InputStreamReader(System.in));
    for (int i=0; i<nosub;i++)
    {
    System.out.println("Enter "+i+"Subject Marks.:=> ");
    marks[i]=Integer.parseInt(br.readLine());
    System.out.println("");
    }

    }
    public void calculateMarks()
    {
    double percentage=0;
    int tmarks=0;
    for (int i=0;i<marks.length;i++)
    {
    tmarks+=marks[i];
    }
    percentage=tmarks/Nsubjects;
    System.out.println("Roll Number :=> "+rollno);
    System.out.println("Name Of Student is :=> "+name);
    System.out.println("Number Of Subject :=> "+Nsubjects);
    System.out.println("Percentage Is :=> "+percentage);

    if (percentage>=70)
    System.out.println("First Class With Distinction ");
    else if(percentage>=60 && percentage<70)
    System.out.println("First Class");
    else if(percentage>=50 && percentage<60)
    System.out.println("Second Class");
    else if(percentage>=40 && percentage<50)
    System.out.println("Paas");
    else
    System.out.println("You Are Fail");
    }
    }
    class StudentDemo
    {
    public static void main(String args[])throws IOException
    {
    int rno,no,nostud;
    String name;
    BufferedReader br= new BufferedReader (new InputStreamReader(System.in));
    System.out.println("Enter How many Students:=> ");
    nostud=Integer.parseInt(br.readLine());
    StudentDemo s[]=new StudentDemo[nostud];

    for(int i=0;i<nostud;i++)
    {
    System.out.println("Enter Roll Number:=> ");
    rno=Integer.parseInt(br.readLine());
    System.out.println("Enter Name:=> ");
    name=br.readLine();
    System.out.println("Enter No of Subject:=> ");
    no=Integer.parseInt(br.readLine());
    s[i]=new Student(rno,name,no);
    }
    for(int i=0;i<nostud;i++)
    {
    s[i].calculateMarks();
    }
    }
    
    
    
    
    constructor i create but no working little i just dont understand.. give me the clear instructions.. 
