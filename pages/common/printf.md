# printf

> Format and print text.
> See also: `echo`.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/printf-invocation.html>.

- Print a text message:

`printf "{{%s\n}}" "{{Hello world}}"`

- Print an integer in bold blue:

`printf "{{\e[1;34m%.3d\e[0m\n}}" {{42}}`

- Print a float number with the Unicode Euro sign:

`printf "{{\u20AC %.2f\n}}" {{123.4}}`

- Print a text message composed with environment variables:

`printf "{{var1: %s\tvar2: %s\n}}" "{{$VAR1}}" "{{$VAR2}}"`

- Store a formatted message in a variable (does not work on Zsh):

`printf -v {{myvar}} {{"This is %s = %d\n" "a year" 2016}}`

- Print a hexadecimal, octal and scientific number:

`printf "{{hex=%x octal=%o scientific=%e}}" 0x{{FF}} 0{{377}} {{100000}}`
