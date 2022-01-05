# BatColor
Command-Line Utility for Adding Colors to Batch Files. Made using VS and C++.

Image:



![cecho1](https://user-images.githubusercontent.com/92847004/148153066-575bca27-d5db-491b-8989-81c7d217d2cc.png)


Manual:
----
- `{XX}`: colors coded as two hexadecimal digits. E.g., {0A} light green color
- `{\n \t}`: color information as understandable text. E.g., {light red on black}
- `{\n \t}`: New line character - Tab character.
- `{\u0000}`: Unicode character code.
- `{{`: escape character '{'.
- `{#}`: restore initial colors.

Available Colors:
----
Available colors:

- `0` = black	   
- `1` = navy	     
- `2` = green	    
- `3` = teal	    
- `4` = maroon	  
- `5` = purple	   
- `6` = olive	     
- `7` = silver	   
- `8` = gray	     
- `9` = blue
- `A` = lime
- `B` = aqua
- `C` = red
- `D` = fuchsia
- `E` = yellow
- `F` = white

Sample:
----
```
@echo off
cecho {0C}This line is red on black{#}
REM Print ASCII char 0x07 (beep) 
cecho {\u07 \u07}
cecho This {black on blue}word{#} is black on a blue background
```
