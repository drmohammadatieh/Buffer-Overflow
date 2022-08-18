### Buffer Overflow in C

This is a buffer overflow in C exercise as part of the secure software development (SSD) module at the University of Essex Online.

## Compile and run

First, the code is compiled using a command terminal after navigating to the directory that contains the buffer_overflow.c as the following:

```
gcc buffer_overflow.c -o buffer_overflow

```
Then compiled code is run using the following command:

```
.\buffer_overflow

```

## Output

Output after a "shorttext" input:

```
Enter name: shorttext
shorttext
zsh: abort      ./buffer_overflow

```
Output after "thisisaverylongtext" input where the size exceeds the size of the buffer

```
Enter name: thisisaverylongtext
thisisaverylongtext
*** stack smashing detected ***: <unknown> terminated
Aborted (core dumped)

```

This "stack smashing detected" message means that the GNU Compiler Collection (GCC) has detected a buffer overflow problem.


### Buffer Overflow in Python

This is a comparison to the work that was done in C.

First, running the following code using ```python buffer_overflow``` command:

```
buffer=[None]*10 

for i in range (0,11): 

    buffer[i]=7 

print(buffer) 
```

## Output

```
IndexError: list assignment index out of range

```

## Pylint

After that the Pylint was installed using the following command:

```
pip install pylint

```


## Running pylint on the buffer_overflow.py 







