Dialogue UI modding doesn't seem to work in the same way as the rest of the UI mods.
Copying the dialogue state in StateMachines/Keyboard.xaml and overriding seems to have
no effect and also introduces a bunch of xaml file not found errors.

Instead, we will directly override the MainUI dialogue file by placing the
`GUI/Pages/Dialogue.xaml` file under `Mods/MainUI`.