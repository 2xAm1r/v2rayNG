vmess://eyJhZGQiOiJ2aXBnci5hbWlyaXguc2JzIiwiYWlkIjoiMCIsImFscG4iOiIiLCJmcCI6IiIsImhvc3QiOiJ0ZWxld2ViaW9uLmNvbSIsImlkIjoiMTRlYWE3YmItYjViNy00ODk5LWExMGMtNjFmMDZkM2VhNWE2IiwibmV0IjoidGNwIiwicGF0aCI6Ii8iLCJwb3J0IjoiMzM5MzQiLCJwcyI6IkFtaXIiLCJzY3kiOiJhdXRvIiwic25pIjoiIiwidGxzIjoiIiwidHlwZSI6Imh0dHAiLCJ2IjoiMiJ9

۸/*
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

  // Open cmd
  delay(2000);

  Keyboard.press(KEY_LEFT_GUI);
  Keyboard.press('r');
  Keyboard.releaseAll();

  delay(2000);

  Keyboard.print("cmd");

  delay(500);

  typeKey(KEY_RETURN);

  delay(500);

  Keyboard.print("ipconfig");

  typeKey(KEY_RETURN);

  delay(1000);

  Keyboard.print("Hi ... IM SECBAZ!");

  // Ending stream
  Keyboard.end();
}

/* Unused endless loop */
void loop() {}








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

  delay(3000);

  Keyboard.press(KEY_LEFT_GUI);
  Keyboard.press('r');
  Keyboard.releaseAll();

  delay(200);

  Keyboard.print("https://www.youtube.com/watch?v=dQw4w9WgXcQ");

  typeKey(KEY_RETURN);

  delay(3000);

  Keyboard.print("reza");

  // Ending stream
  Keyboard.end();
}

/* Unused endless loop */
void loop() {}
