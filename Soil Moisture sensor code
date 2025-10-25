// Soil Moisture Sensor Basic Code

const int sensorPin = A0; // Analog pin connected to sensor
int sensorValue = 0;

void setup() {
  Serial.begin(9600);    // Start serial communication
  Serial.println("Soil Moisture Sensor Started...");
}

void loop() {
  sensorValue = analogRead(sensorPin); // Read analog value (0-1023)
  
  Serial.print("Soil Moisture Value: ");
  Serial.println(sensorValue);

  // Optional: interpret moisture level
  if(sensorValue > 700) {
    Serial.println("Soil is Dry");
  } else if(sensorValue > 300) {
    Serial.println("Soil is Moist");
  } else {
    Serial.println("Soil is Wet");
  }

  delay(2000); // Read every 2 seconds
}
