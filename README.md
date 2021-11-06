# Unit Testing

 This code will create a task to run unit tests on two functions: adcResToVoltageWhole and adcResToVoltageFrac.
 The Units Under Test are:
 adcResToVoltageWhole() which determines whole number part of voltage value corresponding to ADC result, and
 adcResToVoltageFrac() which determines fractional part of voltage value corresponding to ADC result.

# Important Files

 Source file: main/user_main.c,
 Output file: main/lab3_q1_816005001.out,
 Binary file: build/i2c.bin

# Test file

 There is no explicit test file. The unit_test_task in main/user_main.c does the job of a test driver in this code.

# Pin Assignment

 N/A

# Hardware Required

 None

# Example Output  

```

I () main: Unit testing task
I () main: UUTs: adcResToVoltageWhole(), adcResToVoltageFrac()
I () main: adcResToVoltageWhole() determines whole number part of voltage value corresponding to ADC result
I () main: adcResToVoltageFrac() determines fractional part of voltage value corresponding to ADC result

I () main: Test case 1: ADC result: 0x0 [0]
I () main: Expected output > Whole: 0, Fraction: 0 / 16000
I () main: Output > Whole: 0, Fraction: 0 / 16000

I () main: Test case 2: ADC result: 0xa [10]
I () main: Expected output > Whole: 0, Fraction: 10 / 16000
I () main: Output > Whole: 0, Fraction: 10 / 16000

I () main: Test case 3: ADC result: 0x5e1f [24095]
I () main: Expected output > Whole: 1, Fraction: 8095 / 16000
I () main: Output > Whole: 1, Fraction: 8095 / 16000

I () main: Test case 4: ADC result: 0x6c1f [27679]
I () main: Expected output > Whole: 1, Fraction: 11679 / 16000
I () main: Output > Whole: 1, Fraction: 11679 / 16000

I () main: Test case 5: ADC result: 0xffff [65535]
I () main: Expected output > Whole: 4, Fraction: 1535 / 16000
I () main: Output > Whole: 4, Fraction: 1535 / 16000


```
