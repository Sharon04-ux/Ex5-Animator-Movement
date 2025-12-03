# Ex5-Animator-Movement

## Aim :

To develop a animator movement for a player using unity.

## Algorithm :

## Step 1 : 

Import necessary models.

## Step 2 : 

 Right-click -> Create -> Animator Controller.

## Step 3 : 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4 : 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5 : 

Drag Animator Controller to the GameObject in the Inspector.

## Program :

### DEVELOPED BY : ADHARSH VIDYARDH U
### REG NO : 212224230007
PlayerController:


```c#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class script : MonoBehaviour
{
    public Animator animator;
    public float inx;
    public float iny;

    
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();
    }

    void Update()
    {
        inx = Input.GetAxis("Horizontal");
        iny = Input.GetAxis("Vertical");
        animator.SetFloat("inx",inx);
        animator.SetFloat("inY",iny);
    }
}
```
## Output :

<img width="1261" height="790" alt="image" src="https://github.com/user-attachments/assets/1838f97c-fb53-476f-84c9-e9808bc27d55" />




## Result :

An animator movement for a player using unity is developed successfully.
