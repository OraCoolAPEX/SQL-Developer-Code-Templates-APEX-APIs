# Oracle SQL Developer Code Templates for APEX APIs

If you use Oracle Application Express (APEX) APIs reference on SQL Developer, you may benefit from these code templates while working on a SQL Worksheet or PL/SQL Editor.

## Preview

![Preview](/preview.gif?raw=true "Preview")

## To Use It

1. Use `Ctrl + Space` to manually activate the Completion Insight or check the automatic popup speed on **Tools >> Preferences >> Code Editor >> Completion Insight**
2. To navigate through the parameters, use `Tab` to move forward or `Shift + Tab` to move backwards.
3. Some parameters are pre-populated with their default values (if any) and others display their pre-defined possible values in /\*comments\*/.

## Limitations
The real purpose of Code Templates in SQL Developer is to create shortcuts (*ii*) that can expand into larger blocks of code (*insert into table values ()*). For this reason, the are some restrictions when it comes to activating Completion Insight for Code Templates:

1. Completion Insight won't show available Code Templates when activated right after a punctuation mark, such as a period (.), instead, it should be activated before, e.g. **APEX_UTIL** `Ctrl + Space` instead of **APEX_UTIL.** `Ctrl + Space` to get the correct results.
2. Different from other code editors with code completion features such as VS Code IntelliSense, Code Templates in SQL Developer are limited in the amount of information that can be specified (i.e. Id and Template), thus there are no package procedure and function descriptions.
3. By default, Completion Insight won't show more than 20 suggestions and, at the moment, there is no option to increase this value, which affect when displaying the available procedures and functions from a large package.

## To Configure It

1. Download the **CodeTemplate.xml** that matches your current version of Oracle APEX.
2. On Windows, navigate to C:\Users\\\<*USER*>\AppData\Roaming\SQL Developer:
    * If you *do not* have any previous Code Template defined, simply replace the existing **CodeTemplate.xml** file.
    * If you *do* have Code Templates defined, copy everything between the \<rows>\</rows> tags on this **CodeTemplate.xml** file and paste it at the end of your existing file, right before the closing \</rows> tag.
3. Restart SQL Developer.

## Troubleshooting

1. Go to **Tools >> Preferences >> Database >> SQL Editor Code Templates** and make sure all the code templates are visible.
2. Go to **Tools >> Preferences >> Code Editor >> Completion Insight** and make sure the following options are checked:
    * Enable Completion Auto-Popup in SQL Worksheet
    * Enable Completion Auto-Popup in PL/SQL Editor

## License

![MIT](/LICENSE)