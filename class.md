1. Class - Movie
=================

class Movie{
    constructor(title,studio,rating){
      this.title=title;
      this.studio=studio;
      if(rating===undefined || rating===null)
     this.rating="PG13";
     else
     this.rating=rating;

    }
    getpg(Moviearray){
      var temp=[];
      
      for(var i in Moviearray)
      if(Moviearray[i].rating=="PG")
      temp.push(Moviearray[i].title);
      return temp
      
     
    }
}
var n1=new Movie("abc","cde","PG");
var n2=new Movie("hij","cde","PG");
var n3=new Movie("efg","cde","PG");
var n4=new Movie("Casino Royale","Eon Productions","PG13")
var a=[];
a.push(n1,n2,n3,n4);
console.log(n1.getpg(a));




2. Circle - Class
====================

class Circle {
    
    constructor(radius,color){
        this.radius=radius;
        this.color=color;

    }
getRadius(){
    return this.radius;
}
setRadius(radius){
     this.radius=radius;
     }
    getColor(){
        return this.color;
    }
    setColor(color){
this.color=color;
    }
    
    toString(){
    return "Circle[Radius = " + this.radius + ", Color = " + this.color +"]";

    }
    getArea(){
    return Math.PI*Math.sqrt(this.radius);
    }
    getCircumference(){
        return 2*Math.PI*this.radius
    }
}


var a=new Circle();
var b=new Circle(1.0);
var c=new Circle(1.0,"red");
console.log(b.getRadius());
b.setRadius(2.0);
console.log(b.getRadius());
console.log(b.getArea());
console.log(c.getColor());
c.setColor("cyan");
console.log(c.toString());
console.log(b.getCircumference());




3. Write a "person" class to hold all the details:
===============================================
class Person{
    constructor(firstName,lastName,age,address){
        this.firstName=firstName;
        this.lastName=lastName;
        this.age=age;
        this.address=address;
    }
}
var p=new Person("Parvad","raj",21,"Banglore");

4. write a class to calculate the uber price
=============================================
class Uber{
    constructor(distance){
        this.distance=distance;

    }
  uber(){
let totCost=0,dist=this.distance*10;
for(var m=1;m<=dist;m++){
if(m<=100)
totCost+=10;
else if(m>=200)totCost +=(distance*12);
else totCost +=(distance*15);
}
return totCost;
}}
var p=new Uber(10);
console.log(`Uber price:
Distance: ${p.distance} 
Price:${p.uber()}`);
var u=new Uber();

