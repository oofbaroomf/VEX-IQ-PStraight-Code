# VEX-IQ-PStraight-Code
Basic P-Control Guide (VEX IQ)
This block of code helps your robot drive straight using just the Proportional Control (P Loop). It uses the gyro sensor. This was used by team 13765D MAVER1CKS.
**How It Works:**
1. Reset Motor Positions
 - Sets both motor positions to 0 degrees at the start
2. Forward or Backward Check
 - If velocity > 0, it just drives forward (the grey block is just a comment, you don’t need anything there)
 - If velocity < 0, it uses a P loop to drive straight.
3. While Loop
 - Keeps checking average distance ((left + right)/2) until it reaches the target.
 - Calculates error = desired heading - current heading using the gyro.
**In this code, these are the variables used.**
_**    - distance: Target distance in degrees.
    - heading: Desired heading in degrees (irrelevant for p straight).
    - velocity: Speed (%)
    - kp: Tuning constant. Start with 1–2 and test, this will be different for different robots. **_
**Tips:**
 - Tune kp until the robot drives straight with minimal wiggle.
 - DM me on discord (ast1) if you need any help, or want a more complex but more accurate code that uses a distance sensor as well as brain inertial.
