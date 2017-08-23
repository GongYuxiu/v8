# about shell.cc
Some api interface for stdio like: cin, cout, scanf and printf.

# api
*   gets(size)
    read number of size characters from stdin, or util meets \n. \n may in the return string.
*   printsth(sth, ...)
    display sth in stdou, if there are more than on args, the diaplay split by " ", in the end there is no '\n'.
*   print(sth, ...)
    display sth in stdou, if there are more than on args, the diaplay split by " ", in the end there is a '\n'.
*   readInt()
    read a int or long number from stdin.
*   readDouble()
    read a float or double number from stdin.
* read_line
    read number of 1024 characters from stdin, or util meets \n. \n may in the return string.

# use examples
```js
function test() {
    printsth('This output is from nodecmd interface:\n');
    printsth(1234567890.123);
    printsth('\n');
    printsth('Hello workd.');
    printsth('\n');

    print('Please input 10 characters:');
    print(gets(10));

    printsth('Please input something:\n');
    var input = read_line();
    printsth('Your input is:\n');
    printsth(input);
    printsth('\n');

    print('Please input a int:');
    print(readInt());

    print('Please input a double:');
    print(readDouble());
}

test();
```

# Thanks
lineprocessor.cc in v8 samples
