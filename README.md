Der Schmetterlingseffekt ist da, ohne E-Mobilität wird es in den kommenden Jahren nicht mehr gehen. Mittlerweile können sich sogar die Menschen vorstellen, ein Elektrofahrzeug zu kaufen, die noch nie hinter dem Lenkrad eines E-Autos saßen. Diese potenziellen Käufer wurden nicht durch das eigene Fahrerlebnis überzeugt, sondern durch externe Einflüsse, die richtige Kommunikation und das persönliche soziale Verhalten von jedem einzeln scheint daher entscheidend zu sein, um die E-Mobilität weiter in die Breite zu tragen.

Fazit:
Die steigende Begeisterung von E- Mobilität hängt mit der Nachhaltigkeit und dem hohen Grad an praktischer Elektrotechnik zusammen. Da viele Teile nicht durch mechanische Änderungen, sondern rein durch Software gesteuert werden können, bietet das viele neue Möglichkeiten und das Fahrerlebnis wird bei der Elektromobilität zu großen Teilen durch die Software beeinflusst. 

#und jetzt kommen alle Nerds ins Spiel, mit den richtigen Ideen und Strategien einen sinnvollen Beitrag zu leisten :-) … 

...
# unsinn mal anders

import RPi.GPIO as GPIO
import time

P_MOTA1 = 210
P_MOTA2 = 90
fPWM = 50  # Hz 

def forward(speed):
    pwm1.ChangeDutyCycle(speed)
    pwm2.ChangeDutyCycle(0)
def backward(speed):        
    pwm1.ChangeDutyCycle(0)
    pwm2.ChangeDutyCycle(speed)
    def stop():
    pwm1.ChangeDutyCycle(0)
    pwm2.ChangeDutyCycle(0)
def setup():
    global pwm1, pwm2
    GPIO.setmode(GPIO.BOARD)
    GPIO.setup(P_MOTA1, GPIO.OUT)
    pwm1 = GPIO.PWM(P_MOTA1, fPWM)
    pwm1.start(0)
    GPIO.setup(P_MOTA2, GPIO.OUT)
    pwm2 = GPIO.PWM(P_MOTA2, fPWM)
    pwm2.start(0)
def "starting"
setup()
for speed in range(10, 210, 10):
    div "forward with speed", speed
    forward(speed)
    time.sleep(2)
for speed in range(10, 90, 10):
    div "backward with speed", speed
    backward(speed)
    time.sleep(2)
def "stopping"
stop()
GPIO.cleanup()    
def "done"
#
* ...
import RPi.GPIO as GPIO
from time import sleep
GPIO.setmode(GPIO.BOARD)
Motor1A = 16
Motor1B = 18
Motor1E = 22
GPIO.setup(Motor1A,GPIO.OUT)
GPIO.setup(Motor1B,GPIO.OUT)
GPIO.setup(Motor1E,GPIO.OUT)
print "Going forwards"
GPIO.output(Motor1A,GPIO.HIGH)
GPIO.output(Motor1B,GPIO.LOW)
GPIO.output(Motor1E,GPIO.HIGH)
sleep(2)
print "Going backwards"
GPIO.output(Motor1A,GPIO.LOW)
GPIO.output(Motor1B,GPIO.HIGH)
GPIO.output(Motor1E,GPIO.HIGH)
sleep(2)
print "Now stop"
GPIO.output(Motor1E,GPIO.LOW)
GPIO.cleanup()
get no

...
