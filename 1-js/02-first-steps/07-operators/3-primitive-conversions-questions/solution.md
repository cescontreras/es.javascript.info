
```js no-beautify
"" + 1 + 0 = "10" // (1)
"" - 1 + 0 = -1 // (2)
true + false = 1
6 / "3" = 2
"2" * "3" = 6
4 + 5 + "px" = "9px"
"$" + 4 + 5 = "$45"
"4" - 2 = 2
"4px" - 2 = NaN
7 / 0 = Infinity
" -9  " + 5 = " -9  5" // (3)
" -9  " - 5 = -14 // (4)
null + 1 = 1 // (5)
undefined + 1 = NaN // (6)
" \t \n" - 2 = -2 // (7)
```

<<<<<<< HEAD:1-js/02-first-steps/06-type-conversions/1-primitive-conversions-questions/solution.md
1. La suma con un string `"" + 1` convierte el número `1` a un string: `"" + 1 = "1"`, luego tenemos `"1" + 0`, la misma regla es aplicada.
2. La resta `-` (como la mayoría de las operaciones matemáticas) sólo funciona con números, convierte un string vacío `""` a `0`.
3. La suma con un string añade el número `5` al string.
4. La resta siempre convierte a números, por lo que convierte `"  -9  "` al número `-9` (ignorando los espacios alrededor del string).
5. La conversión a número convierete `null` en `0`.
6. La conversión a número convierete `undefined` en `NaN`.
=======
1. The addition with a string `"" + 1` converts `1` to a string: `"" + 1 = "1"`, and then we have `"1" + 0`, the same rule is applied.
2. The subtraction `-` (like most math operations) only works with numbers, it converts an empty string `""` to `0`.
3. The addition with a string appends the number `5` to the string.
4. The subtraction always converts to numbers, so it makes `"  -9  "` a number `-9` (ignoring spaces around it).
5. `null` becomes `0` after the numeric conversion.
6. `undefined` becomes `NaN` after the numeric conversion.
7. Space characters, are trimmed off string start and end when a string is converted to a number. Here the whole string consists of space characters, such as `\t`, `\n` and a "regular" space between them. So, similarly to an empty string, it becomes `0`.
>>>>>>> 405150f1f286db19a3c1ed913fa3e905fcefbe46:1-js/02-first-steps/07-operators/3-primitive-conversions-questions/solution.md