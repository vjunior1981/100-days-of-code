# Annotations day 002

- Sooooooooo... decided do change back to **Python**;
- Why? Best training material, most accepted in the market, more stable and reliable;
- I'm using again an Udemy training, by KodeKloud. You can check it [here](https://www.udemy.com/course/python-entry-level-programmer-certification-pcep/)
---

- First function and program as always:

```python
print("Hello World!")
```

- Print is a builtin python function;
- You can use more functions from other modules;
- Function execution steps:
  - Checks function name;
  - Checks arguments passed;
  - Jumps into the function;
  - Executes the function;
  - Returns to your code;
  - Resumes execution;
- Some python keyword arguments

```python
# end: will change the default termination char (\n)
# for what is inside the quotes
print("Hello World", end="--");\
print("Python is a great language")
Hello World--Python is a great language

# sep: will change the default separator char (<space>)
# for what is inside the quotes
print("Python", "is", "a", "great", "language", sep="||");
Python||is||a||great||language
```

- About literals, 4 types:
  - Integers (Number without a fraction: 200, 123456, -90, 1_000_000 (you can use _ to make easier a number identification)
    - Octal numbers
      - 0o123
      - Calculating octal numbers:
        ```
        # First assign a value for each number, from the right, starting in zero
         "2" "1" "0"
          1   2   3

        # Now we calculate 8 to the value of this powers
           2   1   0
          8   8   8
        =64  =8  =1

        # Finally we multiply the result of the previously calculated numbers,
        # with the numbers of actual number (0o123)
        1 x 64 = 64
        2 x 8  = 16
        3 x 1  =  3

        # and finally:
        64 + 16 + 3 = 83
        ```

    - Hexadecimal numbers
      - 0x123
      - Calculating hexadecimal numbers:
        ```
        # Do the same as octals, but use base 16
        ```

  - Floating point numbers
  - Strings
  - Booleans
