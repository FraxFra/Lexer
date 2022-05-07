# Lexer
The lexer is a program that lexically analyses a code written in a proper grammar.<br/>
Input -> file.txt containing source code written with the following grammar<br/>
Output -> A sequence of tokens grammatically correct.<br/>

## Grammar
```
<prog> -> <statlist> EOF
<statlist> -> <stat> <statlistp>
<statlistp> -> ; <stat> <statlistp> | epsilon
<stat> -> = ID <expr> | print ( <exprlist> ) | read ( ID ) | cond <whenlist> else <stat> | while ( <bexpr> ) <stat> | { <statlist> }
<whenlist> -> <whenitem> <whenlistp> 
<whenlistp> -> <whenitem> <whenlistp> | epsilon
<whenitem> -> when ( <bexpr> ) do <stat> 
<bexpr> -> RELOP <expr> <expr>
<expr> -> + ( <exprlist> ) | * ( <exprlist> ) | - <expr> <expr> | / <expr> <expr> | NUM | ID
<exprlist> -> <expr> <exprlistp>
<exprlistp> -> <expr> <exprlistp> | epsilon
```
