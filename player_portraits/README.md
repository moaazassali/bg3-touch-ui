Unless we override the 'PlayerHUD' state which also overrides any other mod that does so
like our world context mod which edits Overlay.xaml, we have to force the loaded
PlayerPortraits.xaml to show nothing. This is why we need an empty PlayerPortraits.xaml
in MainUI to override it. Unlike other PlayerHUD elements, ImpUI doesn't provide a nicer
way for us to override PlayerPortraits, so we either have to extend ImpUI and add another
dependency to our mods or resort to this hack, which I find much simpler.