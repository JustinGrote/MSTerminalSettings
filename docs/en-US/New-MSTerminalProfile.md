---
external help file: MSTerminalSettings-help.xml
Module Name: MSTerminalSettings
online version:
schema: 2.0.0
---

# New-MSTerminalProfile

## SYNOPSIS
Creates a new MS Terminal profile.

## SYNTAX

```
New-MSTerminalProfile [-Name] <String> [-CommandLine] <String> [-MakeDefault] [[-HistorySize] <Int32>]
 [-SnapOnInput] [[-ColorScheme] <String>] [[-CursorColor] <String>] [[-CursorShape] <String>]
 [[-CursorHeight] <Int32>] [[-FontFace] <String>] [[-StartingDirectory] <String>] [[-FontSize] <Int32>]
 [[-Background] <String>] [[-AcrylicOpacity] <Single>] [-UseAcrylic] [[-ScrollbarState] <String>]
 [-CloseOnExit] [[-Icon] <String>] [[-Padding] <Int32[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Creates a new MS Terminal profile.

## EXAMPLES

### Example 1
```powershell
PS C:\> New-MSTerminalProfile -Name pwsh -CommandLine "C:\Program Files\PowerShell\6\pwsh.exe -WorkingDirectory ~" -Background "#012456" -ColorScheme Campbell
```

Adds a profile named pwsh that runs PowerShell core

## PARAMETERS

### -AcrylicOpacity
Sets the acrylic opacity, 0 being completely transparent and 1 being completely opaque.  This should be a number between 0 and 1.

```yaml
Type: Single
Parameter Sets: (All)
Aliases:

Required: False
Position: 11
Default value: 0.5
Accept pipeline input: False
Accept wildcard characters: False
```

### -Background
Sets the background color of the profile. Overrides "background" set in color scheme if "colorscheme" is set.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloseOnExit
Should MS Terminal close the tab when the program exits.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
```

### -ColorScheme
The name of the color scheme to use for this profile.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: Campbell
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommandLine
The command line to run for this profile.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CursorColor
The cursor color in the format "#RRGGBB"

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: #ffffff
Accept pipeline input: False
Accept wildcard characters: False
```

### -CursorHeight
Sets the height of the cursor. Only works when "cursorShape" is set to "vintage". Accepts values from 25-100.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CursorShape
The cursor shape.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Accepted values: bar, emptyBox, filledBox, underscore, vintage

Required: False
Position: 5
Default value: Bar
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontFace
The name of the font to use for this profile.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 7
Default value: Consolas
Accept pipeline input: False
Accept wildcard characters: False
```

### -FontSize
The size of the font

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 9
Default value: 12
Accept pipeline input: False
Accept wildcard characters: False
```

### -HistorySize
The number of lines of history to store.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: 9001
Accept pipeline input: False
Accept wildcard characters: False
```

### -Icon
The icon to use for this profile.  Ex: "ms-appdata:///roaming/console.ico"

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 13
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MakeDefault
If specified, this profile will become the default profile.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The name of the profile.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Padding
The padding to use between the window edges and the text.

```yaml
Type: Int32[]
Parameter Sets: (All)
Aliases:

Required: False
Position: 14
Default value: 0,0,0,0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScrollbarState
Defines the visibility of the scrollbar. Possible values: "visible", "hidden"

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Accepted values: visible, hidden

Required: False
Position: 12
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SnapOnInput
Enable the SnapOnInput setting.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartingDirectory
The working directory to start in.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 8
Default value: %USERPROFILE%
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseAcrylic
Enable acrylic effects.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### None

## NOTES

## RELATED LINKS