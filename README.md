# contructor 
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
