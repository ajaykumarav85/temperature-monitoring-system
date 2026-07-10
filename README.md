#define LM35 A0
#define RED 7
#define GREEN 6

void setup() {
  Serial.begin(9600);

  pinMode(RED, OUTPUT);
  pinMode(GREEN, OUTPUT);
}

void loop() {
  // Read analog value from LM35
  int sensorValue = analogRead(LM35);

  // Convert to temperature in Celsius
  float temperature = (sensorValue * 5.0 * 100.0) / 1023.0;

  // Display temperature on Serial Monitor
  Serial.print("Temperature: ");
  Serial.print(temperature);
  Serial.println(" °C");

  // LED indication
  if (temperature >= 60.0) {
    // High temperature
    digitalWrite(RED, HIGH);
    digitalWrite(GREEN, LOW);
  } else {
    // Normal temperature
    digitalWrite(RED, LOW);
    digitalWrite(GREEN, HIGH);
  }

  delay(500);
}
