# Tips - bash tricks

---

## diff two commands' outputs

```
diff <(COMMAND1) <(COMMAND2)
```

---

## Arithmetic operation on variables

Use double parenthesis instead single.

```
a=1
((a++))         # a=12
b=$((a+2))      # b=3
```

---

## List elements of array, get length of array

```
arr=("1 one" "2 two" "3 three")
echo ${arr[@]}

len=${#arr[@]}
```

---

## Merge and pipe results from two commands

```
{ cat file1; ls dir; } | wc -l
```

or

```
( cat file1; ls dir; ) | wc -l
```

The parenthesis `()` wrapped command group will be executed in a subshell.

---

## ¶ The end

