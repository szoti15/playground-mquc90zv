# Object-Oriented Programming Concepts


Objects share two characteristics: they all have state and behaviour:
+ stores the state in fields
+ exposes its behaviour through methods: operate in an object's internal state and serve as the primary mechanism for object-to-object communication

Class: a generic model, the blueprint of the real life things from which individual objects are created.

``` java
public class Animal {
    int avarageLifetime;        //in years
    float height;
    float weight;
    
    public Animal breed(Animal otherEntity){
        return new Animal();
    }
}
```

The example above is a class that represents animals.
By modelling ***Animal*** we try to collect every attributes (fields) and every behavioral things (methods) that can be useful for us and can be applicable to every animals in general.
It has 3 fields `avarageLifeTime`, `height`, `weight` and a method `breed`.

From this blueprint you can create an exact instance of an ***Animal*** e.g. your dog, with his avarageLifetime 11 years, his height 35.56 cm and his weight 10.7 kg. We call these instances `object`.


//TODO: bytecode
//TODO: multiplatform
//TODO: gc

