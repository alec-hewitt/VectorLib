Alec Hewitt 2015

# VectorLib
A compact utility library in C++ for dealing with 3D vectors and linear algebra.

VectorLib is a C++ library used to handle 3D vectors and linear algebra.

To use in your projects, just include the header file.

The library currently contains a cpp and header file which define the Vector4 object.

The class allows vector addition subtraction multiplication and division with other vectors
and scalars.

Includes a setter and getter function which each return scalars for independant axis' within the vector object.

Linear algebra is handled, including polar and cartesian conversions, and basic vector arithmatic. In the future, the class will handle conversions to other magnitude and direction
descriptors. 

#HOW-TO
###Operators
Create a Vector object.

>Parameters consist of magnitudes on each axis
```
Vector4 vectorName(x, y, z);
```

Add two Vector objects

>Adds the x, y, and z components of another Vector
```
vectorOne = vectorOne + vectorTwo;
```

Subtract two Vector objects

>Subtracts the x, y, and z components of another Vector
```
vectorOne = vectorOne - vectorTwo;
```

Divide two Vector objects

>Divides the x, y, and z components of another Vector
```
vectorOne = vectorOne / vectorTwo;
```

Multiplies a Vector object by a scalar

>Multiplies the x, y, and z components of the Vector by a scalar
```
vectorOne = vectorOne * 15;
```

Multiplies two Vectors with cross product

>Calculates the vector cross product of two vectors
```
vectorOne = vectorOne * vectorTwo;
```

###Functions

set(float newX, float newY, float newZ)
>Sets the axis components of the vector
```
vectorOne.set(scalarOne, scalarTwo, scalarThree);
```

reset();
>Resets all vector components to zero
```
vectorOne.reset();
```

polarToCartesian(float magnitude, Vector4 direction);
>Converts a polar description of magnitude and direction to a vector object
```
Vector4 cartesian = polarToCartesian(scalarOne, vectorOne)
```

getMagnitude(Vector4 vector);
>Calculates the magnitude scalar of a vector object
```
float unitVector = getMagnitude(vectorOne);
```

scaledVector(float magnitude, Vector4 direction);
>Scales a unit vector of given direction Vector by a given magnitude
```
Vector4 scaledVec = scaledVector(scalarOne, vectorOne);
```
