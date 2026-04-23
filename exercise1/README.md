compile
```sh
javac BookingFormGUI.java BookingForm.java
```

run
```sh
java BookingFormGUI
```

make the fuzzer and run it
```sh
javac -d out BookingForm.java fuzzer.java
chmod +x ./jazzer/jazzer
./jazzer/jazzer --cp=out --target_class=fuzzer
```

! remember: the speed and wheather getting a result at all depends on randomness of some seed the fuzzer uses or auto-picks.
