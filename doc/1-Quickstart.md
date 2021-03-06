## Quickstart 快速开始

Welcome to the Ren'Py quickstart manual. The purpose of this manual is to demonstrate how you can make a Ren'Py game from scratch, in a few easy steps. We'll do this by showing how to make a simple game, *The Question*, from scratch. This manual contains a number of examples, which are included as part of the demo game.

欢迎来到Ren'Py的快速入门教程。本教程旨在展示如何通过几个简单的步骤从从零开始制作一款Ren'Py游戏。我们将演示如何从零开始制作一个简单的游戏，*The Question*。本教程包含的几个简单例子，都将作为示例游戏的一部分。

### The Ren'Py Launcher 启动器

Before you begin making a game, you should first take some time to learn how the Ren'Py launcher works. The launcher lets you create, manage, edit, and run Ren'Py projects.

**Getting Started.** To get started you'll want to [download Ren'Py](http://www.renpy.org/doc/html/quickstart.html).

Once you've downloaded Ren'Py, you'll want to extract it. This can generally be done by right-clicking on the package file, and picking "Extract" if that's an option, or "Open" if it's not. Follow the prompts, and you'll have a working copy of Ren'Py.

>Note:
Please be sure you've extracted Ren'Py to its own directory or folder on disk. If you try to run it from inside a ZIP file, it won't work properly.

Once you've extracted Ren'Py, you'll need to run it.

-	On Windows, run the `renpy` or `renpy.exe` program.
-	On Mac OS X, run the `renpy` application.
-	On Linux, run the `renpy.sh` script.

After running this, the Ren'Py launcher should run.

The Ren'Py launcher has been translated to multiple languages. To change the language, choose "preferences" and then select the language.


![](http://p1.bqimg.com/567571/79e5f58293446dc9.jpg)

**Choosing and Launching a Project.** You should first see what the completed The Question game looks like. To do this, start the Ren'Py launcher, and choose "The Question" from the first screen. Choose "Launch Project" to start The Question.

You can get back to the Ren'Py demo by doing the same thing, but choosing "Tutorial" instead of "The Question".

**Creating a new Project.** Create a new project by choosing "Create New Project" from the launcher. The launcher will then ask you for a project name. Since "The Question" is already taken, you should enter something different, like "My Question". The launcher will then ask you to choose a color theme for the project. It doesn't matter what you pick at this point, just choose something that appeals to you. You'll be returned to the top menu of the launcher with your new game chosen.

###  A Simple Game 一个简单游戏

```
label start:
    "I'll ask her..."

    "Me" "Um... will you..."
    "Me" "Will you be my artist for a visual novel?"

    "Silence."
    "She is shocked, and then..."

    "Sylvie" "Sure, but what is a \"visual novel?\""
```

This is perhaps one of the simplest Ren'Py games. It doesn't include any pictures or anything like that, but it does show a conversation between the two characters.

这或许是最简单的Ren'Py游戏之一。它不包含任何图片或类似的东西，但它确实是呈现了两个角色之间的对话。

To try this out, go into the launcher, select the "**`The Question Project`**", and choose "**`script.rpy`**" from under **`Edit File`**. Ren'Py may ask you to select a text editor, after which it will download the editor you select. When it finishes, script.rpy will open in an editor. Erase everything in script.rpy, as we're starting from scratch, so you don't need what's there. Copy the example above into script.rpy, and save it.


为了实现这一点，打开Ren'Py的启动器，选择"**`The Question `**"，并从**`Edit File`**选择“**`script.rpy`**”。

![](http://i1.piimg.com/567571/bc43cc8bf58968f5.jpg)

![](http://i1.piimg.com/567571/88bdc848afb22618.jpg)

Ren'Py可能询问您选择使用哪一种文本编辑器打开**`.rpy`**文件，并在选择后自动下载您所选择的编辑器。当以上步骤完成后，**`script.rpy`**将在文本编辑器中打开。删除掉**`script.rpy`**中的所有内容，因为我们将从头开始，所以你不需要那里的东西。复制上面的例子到**`script.rpy`**，并保存。

![](http://i1.piimg.com/567571/7c4829cf692a66b7.jpg)


You're now ready to run this example. Go back to the launcher, and choose "Launch Project". Ren'Py will start up. Notice how, without any extra work, Ren'Py has given you menus that let you load and save the game, and change various preferences. When ready, click "Launch Project", and play through this example game.

现在准备运行上述例子。返回到启动器主页，然后选择"**`Launch Project`**，Ren'Py将会启动。现在可以注意到是，在没有进行其他额外的工作时，Ren'Py将会为默认为你提供包括读取游戏，保存游戏和更该偏好设置的游戏界面。当以上准备就绪后，点击**`Launch Project`**，可以开始试玩这个示例游戏。

![](http://i1.piimg.com/567571/98af8c1052481709.jpg)

![](http://p1.bqimg.com/567571/1c2ff25ac5a6a2e3.jpg)


This example shows some of the commonly-used Ren'Py statements.

这个例子展示了Ren'Py常见语句的用法。

The first line is a label statement. The label statement is used to give a name to a place in the program. In this case, we create a label named start. The start label is special, as it's where Ren'Py scripts begin running when the user clicks "Start Game" on the main menu.

第一行是一个**`label`(标签）**声明。标签声明用于在程序中提供一命名空间。在这种情况下，我们创建了一个名为**`start`(标签）**的标签。**`Start`**标签是特殊的，因为它是当玩家点击主菜单的**`start Game`**时，Ren'Py脚本开始运行的入口处。

The other lines are say statements. There are two forms of the say statement. The first is a string (beginning with a double-quote, containing characters, and ending with a double-quote) on a line by itself, which is used for narration, and the thoughts of the main character. The second form consists of two strings. It's used for dialogue, with the first string being a character name and the second being what that character is saying.

其他行都是**`say`(对白）**语句。**`say`**语句有两种形式的声明：第一种形式是以被包裹在半角双引号的文字为一行，主要用于陈述或者描述角色的心理活动。第二种形式则是由两行文字组成，第一行文字用于显示人物名字，第二行文字用于显示人物对白。



Note that all the say statements are indented by four spaces. This is because they are a block underneath the label statement. In Ren'Py, blocks must be indented relative to the prior statement, and all of the statements in a block must be indented by the same amount.

请注意，所有的**`say`**语句都要有四个空格缩进。这是因为它们是隶属于**`label`**语句下方的区块。在Ren'Py，区块必须相对于之前的语句进行缩进。所有在一个区块中的语句，必须以相同的空格数进行缩进。

When strings contain double-quote characters, those characters need to be preceded by a backslash. This is done in the last line of our example.

当字符串包含双引号时，需要在前面加一个反斜杠**`\`**进行转义。在上面的示例游戏的最后一行，你可以看到类似的实现。

While this simple game isn't much to look at, it's an example of how easy it is to get something working in Ren'Py. We'll add the pictures in a little bit, but first, let's see how to declare characters.

虽然这个示例游戏并不值得多看，毕竟它只是在Ren'Py下的一个十分简单的例子。之后我们将学会往游戏里添加图片，但是在那之前，首先来看看如何在脚本里声明（新建）一个角色。


###  Init 初始化


The init statement is used to execute blocks of Ren'Py statements before the script executes. Init blocks are used to define images and characters, to set up unchanging game data structures, and to customize Ren'Py. Code inside init blocks should not interact with the user or change any of the layers, and so should not contain say, menu, scene, show, or hide statements, as well as calls to any function that can do these things.

**`init`(初始化)**语句会在脚本运行前预执行一些Ren'Py的语句区块。初始化区块被用于定义图像和角色，以此设置一些不变的游戏数据结构，以及Ren'Py的自定义功能。初始化区块内部的代码不应该和用户进行任何交互或更改游戏内的图层，因此不应该包含**`say`**, **`menu`**, **`scene`**, **`show`**, 或者**`hide`**等任何在功能上类似的语句。



An init statement is introduced with the keyword init, followed by an optional priority number, and a mandatory colon. If the priority is not given, it defaults to 0. Priority numbers should be in the range -999 to 999. Numbers outside of this range are reserved for Ren'Py code.

一个初始化语句的引入是以**`init`**作为关键字，后面跟着一个可选的表示优先级的数字，最后必须以冒号结束。如果优先级没有给出，则默认为0。优先级的范围应该在-999到999之间，超出此范围之外的数字是Ren'Py的保留字。


The priority number is used to determine when the code inside the init block executes. Init blocks are executed in priority order from low to high. Within a file, init blocks with the same priority are run in order from the top of the file to the bottom. The order of evaluation of priority blocks with the same priority between files is undefined.

表示优先级的数字是原来决定初始化区块中的代码执行顺序的。初始化区块中的语句会按照优先级顺序从低到高执行。在一个文件中，拥有相同优先级的**`init`**块在从上往下依次执行。不同文件之间拥有相同优先级的初始化区块的执行顺序是未定义的。

The init blocks are all run once, during a special init phase. When control reaches the end of an init block during normal execution, execution of that block ends. If an init statement is encountered during normal execution, the init block is not run. Instead, control passes to the next statement.

初始化区块的语句只会在特殊的初始化阶段运行。当主程序在正常的游戏执行过程遇到初始化块，将执行其块中语句直至结束。如果一个**`init`**语句出现在正常的游戏执行过程中，将不会被执行。相对的，主程序将会跳过这一语句执行接下来的代码。

### Characters 角色

===未完待续===

One problem with the first example is that it requires you to repeatedly type the name of a character each time they speak. In a dialogue-heavy game, this might be a lot of typing. Also, both character names are displayed in the same way, in fairly boring white text. To fix this, Ren'Py lets you define characters in advance. This lets you associate a short name with a character, and to change the color of the character's name.

与第一示例的一个问题是，它需要你每次发言时间来反复键入一个字符的名称。在对话为主的游戏，这可能是一个很大的打字。另外，无论字符名称显示在以相同的方式，在相当乏味白色文字。为了解决这个问题，Ren'Py的可以让你预先定义的字符。这可以让你一个简短的名称与角色联系起来，并改变角色的名字的颜色。

```
define s = Character('Sylvie', color="#c8ffc8")
define m = Character('Me', color="#c8c8ff")

label start:
    "I'll ask her..."

    m "Um... will you..."
    m "Will you be my artist for a visual novel?"

    "Silence."
    "She is shocked, and then..."

    s "Sure, but what is a \"visual novel?\""
```

The first and and second lines define characters. The first line defines a character with the short name of "s", the long name "Sylvie", with a name that is shown in a greenish color. (The colors are red-green-blue hex triples, as used in web pages.)

The second line creates a character with a short name "m", a long name "Me", with the name shown in a reddish color. Other characters can be defined by copying one of the character lines, and changing the short name, long name, and color.

We've also changed the say statements to use character objects instead of a character name string. This tells Ren'Py to use the characters we defined in the init block.

我们还改变了发言权语句使用字符对象，而不是一个角色名字符串。这告诉Ren'Py的使用，我们在init块中定义的字符。

## Images 图片

A visual novel isn't much of a visual novel without pictures. Let's add some pictures to our game.

```
image bg meadow = "meadow.jpg"
image bg uni = "uni.jpg"

image sylvie smile = "sylvie_smile.png"
image sylvie surprised = "sylvie_surprised.png"

define s = Character('Sylvie', color="#c8ffc8")
define m = Character('Me', color="#c8c8ff")

label start:
    scene bg meadow
    show sylvie smile

    "I'll ask her..."

    m "Um... will you..."
    m "Will you be my artist for a visual novel?"

    show sylvie surprised

    "Silence."
    "She is shocked, and then..."

    show sylvie smile

    s "Sure, but what is a \"visual novel?\""
```

The first new thing we needed to do was to declare the images, using image statements on lines 2, 3, 5, and 6, inside the init block. These image statements give an image name, and the filename the image is found in.

For example, line 5 declares an image named "sylvie smile", found in the filename "sylvie_smile.png", with the tag "sylvie".

We have a scene statement on line 12. This statement clears out the screen, and shows the "bg meadow" image. The next line is a show statement, which shows the "sylvie smile" image on the screen.

The first part of an image name is the image tag. If an image is being shown, and another image with the same tag is on the screen, then the image that's on the screen is replaced with the one being shown. This happens on line 19, the second show statement. Before line 19 is run, the image "sylvie smile" is on the screen. When line 19 is run, that image is replaces with "sylvie surprised", since they share the "sylvie" tag.

For Ren'Py to find the image files, they need to be placed in the game directory of the current project. The game directory can be found at "Project-Name/game/", or by clicking the "Game Directory" button in the launcher. You'll probably want to copy the image files from the "the_question/game/" directory into the "my_question/game/" directory, so you can run this example.

Ren'Py does not make any distinction between character and background art, as they're both treated as images. In general, character art needs to be transparent, which means it should be a PNG file. Background art can be JPEG or PNG files. By convention, background images start with the "bg" tag.

**Hide Statement.** Ren'Py also supports a hide statement, which hides the given image.Ren'Py的同时还支持一段声明，其中隐藏了给定的图像。

```
label leaving:

    s "I'll get right on it!"

    hide sylvie

    "..."

    m "That wasn't what I meant!"
```

It's actually pretty rare that you'll need to use hide. Show can be used when a character is changing emotions, while scene is used when everyone leaves. You only need to use hide when a character leaves and the scene stays the same.

它实际上是相当罕见的，你需要使用隐藏。显示可当角色正在发生变化的情绪被使用，而每个人都离开现场时使用。你只需要使用隐藏字符叶和现场保持不变的时候。

## Transitions 转场

Simply having pictures pop in and out is boring, so Ren'Py implements transitions that can make changes to the screen more interesting. Transitions change the screen from what it looked like at the end of the last interaction (dialogue, menu, or transition), to what it looks like after any scene, show, and hide statements.

只要有图片弹出进出很无聊，所以Ren'Py的实现过渡，可以更改画面更有趣。转换改变从它看起来像在最后的互动（对话，菜单，或过渡）的结束，以什么样子任何场景，显示和隐藏报表之后的屏幕。

```
label start:
    scene bg uni
    show sylvie smile

    s "Oh, hi, do we walk home together?"
    m "Yes..."
    "I said and my voice was already shaking."

    scene bg meadow
    with fade

    "We reached the meadows just outside our hometown."
    "Autumn was so beautiful here."
    "When we were children, we often played here."
    m "Hey... ummm..."

    show sylvie smile
    with dissolve

    "She turned to me and smiled."
    "I'll ask her..."
    m "Ummm... will you..."
    m "Will you be my artist for a visual novel?"
```

The with statement takes the name of a transition to use. The most common one is dissolve which dissolves from one screen to the next. Another useful transition is fade which fades the screen to black, and then fades in the new screen.

When a transition is placed after multiple scene, show, or hide statements, it applies to them all at once. If you were to write:

```
 scene bg meadow
    show sylvie smile
    with dissolve
```

Both the "`bg meadow`" and "`sylvie smiles`" would be dissolved in at the same time. To dissolve them in one at a time, you need to write two with statements:

无论是“`bg meadow`”和“`sylvie smiles`”将被叠化在同一时间。要一次将它们叠化于一身，你需要写两个with语句：

```
    scene bg meadow
    with dissolve
    show sylvie smile
    with dissolve
```

This first dissolves in the meadow, and then dissolves in sylvie. If you wanted to instantly show the meadow, and then show sylvie, you could write:

```
    scene bg meadow
    with None
    show sylvie smile
    with dissolve
```

Here, None is used to indicate a special transition that updates Ren'Py's idea of what the prior screen was, without actually showing anything to the user.

## Positions 位置
