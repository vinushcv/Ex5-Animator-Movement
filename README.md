# Ex5-Animator-Movement
## Aim:
To develop a animator movement for a player using unity.

## Algorithm:
### Step 1:
Import necessary models.

### Step 2:
Right-click -> Create -> Animator Controller.

### Step 3:
Open Animator window, define states (Idle, Run, Jump, etc.).

### Step 4:
Use keyframes or Unity's Animation tools to animate transitions between states.

### Step 5:
Drag Animator Controller to the GameObject in the Inspector.

## Program:
Name: Vinush.CV

Reg no: 212222230176

```c#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class NewBehaviourScript : MonoBehaviour
{
    // Start is called before the first frame update
    public Animator animator;
    public float InputX;
    public float InputY;
   
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();
    }

    // Update is called once per frame
    void Update()
    {
  
        InputY = Input.GetAxis("Vertical");
        InputX = Input.GetAxis("Horizontal");
       
        animator.SetFloat("InputY", InputY);
        animator.SetFloat("InputX", InputX);
    }

```

## OUTPUT:

![image](https://github.com/vinushcv/Ex5-Animator-Movement/assets/113975318/d201c3ca-9268-4255-8d78-eb85701b0cc5)


## RESULT:
An animator movement for a player using unity is developed successfully.

