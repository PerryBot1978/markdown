# Bash

## Assignment
```bash
*var*=*value*
```

### Append
```bash
*var*=*value*:*var*
*var*=*var*:*value*
```

## If-Else Statement
```bash
if *cond*; then
    *code*
elif *cond*; then
    *code*
else
    *code*
fi
```

## Case Statement
```bash
case *var* in 
    *case1*) *code* ;;
    *case2*) *code* ;;
esac
```

## Alias
```bash
alias *name*='*code*'
```

## Comparison Operators
### Equals
```bash
*var1* -eq *var2*
```

## Auto-Complete
```bash
_complete_exe() {
    COMMANDS="abc bcd cde"
    COMPREPLY=( $( compgen -W "$COMMANDS" -- "${COMP_WORDS[$COMP_CWORD]}") )
}

complete -F *function_name* *command_name*
```
