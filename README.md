object means maan ek class Student {}   ab iska Student s1=new ...  toh s1 object 
# contructor 
<img width="667" height="712" alt="image" src="https://github.com/user-attachments/assets/be8f6baf-05dc-4b37-915f-35a63e53397d" />
yaha upar dekh conructor mein like kitne bhi daal sakta so maan u bina uske ya kisis value ki intialise toh pehle wala constructior run hoga aise 


Student () {
        // this is how you call a constructor from another constructor
        // internally: new Student (13, "default person", 100.0f);
        this (13, "default person", 100.0f);
    }


    // Student arpit = new Student(17, "Arpit", 89.7f);
    // here, this will be replaced with arpit
    Student (int rno, String name, float marks) {
        this.rno = rno;
        this.name = name;
        this.marks = marks;
    } 

    like meri baat sun 
     Student one = new Student(); ye karega toh basically it will call the student jisme this() so ab ye aage wle ko call this yaha pe  Student (13, "default person", 100.0f); but sun jaise this.name=name so yaha pe tu sirf this one.name hua thik yaha tu bata raha ki one wale object ka name hai uski value ye ho gi


# final 
so final keyworkd 
final int =5 so ab int ko 5 hi hona padgea if intialise i karega toh error pehle call ke time intialize 
final Student one =new st..  if yes karega toh one.name="keshav  ye kar sakta as upar parametric value toh yaha one final but andar ki value final ni

# pass by value 
so java is always pass by vlaue
but ek void func m int a b ja raha toh bhale andar swap par main a b swap ni as vo pass by value means value copy ho jaa ri
when array pass in void that array ka bhi pass by value par araay arr jab toh vo address deta so even jo void ya func vo array ke adress ko copy kar let so isliye jab array jaise obj func m pass toh uss array m bhi change as func m bhi arry ke andar change same adress us karke aa raha 

 <img width="387" height="88" alt="image" src="https://github.com/user-attachments/assets/bdd11aef-c4ef-4f5c-a39b-1c21c7a86ebe" />
ye finalize method jaise hi koi class chalti tab last m chalt so garbage collector jaise wrlk means maan le bahut sari func var ban gaye toh dhere dhere if space ni bachi but naye funct var bante rahe toh ye purane wale unko collect remove karta rahega like tune bahut sari tree class ke obj ab bante ja rahe toh space limited toh purane remove kar dega on own 

# package 
means folder ke adar msubfolder 
com.keshav.a so com.keshav ke andar a folder and com.keshav.b bhi toh b folder keshav ke andar and sun tu video oops 2 suru ka part dekh le 

# tu import com.keshav.student.Student(ye student vo class).message -> ye message ek funct uss class m


# static 
isme like maine maanle ek pakage keshav uske andar a.java mein banaya 
 <img width="377" height="75" alt="image" src="https://github.com/user-attachments/assets/72c5e726-48fa-4697-adc0-02fcc78c9832" />
aise same folder ke andar a b so ek dusre ke public func ko acess kar sakte ya static so even b mein static +1 toh chahe kitne bhi instance bana le a a1 = new a()
then a a2=new a()  ye dono same a class ko like point but sono alag obj but ek baat sun a mein jo static vo dono ke liye same if ek usse change toh baki m bhi change hoga

<img width="356" height="167" alt="image" src="https://github.com/user-attachments/assets/b920cf32-14eb-4ce0-bf2d-bca0415ed34b" />
if aise ek banaya tune toh b mein kahi bhi tu direct a.a like ke acess koi zrurtat ni new a() koi zarurat ni class ka obj banne ki direct acess kar le static is free 

