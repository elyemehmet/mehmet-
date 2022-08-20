using System.Collections;
using System.Collections.Generic;
using UnityEngine;
using UnityEngine.InputSystem;

// Takes and handles input and movement for a player character
public class PlayerMovement : MonoBehaviour
{
    public CharacterController controller;
    Vector3 direction;
    public float speed = 8;


    private void Update()
    {
        float hInput = Input.GetAxis("Horizontal");
        float yInput = Input.GetAxis("Vertical");
        direction.x = hInputspeed;
        direction.y = yInput speed ;
        controller.Move(direction*Time.deltaTime);

    }
}
