Der Schmetterlingseffekt ist da, ohne E-Mobilität wird es in den kommenden Jahren nicht mehr gehen. Mittlerweile können sich sogar die Menschen vorstellen, ein Elektrofahrzeug zu kaufen, die noch nie hinter dem Steuer eines E-Autos saßen. Diese potenziellen Käufer wurden nicht durch das eigene Fahrerlebnis überzeugt, sondern durch externe Einflüsse, die richtige Kommunikation und das persönliche Sozialverhalten von jedem einzeln scheint daher entscheidend zu sein, um die E-Mobilität weiter in die Breite zu tragen.

Fazit:
Die steigende Begeisterung von E- Mobilität hängt mit der Nachhaltigkeit und dem hohen Grad an praktischer Elektrotechnik zusammen. Da viele Teile nicht durch mechanische Änderungen, sondern rein durch Software gesteuert werden können, bietet das viele neue Möglichkeiten für IT-Fans und das Fahrerlebnis wird bei der Elektromobilität zu großen Teilen durch die Software beeinflusst. 

#jetzt kommen die Nerds ins Spiel, mit den richtigen Ideen und Strategien  :-) … 

... 

*vrorofhöfhrghrhrefkdvf
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