Public static void main(s).. ye static isliye ki ye allow karta ki uss class ko run kar sake bina uski object banye 
static belog to class means jaha vo class use vaa same rahega vo static object means jab tu same class ka use karke diff object banta like student 1 2 whatever

 static mein non static ko call karne ke liye object create karna padgea
 3. and maan ststic folder uske andar this use ni kar sakta as static means class ka hai this for object this kayde se uss object name se replace

 4. <img width="430" height="382" alt="image" src="https://github.com/user-attachments/assets/4f66b3f4-63fd-4fef-a01f-feccaa01b8e8" />
 so yaha dekh jaise class ke andar if ek class toh usko tujhe static if ni maan aise hi static ni test to error hai error even if Test a =new Test() kar dega tab bhi as dekh test upper inner class oe depndent and ststic bolta ki mujhe pura logical way chaiye but jab tu staic bana deta toh fir tu usse main wale static mein acess kar sakta and yaha pe kunal and    rahul alag bante ab tu puchega kyon test statsic toh fir toh aisa ni hona chaiye tha but main bhi static islliye ban jata as tu naya object bana raha static means ye yaad ki apni class se independent ab vo uss class ka hi object hai class se jud gaya direct and main

5. outer class static ni ho sakti  as static ko chaiye ek parent jispe vo chipak jaaye
Araay.toStrig toh ye Array name ke class se to string wala method call kar deta hai simple as simple




# TO string
<img width="380" height="331" alt="image" src="https://github.com/user-attachments/assets/ee7f941f-6ebe-4a66-96fd-565a9aa74aae" />
jaise yaha dekh upa maine class ko print karna chah toh piche println ne dekha ki iss class mein tostring hai kya if yes uss chala de if ni toh uss class ka name and hex value priint kar deti hai so its just funct class ka combination



# singleton

means sirf ek variable create akrta hai tu ya ek object create ho sakti kisis class ki and baaki object same ushi class ko call

<img width="483" height="453" alt="image" src="https://github.com/user-attachments/assets/783c624a-8dcf-45cc-9ecc-e2762de4e74a" />

ab tu alag alg bana ke bhi karega tab bhi vo sab same class ko hi refer karenge an return
<img width="514" height="294" alt="image" src="https://github.com/user-attachments/assets/200fd9bb-21d4-4f2a-b2ab-0db32c8e8960" />


# Inheritance 

impt jab bhi tu parent ko like ectend sme ek default contructor hona chaye 

                public  class b {
                   int l;
                   int b;
                   int w;
                   public  b(){
                       
                   }
                   public  b(int l,int b,int w){
                       this.w=w;
                       this.l=l;
                       this.b=b;
                   }
                        }
                        
                        class c extends  b{
                    
                        }

<img width="667" height="712" alt="image" src="https://github.com/user-attachments/assets/be8f6baf-05dc-4b37-915f-35a63e53397d" />
Ye niche wala super apne parents ke contructor ko call kar dega jaise yaha pe box ke 3 double wala constructor run hojayega 

<img width="952" height="425" alt="image" src="https://github.com/user-attachments/assets/38652075-00d9-4cf6-97e6-95817f23e4b9" />



Yaha pe dekh jaise Box parent and box wiegth se intitlise so kar sakta as boxwieght mein parent ke sare element but boxwoeght mein ek var weight 
jab tu usse box5.weight to error as kitne element tu acess ye tu kisse intitlize usse tai hota yaad rakhna \
And boxwieght object new box ()  karke ni intilaize as child parent ke object se intilize ni ho sakta 
<img width="826" height="139" alt="image" src="https://github.com/user-attachments/assets/b893bd6b-9cd0-43b2-bbef-f375cd2bc0b4" />


Ab ek cheez samjha this.w se tu parent ke w ko acess kar sakta haui 
so like in this this.w se parent ke w ko aacess 

```` java
public  class b {
   int l;
   int b;
   int w;
   public  b(){

   }
   public  b(int l,int b,int w){
       this.w=w;
       this.l=l;
       this.b=b;
   }
        }

        class c extends  b{
            int weight;

            public c(){
                System.out.println(this.w);
            }
        }
````
so jaise above dekh this.w se acess but ise acess ni karte 
super.w se bhi same weight but super bata ki parent ko acess for ex w parent m bhi and hild mein bhi w so now this apne andar wale means child wale class ka w layega so
super() for super ke constructor ko acess and super.w ya super.fucntion name se parent 

