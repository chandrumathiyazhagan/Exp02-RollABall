# Exp02-RollABall
## Aim :
To develop a 3D application for RollABall in unity.
## Algorithm:
### Step1 :
Create a new project.

### Step 2 :
Click Heirarchy -> 3D object -> Select the plane -> 3DObject -> Sphere.

### Step 3 :
Define the physics properties of the surface (Rigidbody).

### Step 4 :
Assets -> Create -> # Script

### Step 5 :
Create a folder name Coding and create a C# file to add the coding in it.

### Step 6 :
To add our C# Script file to our selected object, click on the C# Script file and drag it to our selected objects in the Hierarchy window nad run the application.

### Step 7 :
Stop.

## Program:

### Developed by :M.Chandru

### Register Number:212222230026

```python
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class roll : MonoBehaviour
{
    public float xForce = 5.0f;
    public float zForce = 5.0f;
    public float yForce = 200.0f;
    void Update()
    {
        float x = 0.0f;
        if (Input.GetKey(KeyCode.A))
        {
            x = x - xForce;
        }
        if (Input.GetKey(KeyCode.D))
        {
            x = x + xForce;
        }
        float z = 0.0f;
        if (Input.GetKey(KeyCode.S))
        {
            z = z - zForce;
        }
        if (Input.GetKey(KeyCode.W))
        {
            z = z + zForce;
        }
        float y = 0.0f;
        if (Input.GetKeyDown(KeyCode.Space))
        {
            y = y - yForce;
        }
        GetComponent<Rigidbody>().AddForce(x, y, z);
    }
}
```
## Output:

![Screenshot 2024-03-06 201020](https://github.com/chandrumathiyazhagan/Exp02-RollABall/assets/119393023/0ce9e909-c0a8-46ec-986c-fa92d538e93b)

## Result:
Thus a 3D application for RollABall objects in unity is developed successfully.
