### In Vivado suite
1. Click on create project .
2. Select RTL Project and click next.
3. Select Target Lang :Verilog and click next.
4. Click next
5. Choose the following settings for our Minized 7Z007

![1](https://user-images.githubusercontent.com/68508872/130557876-6df94117-0794-4398-9189-c28229549066.jpg)

6. Finish



### Under IP Integrator:
1. Create Block Design ,Choose project name and OK
2. In the Digram box ,Add a IP name "ZYNQ7 Processing system"
3. Click on "run block automation" and click ok
4. Double Click on your block diagram to recustomize your IP
5. In PS-PL configration ->AXI Non Secure Enablement->GP master AXI interface->M AXI GP0 interface should be unchecked.
6. In MIO configration ->I/O peripherals->check UART-1
7. In DDR configration->DDR Controller Config->Memory Type->choose DDR3(LOW VOLTAGE) 
8. In DDR configration->DDR Controller Config->Memory Part->choose MT41K256M16 RE-125
9. In DDR configration->Training/Board details->DQS to clock delay(ns)->change DQS0 and DQS1 to 0.054
10. In DDR configration->Training/Board details->Board Delay->DQ[7:0] and DQ[15:8] =0.234 and DQ[23:16] and DQ[31:24]=0.1
11. Click OK 
8. Click on "validate design"
9. In Source Tab ->Design sources ->(filename).bd->right click and click on CREATE HDL WRAPPER and click Ok.
10. In Program and Debug->Generate Bitstream and few min click OK.
11. Then click On File ->Export HW (Check Include Bitstream).
12. Now Launch SDK
