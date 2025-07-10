# Squirrel With Inputs
A small C code modification to the Squirrel 3.2 Standard Library that enables scanning user input as strings. This is very experimental, and i recommend not taking it too seriously.

## Usage
The only function introduced is `scanline()`, which reads user input and converts it into a string of up to 255 characters.

Trailing characters will simply be ignored.

```squirrel
print("Say something: ");
message <- scanline();

printf("The user said: %s\n", message);
```

Optionally, you may also parse a string as an argument to instantly print it to the terminal, pretty much like the `input()` function in Python.

```squirrel
message <- scanline("Say something: ");

printf("The user said: %s\n", message);
```

## Building
See [COMPILE](/COMPILE).

