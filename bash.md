# Bash

## Assignment
```
*var*=*value*
```

### Append
```
*var*=*value*:*var*
*var*=*var*:*value*
```

## If-Else Statement
```
if *cond*; then
    *code*
elif *cond*; then
    *code*
else
    *code*
fi
```

## Case Statement
```
case *var* in 
    *case1*) *code* ;;
    *case2*) *code* ;;
esac
```

## Alias
```
alias *name*='*code*'
```

## Comparison Operators
### Equals
```
*var1* -eq *var2*
```

## Auto-Complete
```
_complete_exe() {
    COMMANDS="abc bcd cde"
    COMPREPLY=( $( compgen -W "$COMMANDS" -- "${COMP_WORDS[$COMP_CWORD]}") )
}

complete -F *function_name* *command_name*
```
