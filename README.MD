# IntelliJ Theme demo plugin

Themes are special plugins for IntelliJ-based IDEs allowing to change IDE's look. A theme can modify following parts of IDE:
- Colors of common components like Panels, Labels, Comboboxes, etc. 
- Editor color scheme
- Icons
- Background image 

### To create a theme: 
1. Install IntelliJ IDEA 2018.3 or newer with DevKit plugin enabled
2. Create new plugin project
3. In Project View on **src** folder invoke New -> Plugin DevKit -> Theme
4. Edit necessary fields in just created Xxx.theme.json file

### *.theme.json file structure
*.theme.json file consists of following parts:

<pre>
<span color="#a9b7c6">{</span>
  <span color="#6a8759">&quot;name&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;Stalker&quot;</span><span style="color: #cc7832;">,</span>
  <span style="color: #6a8759;">&quot;dark&quot;</span><span style="color: #cc7832;">: </span><span style="color: #cc7832; font-weight: bold;">true</span><span style="color: #cc7832;">,</span>
  <span style="color: #6a8759;">&quot;author&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;Konstantin Bulenkov&quot;</span><span style="color: #cc7832;">,</span>

  <span style="color: #6a8759;">&quot;editorScheme&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;/editorScheme.xml&quot;</span><span style="color: #cc7832;">,</span>

  <span style="color: #6a8759;">&quot;ui&quot;</span><span style="color: #cc7832;">: </span><span style="color: #a9b7c6;">{</span>
    <span style="color: #6a8759;">&quot;*&quot;</span><span style="color: #cc7832;">: </span><span style="color: #a9b7c6;">{</span>
      <span style="color: #6a8759;">&quot;background&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#000000&quot;</span>
    <span style="color: #a9b7c6;">}</span><span style="color: #cc7832;">,</span>
    <span style="color: #6a8759;">&quot;Label&quot;</span><span style="color: #cc7832;">: </span><span style="color: #a9b7c6;">{</span>
      <span style="color: #6a8759;">&quot;foreground&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#aaaaaa&quot;</span>
    <span style="color: #a9b7c6;">}</span><span style="color: #cc7832;">,</span>
    <span style="color: #6a8759;">&quot;SidePanel.background&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#222222&quot;</span><span style="color: #cc7832;">,</span>
    <span style="color: #6a8759;">&quot;SearchMatch.startColor&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#FFD103&quot;</span><span style="color: #cc7832;">,</span>
    <span style="color: #6a8759;">&quot;SearchMatch.endColor&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#DDAF03&quot;</span><span style="color: #cc7832;">,</span>
    <span style="color: #6a8759;">&quot;SearchMatch.transparency&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6897bb;">70</span>
  <span style="color: #a9b7c6;">}</span><span style="color: #cc7832;">,</span>

  <span style="color: #6a8759;">&quot;background&quot;</span><span style="color: #cc7832;">: </span><span style="color: #a9b7c6;">{</span>
    <span style="color: #6a8759;">&quot;image&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;/background.jpg&quot;</span><span style="color: #cc7832;">,</span>
    <span style="color: #6a8759;">&quot;transparency&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6897bb;">10</span><span style="color: #cc7832;">,</span>
    <span style="color: #6a8759;">&quot;fill&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;scale&quot;</span><span style="color: #cc7832;">,</span>
    <span style="color: #6a8759;">&quot;anchor&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;center&quot;</span>
  <span style="color: #a9b7c6;">}</span><span style="color: #cc7832;">,</span>

  <span style="color: #6a8759;">&quot;icons&quot;</span><span style="color: #cc7832;">: </span><span style="color: #a9b7c6;">{</span>
    <span style="color: #6a8759;">&quot;ColorPalette&quot;</span><span style="color: #cc7832;">: </span><span style="color: #a9b7c6;">{</span>
      <span style="color: #6a8759;">&quot;Actions.Green&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#FF365D&quot;</span><span style="color: #cc7832;">,</span>
      <span style="color: #6a8759;">&quot;Actions.Grey&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#FFFFFF&quot;</span><span style="color: #cc7832;">,</span>
      <span style="color: #6a8759;">&quot;Objects.Blue&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#0C76FF&quot;</span><span style="color: #cc7832;">,</span>
      <span style="color: #6a8759;">&quot;Objects.Grey&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#EA8E2C&quot;</span><span style="color: #cc7832;">,</span>
      <span style="color: #6a8759;">&quot;Objects.Red&quot;</span><span style="color: #cc7832;">: </span><span style="color: #6a8759;">&quot;#ff0000&quot;</span>
    <span style="color: #a9b7c6;">}</span>
  }
}</pre>



