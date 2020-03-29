# __Spring Core By Udemy__  

## _Q1:_ What is dependency Injection and what are there uses ?  
Answer::  
When you write any code and you are creating any object inside that code you are dependent on that object/class means if the same work you require to do in another way you require to change in code or
the class which is creating that objects. Now how you can handle this situation ? if you pass object in cunstructor of class from outside then it is not dependent on that object and you can easly anyone
can use that class according to its requirement and also in test cases you can pass mock from outside.  
For Example please have a look on GitRepo:


## _Q2_: What is pattern and how it will help in Spring(DI)?    
Answer::  
Pattern is a way to solve a well known problem statement in a specific way which is developed/find by many other developers over the time. This is a well known and eddicient way to solve this problem.
There are numbers of pattern which are also divided in diffrent groups, this is a seprate talk and require a lot of time.DI is also a pattern and well known way to apply. There are alo anti pattern which are just opposite of this.  

## _Q3_: What is interface and how it is very important for DI? 
Answer::  
In point of java it a collection of __abstract function__ and use as a contract for those class which implement them. Interface fouce a class to define all functions which are define in interface.
This is very usefull for testing and interchangebility.   
In pont of Spring it allow JDK dynamic proxy, Implimentation hiding (No class is public only the interface is public and you can you that only), Easy to switch beans (This is DI, In class you make a ref
of a interface and then you pass implimented class(beans) from outside . __DI__)   
For Example please have a look on GitRepo:  

## _Q4_: What is Application Context ?  
Answer::  
__Application Context__ is central part of Spring, this is rewsponsible for may things like   
* initating Beans  
* configure beans  
* Assemble beans  
* Manage bean life cycle  

This means bean related all things are handle by Application context and this is also responsible for _BeanFactory, resource loader, Event registered and listners and property resolver_.  Application ctx
require configuration for beans knowns as metadata which is mainly provideed by xml, annotation and java code, On basis of this it is divided in areas.  
There are diffrent type of Context in Spring:-  

* __AnnotationConfigApplicationContext__ : In this we provide configuration by annotation.  
* __AnnotationConfigWebApplicationCtx__ : In this we provide config by annottion but for web application not standart application.  
* __ClassPathXmlApplicationCtx__ : This is where you provide config by xml file present in classpath only.  
* __FileSystemXmlAWpplicationCtx__ : This is where you provide config by providing config using xml which is present any where in file system.  
* __XmlWebApplicationCtx__ : This is for web application in which config provided by xml.  


## _Q5_: What is container and its life cycle?  
Answer::  
Let take a Example, if have to make a rest API then you have to configure every thing foe http, sest and other thing but if you get a environment where you get all configuration setup by default and 
you only require write bussiness logic that is good one. This is container, you can read more in docker or contaier concept sepratly.  
Life Cycle of Container in Spring::  
* Application Started  
* Spring Container Created  
* Container Read Config  
* Beans created from config  
* Post Process for modify bean run  
* Bean Created ( still no property value set)  
* Bean dependency injected  
* Post processor  
* Run time  
* Application shutdown  
* Ctx Close  
* dstruction method call  

