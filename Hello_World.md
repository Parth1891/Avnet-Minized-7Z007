## SDK

### HELLO WORLD PROGRAM ON SDK TERMINAL
1. Once HW is generated ,under File -> Create BSP->Finish (Note in BSP setting choose stdin and stout according to your UART settings).
2. Create Application Project and choose "existing bsp" created .
3. Choose "Hello World" Template and Click Finish.
4. Under Application project (filename) created ,go to src code "HelloWorld.c".
5. Keep Board In JTAG MODE
6. Now ,connect your minized board to the laptop.
##### Note: SDK Terminal Setup:
      In SDK Terminal->Add(Green plus)->choose serial port in which minized is connected(ttyUSB1 for linux)
7. Right click on App project->Run As->Launch On HW
