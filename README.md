# **JavaScript** #

##Creating an object##

1. Object Constructor   => Create several similar objects  => Classes
2. Literal constructor  => One object of a kind
3. Function constructor
4. Protoype Based
5. Function and Prototype Based
6. Singleton Based


### Examples:

1.) Object constructor

<!-- language: javascript -->

    var person = new Object();
        
    person.name = "Anand",
    person.getName = function(){
      return this.name ; 
    };

2.) Literal constructor


<!-- language: javascript -->

    var person = { 
      name : "Anand",
      getName : function (){
       return this.name
      } 
    } 

3.) Function Constructor


<!-- language: javascript -->

    function Person(name){
      this.name = name
      this.getName = function(){
        return this.name
      } 
    } 


4.) Prototype


<!-- language: javascript -->

    function Person(){};

    Person.prototype.name = "Anand";


5.) Function/Prototype combination


<!-- language: javascript -->

    function Person(name){
      this.name = name;
    } 
    Person.prototype.getName = function(){
      return this.name
    } 

6.) Singleton


<!-- language: javascript -->

    var person = new function(){
      this.name = "Anand"
    } 
