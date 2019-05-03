# Oracle SQL Developer Code Templates for APEX APIs

If you use Oracle Application Express (APEX) APIs reference on SQL Developer, you may benefit from these code templates while working on a SQL Worksheet or PL/SQL Editor.

## Preview

![Preview](/preview.gif?raw=true "Preview")

## Remarks

1. Use `Ctrl + Space` to manually active the Completion Insight or check the automatic popup speed on **Tools >> Preferences >> Code Editor >> Completion Insight**
2. While navigating through the parameters, use `Tab` to move to the next parameter or `Shift + Tab` to move to the previous parameter.
3. Some of the parameters are pre-populated with their default values and some of the parameters display in /\*comments\*/ their available pre-defined values.

## Instructions
1. Download the **CodeTemplate.xml** that matches to your current Oracle APEX version (only 18.2 is available right now).
2. On Windows, navigate to C:\Users\\\<*USER*>\AppData\Roaming\SQL Developer:
    * If you *do not* have any previous Code Template defined, simply replace the existing **CodeTemplate.xml** file.
    * If you *do* have Code Templates defined, copy everything between the <rows></rows> tags on this **CodeTemplate.xml** file and paste it at the end of your existing file, right before the closing </rows> tag.
3. Restart SQL Developer.

## Troubleshooting

1. Go to **Tools >> Preferences >> Database >> SQL Editor Code Templates** and make sure all the code templates are visible.
2. Go to **Tools >> Preferences >> Code Editor >> Completion Insight** and make sure the following options are checked:
    * Enable Completion Auto-Popup in SQL Worksheet
    * Enable Completion Auto-Popup in PL/SQL Editor

## License

![MIT](/LICENSE)