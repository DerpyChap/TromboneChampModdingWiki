谱面制作常见问题
---

在制作自制谱面时遇到了问题？ 可以在这里寻找答案！

### 我的谱面无法在长号冠军里正常运行！ 我可以控制长号，但我无法暂停。

这类问题通常与您的 `song.ogg` 文件有关。 请确保您正确放置 `song.ogg`文件，并且它的曲目时长要超过谱面文件的时长（取决于谱面的结束点 endpoint）。 如有必要，可以在 `song.ogg` 末尾额外添加几秒静音来将其延长。

### 我的谱面在末尾或在中途会出现卡死，并且无法暂停。但我仍然可以控制长号。

解决方法同上（我的谱面无法在长号冠军里正常运行！）

### 在我点击某个特定音符时，长号冠军出现了卡顿甚至卡死。当曲目结束时我被莫名其妙扣掉了30亿toots？？ （或者Autotoot模式下出现了F或者0分）

这可能是由于在谱面卡顿的地方隐藏了一个幽灵音符。 请检查您的 MIDI 文件，寻找是否有被正常MIDI音符覆盖的错误音符。或在Trombone Charter/BonerViewer中对谱面内容进行检查。 并不能保证每一个程序都能检查出问题所在。 再次游玩已损坏的谱面就可以拿回你的Toots。 在长号冠军的旧版本中，这种现象类似于与点击音符（tap note）相关的问题。 检查您是否是最新版本！

### 我的谱面中有些位置总是会断Combo，甚至Autotoot也会断。

在这些点位检查是否有幽灵音符藏在正常的音符之中！ 直接检查MIDI原文件，或者使用Trombone Charter, and/or BonerViewer。 并不能保证每一个程序都能检查出问题所在。 同时也要注意Autotoot并非完美 您可以更改配置文件中的一些设置以使其更加准确， 但有时它只是单纯跟不上非常快的音符而已。

### 我的自制谱面无法显示在曲目列表中！

确保您的谱面有一个唯一的 `trackref`！ 用记事本或类似功能的编辑器打开tmb 文件，按 Ctrl+F，并搜索 `trackref`。 如果 `Trackref` 值不是唯一的(例如 `trombonecharter_x64` 或歌曲名)，则将其更改至不与其他谱面重复的值。 如果您担心您安装的自制谱面有重复的trackref， 您可以尝试在您的自制歌曲文件夹中运行 [Guardie 的 trackref 查重器](https://github.com/Guarde/TrackRef-Checker/releases/latest)。

### 我的谱面背景看起来很小，且周围有灰色边框。

请修改您的背景尺寸，图片为 1780 x 1000，视频为1920 x 1080。

### 我的谱面背景根本不显示！

确认您的背景文件命名，图像为 `bg.png` ，视频为 `bg.mp4` ，TromBackground为 `bg.trombackground`。

### 我还有其他问题！

如果你仍然有问题，你可以考虑在 Trombone Champ Moding Discord 服务器上寻求帮助。 记得在您的BepInEx文件夹中找到 `LogOutput.log` 文件并与您的问题一同发送，通过它我们可以看一看游戏出问题时发生了什么。