2. ye niche dekh boxweight mein ek constructor jo like boxwieght se intitlise toh vo box wieght box type ke contructor ko call with same box weight bhej ke so ye aisa kuch Box b=new BoxWoeght jo sahi as dekh boxwieght ke pas sab kuch jo box type ke pas so ye sahi hai 
<img width="577" height="416" alt="image" src="https://github.com/user-attachments/assets/2b6e4fc9-c2dc-403d-9a64-3a07b92e8ac6" />

<img width="361" height="223" alt="image" src="https://github.com/user-attachments/assets/a93687ac-d56d-47bd-ab43-1893b9c13697" />


3. You can checkout video like multihertance mein super keyword kaise use bataya hai dekh sakta hai

**Types of inheritance**
1. single
2. multitype mein ek ke niche ek
3. multiple inheritance is not in java like dk child multiple parent ko extend
4. heirachial inheritance

# polyphorphism

many function or feature of same name 

1. jaise ye dekh shpe sabse upar parent and circle and triangle uske child so parent ke pas bhi apna area and dono child ke pas bhi so 
if aage Shape s=new SHape toh s.area() toh shape ka area hoga print same if circle ke constructor se karnege toh child ka hoga 
<img width="356" height="191" alt="image" src="https://github.com/user-attachments/assets/501461ab-592e-4f91-9a76-0c1e1795def3" />
2. But catch if maan le SHape s=new Cricle()  s.area() circle ka area function print karega ye poly mor[phism ka ek point like jiss function se vo

## types of polymorphism
1. compile time /static : overloading -> yaha same name hota hai but types of parameters,no. of parameters , return type differnt ho sakta
ye cheez constructor and function dono pe lagta
2. runtime : overridding -> yaha pe parent ke kisi func ya element ko overide karte

````java
package com.keshav.hello;


public class a {
    int wr=19;
    static class test{
        String a="keshav";
    }
    public String hello(){
        return "iam parent";
    }
}


public  class b extends a{
   int l;
   int b;
   int w;
   public  b(){

   }
   public  b(int l,int b,int w){
       this.w=w;
       this.l=l;
       this.b=b;
   }
   public  String hello(){
        return "iam child";
   }


        }


        class main{
            public static void main(String[] args) {
                a j=new b();
                System.out.println(j.hello());
            }
        }
// output-> Iam child

````
2. Yaha pe dekh Kayde se main j a type ka toh usse iam parent but yaha output iam child why kyonki jab tune b() se inilize toh if hello parent mei ni hota j.hello error paka deta but ab a mein bhi hello and jab tune b se intitlize toh a wala hello overid ehoke b wala hello bana gaya if pure a wala hello toh a() se intilize kar so ye yaad rakhna
3. kayde se ab bhi j se sirf vo hi elemnt  a j=new b(); acess jo a mein hai bas b se intilize ki vaah se a wale same name wali func overide ho jayenge if child ne overid kiya hai toh


ek aur cheez jaise tu class main {} aise bina etend bhi jab  kata toh tostring ya aur sari func overide kaise ek baat dhyadn rakh bydefault java mein object class ko  sari class extend karti hai
<img width="334" height="144" alt="image" src="https://github.com/user-attachments/assets/ca350662-61f6-451b-8651-db57044a9530" />


# Abstract 
```java
package com.keshav2.p;

import com.keshav.hello.a;

public abstract  class hello {
    public abstract  void hello();
public   abstract  String peop();
}

class main extends  hello{

    public main(){}
    
    int p(){
        return 1;
    }
    
    @Override
    public void hello() {
        
    }

    @Override
    public String peop() {
        return "";
    }
}
```
you can also like create abstract class constructor bas tujhe uss constructor ko jisme extend vaha pe like call karna padega 
```java
public abstract  class hello {
    int age;
    public hello(int age){
        this.age=age;
    }
    public abstract  void hello();
public   abstract  String peop();
}

class main extends  hello{

    public main(){
        super(12);
    }

    int p(){
        return 1;
    }

    @Override
    public void hello() {

    }

    @Override
    public String peop() {
        return "";
    }

    public static void main(String[] args) {
        main a=new main();
        System.out.println(a.age);
    }
}
```
