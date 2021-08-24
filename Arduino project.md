int GREEN = 2;<br>
int YELLOW = 3;<br>
int RED = 4;<br>
int DELAY_GREEN = 5000;<br>
int DELAY_YELLOW = 2000;<br>
int DELAY_RED = 5000;<br>
void setup()<br>
{<br>
  pinMode(GREEN, OUTPUT);<br>
  pinMode(YELLOW, OUTPUT);<br>
  pinMode(RED, OUTPUT);<br>
}<br>
void loop()<br>
{<br>
  green_light();<br>
  delay(DELAY_GREEN);<br>
  yellow_light();<br>
  delay(DELAY_YELLOW);<br>
  red_light();<br>
  delay(DELAY_RED);<br>
}<br>
void green_light()<br>
{<br>
  digitalWrite(GREEN, HIGH);<br>
  digitalWrite(YELLOW, LOW);<br>
  digitalWrite(RED, LOW);<br>
}<br>

void yellow_light()<br>
{<br>
  digitalWrite(GREEN, LOW);<br>
  digitalWrite(YELLOW, HIGH);<br>
  digitalWrite(RED, LOW);<br>
}<br>

void red_light()<br>
{<br>
  digitalWrite(GREEN, LOW);<br>
  digitalWrite(YELLOW, LOW);<br>
  digitalWrite(RED, HIGH);<br>
}<br>
