# CompilaCompiler
A basic Compiler of a custom programming language called Compila


## Langage specifications 
- One and only one instruction per line
- Program always starts with "Start_Program" and ends with "End_Program"
- A comment can only be contained in one line, and must start with  //.
- An instruction always ends with ";;"
- Regular expressions corresponding to variables types of this language are : 

Type | Description | RegEx 
-----| ------------| ---------
Identifier | Starts with a letter followed by one AlphaNum character or more | `{letter}(_?({letter}\|{digit})+)*` 
Integer number | Composed of at least one digit  |  `[0-9]+`
Real number | Composed of atleast two integers separated by a point "." |  `[0-9]+\.[0-9]+`

- Here are some of the language's commands : 

Command | Description | Example 
------- | ----------- | ---------------
Assignment of a number (Integer/Real) to a variable | Give <<identifier>> <<value>> ;; | `Give i 23 ;;`
Assignment of the value of a variable to another variable | Affect <<identifier>> to <<identifier>>;; | `Affect i to j ;;`
Condition | If - condition - action ;; | `If - i > j -Give Aft_5 10 ;;`


## Exemple de Code 
`Start_Program` <br/>
`Int_Number` i , j, Aft_5 ;;<br/>
`Give` i 23 ;; <br/>
`Real_Number` Aft34_2 ;; <br/>
`If `- i < j - <br/>
`Give` Aft_5 10 ;; <br/>
`Else` <br/>
`Start` <br/>
`Affect` i `to` j ;; <br/>
`Give` Af34_2 123.54 ;; <br/>
`Finish` <br/>
`ShowMes` " ceci est un message " ;; <br/>
`//.` ceci est un commentaire <br/>
`End_Program`
