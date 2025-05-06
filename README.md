# lab-9---inheritance-solved
**TO GET THIS SOLUTION VISIT:** [Lab 9 – Inheritance Solved](https://www.ankitcodinghub.com/product/lab-9-inheritance-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;12755&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;6&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (6 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Lab 9 – Inheritance Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (6 votes)    </div>
    </div>
<h1>Overview</h1>
In this assignment, you’re going to create a series of classes to represent simple 2D and 3D shapes. While the classes themselves are all simple, you will be using <em>inheritance</em> &amp; the concept of <em>polymorphism</em> to store and use a group of these separate classes. You will also create classes which make use of multiple inheritance, as well as private inheritance.

<h1>A note about Pi and math functions</h1>
While many languages have math libraries of varying size and complexity built into them, C++ includes little, if any, such functionality. The value of PI, for example, is not officially defined in any C++ standard, although some header files provided by various creators of compilers do contain them.

For a standard in this assignment, you should use the following definition of PI, in one of two different ways:

#define PI 3.14159f // Do a simple find-and-replace of PI everywhere in your code const float PI = 3.14159f; // Create an actual variable with PI as its value.

&nbsp;

Also, in this assignment you should use the float data type instead of double to ensure proper results.

Lastly, there exists a header file called &lt;math.h&gt; which you can include to get access to some useful functions such as the pow() function, which lets you raise a value to an exponent and return the result.

<h1>Description</h1>
The basic idea of inheritance is that you have a <strong><u>base</u></strong> class, and you create new classes which <strong>derive</strong> from that base class. One common use of inheritance is to reuse data and functions: if a base class defines those things, then the derived class doesn’t have to; it inherits them, so in effect, you get “free” code in that class.

Another use of inheritance is to define a class which serves as what other programming languages would call an <strong>interface</strong>. In C++, the keyword interface doesn’t exist, but some of the classes you create here will serve the same purpose. An interface defines how a class should look on the outside.

The first three classes shown below will serve as these interfaces; all the other classes will derive, ultimately, from those 3 base classes. In this way, all classes in this assignment are Shapes, even if their type is Triangle, Sphere, Circle, etc. Some types of inheritance model the “Is-a” relationship—a triangle IS A shape. A circle IS A shape as well. The “Is-a” model is heavily used in relational databases.

Other types of inheritance model a “has-a” relationship. A car, for example, has an engine—but it isn’t an engine. This type of relationship can still be created, but the process is a bit different.

&nbsp;

<h1>Class Description</h1>
Let’s look at the first level of these classes: the Shape, Shape2D, and Shape3D:

Shape is an abstract base class. Because <u>at least one</u> of the functions in this class are <strong>pure virtual functions</strong> (i.e. virtual functions with = 0 at the end of the prototype, and no definition). This base says that all Shapes can scale, and display their data. Each derived class can define HOW they scale or display. (Each class should multiply all of its components by the passed-in scaleFactor variable).

&nbsp;

Shape2D derives from the Shape class (a 2D shape IS A shape). Like the Shape class, it is also an abstract base class.

All Shape2D objects have an Area() &amp; ShowArea() function. In addition, comparison operators are overloaded so that a Shape2D can compare itself to other shapes to test different relations, in terms of the shape’s area. These functions will be defined only once, in this class. All classes deriving from Shape2D will inherit them.

The definition of these functions will simply be comparing the Area() of “this” to the Area() of the incoming object (greater than, less than, or equal to, respectively). Due to polymorphism, you will not have to define one of these comparisons for every possible combination of shapes, but instead you could compare the area of a circle against a triangle, square, hexagon, etc… any class deriving from Shape2D will be able to use these 3 functions as-is.

&nbsp;

&nbsp;

The same is true for the Shape3D class—it’s an abstract base class that does not define two functions relating to volume, but instead requires child classes to define them. The overall concept is still the same though.

The comparison operators will have to be defined in terms of the Volume() function of these shapes. Like the Shape2D class, these can be defined once in this class, and all Shape3D objects can use them as-is.

&nbsp;

<h2>GetName2D() vs GetName3D()</h2>
Why two different versions of GetName()? Couldn’t you just inherit one from the base Shape class? Some classes have both 2D AND 3D components. A TriangularPyramid, for example, IS A 3D Shape, but it HAS A 2D Shape. As a result, any calls to Triangle::GetName() will be through a 3D Shape pointer, instead of a 2D Shape pointer.

<h2>ShowArea() and ShowVolume()</h2>
These two functions can be reused across any type of 2D or 3D shape, respectively. We don’t need these functions to be virtual themselves, but they will be calling virtual functions. For example, in the ShowArea() function: void Shape2D::ShowArea() const

{

// Each of these function is invoked by a Shape2D pointer (this)

// Polymorphic behavior determines which specific version is called

// If “this” is a Circle, call Circle::GetName() and Circle::Area()&nbsp;&nbsp;&nbsp;&nbsp; // If “this” is a Rectangle, call Rectangle:GetName(), etc… &nbsp;&nbsp;&nbsp;&nbsp;cout &lt;&lt; GetName2D() &lt;&lt; endl;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; cout &lt;&lt; Area() &lt;&lt; endl;

}

&nbsp;

The same concept applies for the Shape3D class and ShowVolume.

&nbsp;

<h2>2D Shapes</h2>
The classes derived from Shape2D are going to be based on calculating the area of common shapes. The shapes and their respective area formulae are:

<table width="0">
<tbody>
<tr>
<td width="199"><strong>Shape </strong></td>
<td width="435"><strong>Area Formula </strong></td>
</tr>
<tr>
<td width="199">Square</td>
<td width="435">Area = 𝑠<sup>2</sup>

s = length of side
</td>
</tr>
<tr>
<td width="199">Rectangle</td>
<td width="435">Area = w x h

w = width h = height
</td>
</tr>
<tr>
<td width="199">Triangle</td>
<td width="435">Area = 𝑏ℎ

b = length of base h = height
</td>
</tr>
<tr>
<td width="199">Circle</td>
<td width="435">Area = π𝑟<sup>2</sup>r = radius</td>
</tr>
<tr>
<td width="199">Ellipse</td>
<td width="435">Area = πab

a = semi-minor axis b = semi-major axis
</td>
</tr>
<tr>
<td width="199">Trapezoid</td>
<td width="435">Area =

a&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; = side

b&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; = side h = height
</td>
</tr>
<tr>
<td width="199">Sector</td>
<td width="435">1 Area = &nbsp;𝑟<sup>2</sup>𝛳

2

r = radius

𝛳 = angle in radians
</td>
</tr>
</tbody>
</table>
Reference: <u><a href="https://www.mathsisfun.com/area.html">https://www.mathsisfun.com/area.html</a></u> (It also has an area calculator to test against your code)

Because they inherit from Shape2D, you will have to implement the four functions required by the abstract base classes. In addition, each class should have:

<ul>
<li>A default constructor – initialize all member variables to 0</li>
<li>A constructor which takes in parameters for each of the main components, like this (all variables are <strong>floats</strong>):</li>
</ul>
Square(length of each side)

Rectangle(width, height) [Note: these would be interchangeable in most, but not necessarily all scenarios]

Triangle(base, height)

Circle(just a radius)

Ellipse(length of the major axis, length of minor axis)

Trapezoid (length of one parallel side, length of the other, height) Sector(radius, angle in degrees)

&nbsp;

<h2>Special Requirement: Sector</h2>
The Sector class will have a special requirement regarding handling of degrees/radians. The constructor should take in an angle in <strong>degrees</strong> and convert it to radians. This could be done using radians instead (or in addition to), but many math libraries will do this one of two ways, possibly both. There are <strong>2π radians in a circle</strong>, or 1 degree is equal to π/180.

<h2>3D Shapes</h2>
The 3D shapes will be a little different, partly due to how they will derive from the base classes. They will utilize <strong>multiple inheritance</strong>, and one of the base classes will derive using <strong>private inheritance</strong>.

<table width="0">
<tbody>
<tr>
<td width="160"><strong>Shape </strong></td>
<td width="247"><strong>Base classes </strong></td>
<td width="217"><strong>Volume </strong></td>
</tr>
<tr>
<td width="160">TriangularPyramid</td>
<td width="247">public Shape3D, private Triangle

It <em>IS A</em> Shape3D, and it <em>HAS A </em>triangle

(the triangle is at its base)

It has a private <u>height</u> variable
</td>
<td width="217">Volume = 𝐴ℎ

A = area of base (you can get this from the Triangle you inherit!)

h = height
</td>
</tr>
<tr>
<td width="160">RectangularPyramid</td>
<td width="247">It <strong>IS A</strong> Shape3D, and it <strong>HAS A</strong> rectangle

It also has a private height variable

&nbsp;

Note: length * width sounds like Area() too!
</td>
<td width="217">Volume = 𝑙𝑤ℎ

l = length of base

w = width of base h = height
</td>
</tr>
<tr>
<td width="160">Cylinder</td>
<td width="247">It is a Shape3D, and it has a circle It has a height (private) variable too!</td>
<td width="217">Volume = 𝜋𝑟<sup>2</sup>ℎ

r = radius h = height
</td>
</tr>
<tr>
<td width="160">Sphere</td>
<td width="247">It is a Shape3D, and it has a circle

It only needs the radius (private) of its circle to define its volume
</td>
<td width="217">4 Volume = &nbsp;𝜋𝑟<sup>3</sup>

3

r = radius

&nbsp;
</td>
</tr>
</tbody>
</table>
Because they inherit from Shape3D, you will have to implement the four functions required by the abstract base classes. In addition, each class should have:

<ul>
<li>A default constructor</li>
<li>A constructor which takes in a parameter for its main component (if it has one), and then anything its base class would need:</li>
</ul>
TriangularPyramid(height of the pyramid, length of its triangular base, height of its base [which is on the ground])

RectangularPyramid(pyramid height, length of its base, width of its base)

Cylinder(height of the cylinder, radius of its circle) Sphere(just a radius)

<h1>Abstract Base Class</h1>
An <strong>A</strong>bstract <strong>B</strong>ase <strong>C</strong>lass (<em>ABC</em>) is a class you never want to create an instance of; it doesn’t have enough information to be useful <strong>on its own</strong>. An ABC could have any number of functions or variables, whether public, protected, or private. You cannot create an instance of an abstract base class.

Perhaps you are creating a program that needs to store data about students and faculty members. They share similar data (name, age, email address, etc.), but have their own <strong>unique</strong> data as well. You might create 3 classes:

// Abstract class. “Just a Person” isn’t enough data&nbsp; class Person

class Student : public Person class Faculty : public Person

To create an abstract base class, at least one function in the class must be a <strong>pure virtual function</strong>. A pure virtual function is one that:

<ol>
<li>Have the virtual keyword before the return type</li>
<li>Has = 0 at the end of the prototype</li>
<li>Has no function definition (i.e. no body) – the only exception to this is the destructor. You MUST have a body on a destructor, pure virtual or otherwise virtual void Display() const = 0;</li>
</ol>
<h1>Multiple Inheritance</h1>
While many languages do not allow multiple inheritance, C++ does! The basic concept is the same. You have multiple base classes, and a single class can derive from some or all of them, inheriting the data members and functions of each base class.

<h1>The Diamond Problem</h1>
An issue with multiple inheritance is the dreaded “diamond problem.” This comes about when a derived class inherits from two base classes, which each derive from the same parent base class. Consider this:

&nbsp;

<h2>How to resolve the diamond problem</h2>
You can fix the issue of the diamond problem by using <strong>virtual</strong> inheritance. In the above example, the class declarations might look like this:

class Vehicle class Car&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : public Vehicle class Airplane&nbsp; : public Vehicle

class FlyingCar : public Car, public Airplane

With virtual inheritance, the “in-between” classes would add the virtual keyword to the inheritance:

class Car&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : virtual public Vehicle class Airplane : virtual public Vehicle

This ensures that FlyingCar would only inherit ONE instance of anything Car and Airplane inherited from Vehicle.

For more information:

<u><a href="https://en.wikipedia.org/wiki/Virtual_inheritance">https://en.wikipedia.org/wiki/Virtual_inheritance</a></u> <u><a href="https://isocpp.org/wiki/faq/multiple-inheritance#virtual-inheritance-where">https://isocpp.org/wiki/faq/multiple</a><a href="https://isocpp.org/wiki/faq/multiple-inheritance#virtual-inheritance-where">–</a><a href="https://isocpp.org/wiki/faq/multiple-inheritance#virtual-inheritance-where">inheritance#virtual</a><a href="https://isocpp.org/wiki/faq/multiple-inheritance#virtual-inheritance-where">–</a><a href="https://isocpp.org/wiki/faq/multiple-inheritance#virtual-inheritance-where">inheritance</a><a href="https://isocpp.org/wiki/faq/multiple-inheritance#virtual-inheritance-where">–</a><a href="https://isocpp.org/wiki/faq/multiple-inheritance#virtual-inheritance-where">where</a></u>

<h1>Public and Private Inheritance</h1>
Perhaps the most common type of inheritance is public inheritance. It represents an “is-a” relationship between classes.

The derived class is a base class.

For example:

class Car&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : public Vehicle class SavingsAccount : public BankAccount class Button&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : public UIControl

We would say that the Car (derived class) IS A Vehicle (base class). A SavingsAccount IS A BankAccount. A Button IS A UIControl, etc. If class inherits from another class using <strong>private</strong> inheritance, however, it models a “has a” relationship. This is also sometimes referred to as <strong>composition</strong>. For example:

// Private inheritance — the car “has a” Engine class Car : private Engine

&nbsp;

The only thing the Car class can access of the Engine object is <em>public</em> members and functions — here’s where the <em>accessor</em> functions of a class would come into play.

<h2>Accessing members of base class(es)</h2>
To access the functions or variables of a base class, you must specify the name of the class, and then the thing you are trying to access. So in the case of the car and its engine, you would do something like this: void Car::SomeFunction()

{

string maker = Engine::GetManufacturer(); }

Reference: <u>https://isocpp.org/wiki/faq/private-inheritance</u>

<h1>Polymorphism</h1>
One important concept in object-oriented programming is that a <strong>base-class pointer</strong> can point to any object which <strong>derives</strong> from that base class. For example:

class Car{}; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; // Base class

class Mustang : public Car{};&nbsp;&nbsp; // Derived class

&nbsp;

// Set a base class pointer to an instance of the derived class Car *someCar = new Mustang; // Valid due to inheritance

Following that same concept, we could extend that to something like the following:

Car *cars[3]; cars[0] = new Car; cars[1] = new SportsCar; cars[2] = new LuxurySedan;

&nbsp;

What polymorphism allows you to do is call a function from one of those objects and <strong>depending on what the pointer is pointing to</strong> the correct function will be called.

class Car { public:

virtual void Identity()&nbsp; &nbsp; { cout &lt;&lt; “I’m just a car!”; }

};

class SportsCar : public Car { public:

void Identity()

{ cout &lt;&lt; “I’m a sports car!”; }

};

class LuxurySedan : public Car { public:

void Identity()

{ cout &lt;&lt; “I’m a luxury car!”; }

};

&nbsp;

Given the previous array, a line of code like the following would print out “I’m a sports car!”:

cars[1]-&gt;Identity(); // cars[1] points to a SportsCar

Polymorphism is the concept that allows you to write code like that, without knowing exactly what type of object you are pointing to. Since cars[1] points to a SportsCar, the call to Identity() will determine that the SportsCar version of the function should be used. The <strong>virtual</strong> keyword is required on the base class version of the function in order to make this functionality possible.

For more on polymorphism: <u><a href="http://www.cplusplus.com/doc/tutorial/polymorphism/">http://www.cplusplus.com/doc/tutorial/polymorphism/</a></u>

<h1>Bringing it all together</h1>
While it may seem like a lot of work to create such simple classes, once this framework is in place, you can very easily modify the class hierarchy with minimal effort (such as changing code elsewhere). Consider the following code:

&nbsp;

Shape *shapes[] =

{&nbsp; &nbsp; new Square(2.4f),&nbsp; &nbsp; new Rectangle(3, 5),&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; new Triangle(4.2f, 6),&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; new Circle(2),&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; new Trapezoid(2, 6, 2.3f),

new Sector(2, 35)

};&nbsp; float area = 0.0f; for (int i = 0; i &lt; 6; i++)&nbsp; area +=shapes[i]-&gt;Area(); // Mix 2D and 3D shapes

Shape *shapes[] = {&nbsp;&nbsp;&nbsp; new Circle(3.02f),&nbsp;&nbsp;&nbsp; new TriangularPyramid(4.5f, 1, 4),&nbsp;&nbsp;&nbsp; new Sector(3, 18),&nbsp;&nbsp;&nbsp; new RectangularPyramid(3.23f, 2, 3)&nbsp;&nbsp;&nbsp; new Trapezoid(2, 6, 2.3f),

};

for (int i = 0; i &lt; 5; i++)

{&nbsp; &nbsp; shapes[i]-&gt;Display();

cout &lt;&lt; endl;

}

&nbsp;

&nbsp;

Nowhere in the loops is there any code checking the types of the objects (Shape2D, Shape3D, it doesn’t matter). It simply uses a function, and because of inheritance, polymorphism, and virtual functions, each object behaves as it should. In this particular case the behavior of each object is simple, and very similar, but this concept allows us to change any individual object’s behavior, without modifying the code you see here. And if you were to write a function like this: void SomeFunction(vector&lt;Shape *&gt; shapes)

{

for (unsigned int i = 0; i &lt; shapes.size(); i++)

shapes[i]-&gt;Display();

}

You can further reduce the amount of information you need to have in order to write your code. How many objects are in the shapes vector? The size() function will tell us. What shapes, exactly, are in that vector? Don’t need to know, don’t need to care. The importance of this concept, of working with objects, <strong>WITHOUT KNOWING ALL OF THAT OBJECT’S DETAILS</strong>, cannot be overstated. Many things you will work on later in your programming career will rely on this concept.

<h1>Tips</h1>
A few tips about this assignment:

<ul>
<li>Start with one class at a time. Since Square derives from Shape2D, which derives from Shape… start with the Shape class first. Then Shape2D, then Square, then all the other 2D shapes.</li>
<li>Similarly, if a class like TriangularPyramid derives from both Shape3D and Triangle, it’s probably a good idea to complete those classes first.</li>
<li>If you want to add any other functionality to these classes in order to help you get the job done, do it! Helper functions, constant values (pi, degrees to radian conversions, etc), go for it! The interface of the class indicates  <strong><u>what</u></strong> it can do. It says nothing about <strong><u>how</u></strong> that gets done.</li>
</ul>
<h1>Sample Output</h1>
2D Shapes:

&nbsp;

3D Shapes:

&nbsp;
