# Toggle-Switch-use-on-Jetson-Nano

> TOGGLE SWİTCH  USING ON JETSON NANO


Jetson is not connected to nano as the toggle switch is connected to arduino or cannot read data. today i will show you how to use toggle switch on jetson nano


First, let's draw our circuit from the fritzing program.

![CONNECTİONS](https://github.com/ElectronicEngineerr/Toggle-Switch-use-on-Jetson-Nano/blob/main/Untitled%20Sketch%202_bb.png)


Now I write a simple code in the python compiler in jetson nano, let's learn to get 0 and 1

After installing the sdk manager in Jetson nano, we will import the `Jetson.GPIO` library that comes as the default library.
` import Jetson.GPIO as GPIO`

Some setup is required to use the Jetson.GPIO library, let's add it to our python compiler and choose a GPIO pin for a toggle switch. I chose pin 15
`toggle_switch = 15`
` GPIO.setmode(GPIO.BOARD) `
` GPIO.setup(15, GPIO.IN) `
` GPIO.setwarnings(False) `

 After the necessary installations, you can open a while true command and find the status of the toggle switch easily with if , elif and else commands. but after opening while true, you should write ' switch_state = GPIO.input(15)' on the next line without writing the if variable





