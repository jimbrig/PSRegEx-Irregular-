﻿## Irregular 0.7.9:

* Irregular Docker Support (#205,#206,#207)
  * `docker run --interactive --tty ghcr.io/startautomating/irregular`
* Irregular Repository Cleanup (#208, #209, #210, #211)
* Exporting $Irregular (#212)
* Mounting Irregular: (#213) 
* Simple Symbol Patterns
  * ?<Symbol> (#202)
  * ?<Symbol_Currency> (#214)
  * ?<Symbol_Math> (#203)
  
---

## Irregular 0.7.8:

* Adding Compress-Regex (Fixes #178)
* New Regexes:  
  * ?<YAML_Value> (Fixes #192)
  * ?<YAML_Key> (Fixes #191)
  * ?<Degrees> (Fixes #185)
  * ?<Git_Commit> (Fixes #193)
  * ?<RegularExpression_GroupName> ( #195 )
  * ?<PowerShell_Hashtable> ( Fixes #194 )
  * ?<PowerShell_Requires>:  Allowing open ended requirement (Fixes #182)
Renaming ANSI Regexes to Console (Fixes #188)

---

## Irregular 0.7.7:

New Patterns:

* ?<Code_Method> : Matches methods in most languages  (Fixes #171)
* ?<Code_PackageVersion> : Matches a package name and version (Fixes #172)
* ?<ANSI_Link> : Matches an ANSI Hyperlink (Fixes #173)

---

## Irregular 0.7.6:

* New-RegEx improvements:
  * Now supporting new character classes:  MarkSpacing, MarkEnclosing, MarkNonEnclosing (Fixes #168)

* More CSharp Patterns:
  * ?<CSharp_Class> (Fixes #164)
  * ?<CSharp_Identifier> (Fixes #165)

* Improved Patterns:
  * ?<ANSI_4BitColor>/?<ANSI_Style>: Handling brightness bit before or after color (Fixes #166)

---

## Irregular 0.7.5:

* Added Patterns for Liquid:
  * ?<Liquid_Expression> (Fixes #153)
  * ?<Liquid_Tag> (Fixes #154)

---

## Irregular 0.7.4:
* ANSI Improvements:
  * Regenerated ?<ANSI_Color> (Fixes #150)
  * Added ?<ANSI_Cursor> (Fixes #151)

---

## Irregular 0.7.3:
* ANSI Improvements:
  * Fixed ?<ANSI_Style> (Fixes #143)
  * ?<ANSI_4BitColor> now supports bright ranges (Fixes #145)
  * ?<ANSI_8BitColor>/?<ANSI_24BitColor> now supports background colors (Fixes #144)
  * ?<ANSI_8BitColor>/?<ANSI_24BitColor> now supports underline colors (Fixes #146)

---

## Irregular 0.7.2:
* Lots More ANSI support:
  * ?<ANSI_Bold> (Fixes #131)
  * ?<ANSI_Blink> (Fixes #132)
  * ?<ANSI_Faint> (Fixes #133)
  * ?<ANSI_Hide> (Fixes #134)
  * ?<ANSI_Invert> (Fixes #135)
  * ?<ANSI_Italic> (Fixes #136)
  * ?<ANSI_Reset> (Fixes #137)
  * ?<ANSI_Strikethrough> (Fixes #138)
  * ?<ANSI_Underline> (Fixes #139)
  * ?<ANSI_Style> (Fixes #140)
  * ?<ANSI_Note>:  Fixing capture names (Fixes #130)

---

## Irregular 0.7.1:
* New Pattern:
  * ?<ANSI_Note> (Match ANSI VT520 / DECPS note sequences) (Fixes #127) 
* Updated Patterns:
  * ?<FFMpeg_Progress>: Supporting duplicated / dropped frames (Fixes #128)
  * ?<Code_BuildVersion>: No longer matching if preceeded by punctuation (Fixes #126)

---

## Irregular 0.7.0:
* New Patterns:
  * ANSI
    * ?<ANSI_Code>  (Fixes #123)
    * ?<ANSI_Color> (Fixes #124)
    * ?<ANSI_DefaultColor>
    * ?<ANSI_4BitColor>
    * ?<ANSI_8BitColor>
    * ?<ANSI_24BitColor>
  * Mustache
    * ?<Mustache_Tag> (Fixes #121)
* New-Regex -LiteralCharacter '_' no longer escapes (Fixes #122)
* Reducing module size (excluding assets) (Fixes #118)

---

## Irregular 0.6.9:
* Adding ?<Markdown_Link> (Fixes #117)
* GitHub Action now prefers local bits (Fixes #111)
* Using PipeScript to enhance the repository experience (Fixes #119)

---

## Irregular 0.6.8:
* Added ?<CamelCaseSpace> (Fixes #114)
* Fixing ?<PowerShell_HelpField> (Fixes #108)
* Use-Regex:
  * Returning generator if -Match and -ExpressionParameter are not provided (Fixes #113)
* Automatically documenting module (Fixes #109)
* Automatically building module formatting (Fixes #112)
* Fixing Documentation (Fixes #115)

---

## Irregular 0.6.7:
* Command Improvements:
  * New-Regex:  Adding -ExcludeCharacterClass/-ExcludeLiteralCharacter/-ExcludeUnicodeCharacter (Fixing #104)
  * Use-Regex:  Adding -IncludeInputObject (Fixing #103)
  * Import-Regex:  Imported regular expressions are more likely to keep their path, even if they must be retried.
* Renaming Regex:  ?<BuildVersion> is now ?<Code_BuildVersion>
* GitHub Action Improvements:
  * Additional Tracing in GitHub Action.  Now ready for use.  (Fixing #93)
* Additional Improvements:
  * [SavedPatterns.md](SavedPatterns.md) now automatically updates.

---

## Irregular 0.6.6:
* New Regexes:
  * ?<C_Enum> (#98)
  * ?<C_Struct> (#99)
* Fixing Issues with whitespace in ?<FFMpeg_Progress> (#97)

---

## Irregular 0.6.5
* Renaming Regex: ?<IPV4Address> is now ?<Network_IPV4Address> (#90)
* New Regex: ?<Network_MACAddress> (#89)
* Use-Regex -Extract:  Now attempting [Timespan] before [DateTime] (#88)

---

## Irregular 0.6.4
* Renaming Write-RegEx to New-RegEx (#66) ** Write-RegEx will remain aliased until at least 0.7**
* Fixing Issue in Embedding (#82)
* Improving -Extract by auto-detecting data types (#81)
* ?<FFMpeg_Progress> - Fixing capture name (#80)
* Adding ?<FFMpeg_Configuration> (#83)
* Adding ?<FFMpeg_Stream> (#83)
* Adding ?<FFMpeg_Input> (#83)
* Adding ?<FFMpeg_Output> (#83)
* Adding ?<FFMpeg_Metadata> (#83)

---

## Irregular 0.6.3
New Regular Expressions:
* ?<CNC_GCode> (Fixes #76)
* OpenSCAD Expressions (Fixes #75)  
  * ?<OpenScad_Customization>
  * ?<OpenScad_Function>
  * ?<OpenScad_Include>
  * ?<OpenScad_Module>
  * ?<OpenScad_Parameter>
  * ?<OpenScad_Use>
* Additional Markdown Regexes
  * ?<Markdown_List> (Fixes #70)
  * ?<Markdown_YAMLHeader> (Fixes #71)
* Subtitle Regexes (Fixes #72)
  * ?<Subtitle_SRT>
  * ?<Subtitle_VTT>

---

## Irregular 0.6.2
New Regular Expressions:
* ?<Unix_Cron_Interval> (Fixes #67)
* ?<Unix_Duration> (Fixes #69)

---

## Irregular 0.6.1
* New Command:  Remove-RegEx (Fixes #62)
* Set-RegEx now supports -PassThru (Fixes #61)
* Set-RegEx now allows modifiers (Fixes #60)
* Use-RegEx now allows -Pattern to be directly provided, and supplies an ArgumentCompleter (Fixes #59)
Hat Tips: @JayKul, @LaurentDardenne

---

## Irregular 0.6
* JSON Regex Improvements
 * ?<JSON_Property> now can handle quotes
* Markdown Regexes:
 * ?<Markdown_Heading>
 * ?<Markdown_CodeBlock>
 * ?<Markdown_ThematicBreak>
* ?<REST_Variable> is now a generator.

---

## Irregular 0.5.9
* New RegEx:
  * ?<C_IfDef>
* New and Improved RegEx:
  * ?<JSON_Property> is now a generator (can specify -PropertyName)
  * ?<JSON_ListItem>
* Write-RegEx Improvements:
  * -Atomic now indents
  * -Or now indents
  * No longer makes -Then/-Else explicily non-capturing

---

## Irregular 0.5.8
* New RegEx:
  * ?<RegularExpression_Quantifier>
* Fixes to RegExes:
  * ?<REST_Variable> now allows variables to be embedded within <>s

---

## Irregular 0.5.7
* New RegExes:
  * ?<Security_AccessToken>
  * ?<Security_JWT>
* Fixes to Regexes:
  * ?<EmailAddress> now handles subdomains (#39)
  * ?<IPV4Address> will no longer match digits past the byte-range. (#38)
* New Capabilities:
  * Write-RegEx -DigitMax

---

## Irregular 0.5.6
* New RegExes:
  * ?<Code_SemanticVersion>
  * ?<FFmpeg_Progress>
  * ?<Keyboard_Shortcut>
  * ?<PowerShell_ParameterSet>
* Use-RegEx Improvements:
  * -Extract no longer includes .0 and the eponymous match group (unless that was the only group).
  * -Extract no longer includes .Match unless -IncludeMatch is passed.
  * -PSTypename can be used to decorate a match (implies -Extract)
* Write-RegEx Improvements:
  * Write-RegEx -Atomic -Or no longer overgroups
  * Write-RegEx -LiteralCharacter -Not now works as expected
  * Write-RegEx -Atomic -Min/-Max location fixed

---

## Irregular 0.5.5
* New Programming RegExes:
  * ?<PowerShell_Requires>
  * ?<C_Include>
  * ?<C_Define>
  * ?<CSharp_Using>
  * ?<CSharp_Namespace>

* Renaming ?<Namespace> to ?<Code_Namespace> [breaking]
* ?<REST_Variable>:
  * support for {/optionalsegments} (as seen in Git)
  * dollar sign now requires backtick (URL parameters can be named $, e.g. $top)

---

## Irregular 0.5.4
* Fixes in Irregular import (no longer producing a module per RegEx on import)
* Fixing a subtle bug in Write-RegEx -Until (was failing to match when no characters were between)
* New regex:
  * ?<HTML_LinkedData>, ?<HexColor>, ?<IPv4Address>

---

## Irregular 0.5.3
* Get/Export-Regex: Now supporting -As EmbeddedEngine (lambas) or -As Engine (smart aliases)
* Write-RegEx:  Added -UnicodeCharacter
* New regex:
  * ?<PowerShell_Region>
  * ?<Unix_Conf_Line>, ?<Unix_Conf_Section>, ?<Unix_Conf_File>, ?<Unix_Mount>, ?<Unix_FileSystemType>, ?<Unix_User>
* Updated RegEx Generators:
  * ?<MultilineComment> now supports OpenSCAD (.scad)

---

## Irregular 0.5.2
* Use-RegEx now matches within returns by default.
* Use-RegEx can -Scan to match after a given item
* Use-Regex breaking change:  -Parameter/-ArgumentList are now -ExpressionParameter/-ExpressionArgumentList
* Improving formatting (no longer showing match status, which was always 'true')

---

## Irregular 0.5.1
* Making Import-Regex support Regexes defined in other modules
* Allowing Import-Regex to import as lambdas
* Get/Export-Regex now include -As "Engine", which will export an embeddedable engine including an inline Import
* Write-Regex now supports -Modifier
* New Expressions:
  * ?<HexDigits>
  * ?<Git_Diff>
  * ?<Git_DiffHeader>
  * ?<Git_DiffRange>
  * ?<Git_Log>
  * ?<HTML_IDAttribute>
  * ?<HTML_DataAttribute>
  * ?<HTML_DataSet>
  * ?<HTML_ItemScope>
