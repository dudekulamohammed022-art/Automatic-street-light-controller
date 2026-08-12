# Automatic-street-light-controller
// code \\
int ldrPin = A0;
int ledPin = 8;

int ldrValue = 0;
int threshold = 500;

void setup()
{
  pinMode(ledPin, OUTPUT);
  Serial.begin(9600);
}

void loop()
{
  ldrValue = analogRead(ldrPin);

  Serial.println(ldrValue);

  if (ldrValue < threshold)
  {
    digitalWrite(ledPin, HIGH);
  }
  else
  {
    digitalWrite(ledPin, LOW);
  }

  delay(500);
}



##circuit diagram ##

<img width="1706" height="713" alt="Surprising Albar" src="https://github.com/user-attachments/assets/c336b8b6-ace5-4cab-8314-77db6222e8d9" />
## Tinkercad share link ##
https://www.tinkercad.com/things/2NCUyRZjw5F/editel?returnTo=%2Fdashboard
