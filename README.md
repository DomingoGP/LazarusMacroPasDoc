# LazarusMacroPasDoc
Macro for [Lazarus ide](https://www.lazarus-ide.org/) to document functions and procedures. Makes [Pasdoc](https://github.com/pasdoc/pasdoc/wiki) comment template


[Create a macro](https://wiki.freepascal.org/IDE_Window:_Editor_Macros) in lazarus and edit inserting 
MacroPasDocLazarus.txt in the macro, assign a key to the macro.

To create a new macro push the Record button and pulse a key then stop recording in the lazarus editor status line.
Move the new macro to the ide page and edit then macro changing the text with the contents of MacroPasDocLazarus.txt.


Execute the macro with the caret in the line of the
procedure function declaration.


example:

    function AddRadioButton(const aCaption: string; aChecked: boolean = False): TCheckBox;
    
Executing the macro with the caret in the line of function declaration will insert the comment before.

    { Description
      @param(aCaption description )
      @param(aChecked description )
      @returns( description )
      @raises( none )
    }
    function AddRadioButton(const aCaption: string; aChecked: boolean = False): TRadioButton;

**Requeriments**: The package *editormacroscript* must be installed in the ide.


[More Lazarus macros and information of the other macros](https://wiki.freepascal.org/IDE_Window:_Editor_Macros)
