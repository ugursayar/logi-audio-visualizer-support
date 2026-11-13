# Audio Visualizer for the MX Creative Console – support

Audio Visualizer is a plugin for Logi Options+ that turns the LCD keys of the **Logitech MX Creative Keypad** into one live audio visualizer, with dashboard keys (now playing, volume, microphone, clocks) and dials for the **MX Creative Dialpad**. Windows only.

This repository is the plugin's support page. It holds no code.

## Report a problem or ask a question

Open an issue here: **[Issues](../../issues/new)**. That is also the way to contact the author.

To make a problem easy to find, please include:

- the plugin version (Logi Options+ → Plugins → Audio Visualizer)
- your Windows version and Logi Options+ version
- the device (MX Creative Keypad, Dialpad, or both)
- what you did, what you expected, and what happened instead
- a photo or short video of the keys, if it is about what they show

## Sending a log

The plugin normally logs only warnings and errors. If a problem needs a closer look, a detailed log helps:

1. Open the folder `%LOCALAPPDATA%\Logi\LogiPluginService\PluginData\AudioVisualizer` (paste that into the Explorer address bar) and create an empty file named `diagnostics.txt` in it.
2. Use the keypad until the problem shows again, then wait about half a minute.
3. Attach `%LOCALAPPDATA%\Logi\LogiPluginService\Logs\plugin_logs\AudioVisualizer.log` to your issue.
4. Delete `diagnostics.txt` again.

The log contains technical figures and the name of your output device. It never contains what you play.

## Common questions

**The keys stay dark while music plays.**
Some players can take the output device for themselves ("exclusive mode", "bit-perfect", "bypass"). Windows then has nothing to hand to the visualizer. Turn that option off in the player, or untick *Allow applications to take exclusive control of this device* in the Windows sound settings of the output.

**The keys show their action names instead of pictures.**
Restart Logi Plugin Service (end it in Task Manager; it starts again on its own), or restart the computer.

**Does the plugin record or send anything?**
No. It reads the sound your PC plays and the current track's title and cover from Windows only to draw them on the keys. Nothing is saved, logged or sent anywhere.

## License

The plugin is published under the MIT license.
