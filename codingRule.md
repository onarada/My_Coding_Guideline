# My Coding Guideline

## Naming
- Name variables to help understanding code, however, when scope of variable is very short range, it mey be so.
- Naming formats comply with each language starndard or recommendation
- Avoid Japanese word expressed romaji
- Avoid lower-case 'l' because 'l' and '1' are imitate

## Coding Style
If there are not documentaions, coding style comply with each topics example.
- Indent : 4 spaces
- Control Statemants
    - Insert space between statement and brash
    ```Java
    if (a == b) {
        ...
    }
    ```
    - Braces are used with if, else, for, do and while statements, even when the body is empty or contains only a single statement.
    ```Java
    if (a == b) {
        control1();
    } else {
        control2();
    }

    //Example of body is empty
    void doNothing() {}
    ```
    - The order of arguments in conditions  
    Left-side:  
        The expression “being investigated,” whose value is more in flux.  
    Right-side:  
        The expression being
        compared against, whose
        value is more constant.
    ```Java
    if (speed >= 60)
    while (time < limit)
    if (dir == EAST)
    ```
- Variables
    - Space
    ```Java
    int a = 0;
    int b = 10;
    a = b + 10
    ```
    - Multiple declaration is possible, by the way, if declaration may become so long, insert line break properly
    ```Java
    int a = 0, b = 0, c = 0;
    ```
- Comments
    - Do not write comment to explain behavior
    - If you think explaining behavior is needed, you should recondier and rewrite the code
    - Please write "WHY", not "WHAT"
    - Please remove unnecessary comment out


## Limitation
- Max nesting : 3 (recommend 2)
- Max line in block : 50
- If there is a big module, you should divide into some module
- You can use comprehension for only simple case
- Avoid do-while

## Prohibition
- Avoid goto
- Avoid global variables
- Using "Enum" or "Fixed number" instead of magic number
- Do not reuse local variable

