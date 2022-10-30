# 如何创建一个有吸引力的，定制的桌面 HUD 与雨量计

> 原文:[https://life hacker . com/how-to-create-an-attractive-customized-desktop-hud-wit-5828789](https://lifehacker.com/how-to-create-an-attractive-customized-desktop-hud-wit-5828789)

Rainmeter 是一个强大的工具，让您创建一个美丽的，信息丰富的平视显示器，跟踪您的系统状态，RSS 提要和其他大量的信息。以下是如何使用它来为你的 Windows 桌面制作一个令人敬畏的、类似钢铁侠的 HUD。

Watch

<small>***更新** :*</small> [<small>*雨量计 4.0*</small>](https://www.rainmeter.net/release-4-0)<small>*本周早些时候掉了，所以我们决定大修我们的初学者指南。你可以查看这篇文章来了解更多关于*</small>[<small>*4.0 中所有可爱的新功能，包括矢量图形、更简单的皮肤创建等等。*T29】</small>](http://lifehacker.com/rainmeter-4-0-is-now-available-packs-in-new-skin-creat-1790714436)

Windows 定制 app [雨量计](http://rainmeter.net) 是我们特色桌面系列 的 [的常客，理由很充分。它有大量不同的配置选项，让您可以完全按照自己的喜好定制桌面的几乎每个像素，而且它看起来棒极了。一旦设置好，它就非常强大和有效，但是它不是非常用户友好。本演练将带您开始走上桌面定制的幸福之路，没有任何烦恼。](http://lifehacker.com/most-popular-featured-desktops-of-2016-1790295044)

### 安装雨量计并学习一些基本术语

雨量计安装非常简单。 [从这里](https://www.rainmeter.net/) 下载，运行. exe，你可以选择完全安装，也可以选择便携安装，把所有东西都放在一个文件夹里，可以从闪存盘上运行。

一旦安装完毕，开始使用 Rainmeter 的最大障碍就是它的术语。该应用程序使用的一些术语与其他应用程序不同，当你开始使用时，可能会非常混乱。因此，为了确保我们从同一页开始(并使用 Rainmeter 的语言)，这里有一个快速的术语表:

*   **皮肤:**rainmet 所说的皮肤，我们其他人通常称之为“widgets”。它们是在你的桌面上，在你的窗户下面的小应用程序。您可以有一个 RSS 皮肤、一个 Now Playing 皮肤、一个时钟皮肤等等。有些皮肤可能非常复杂，类似于小应用程序本身。术语“皮肤”指的是小部件是什么，而不是它看起来像什么。
*   皮肤套件:皮肤创建者可以将一堆外观相似的小部件捆绑在一起，称为“皮肤套件”例如，Rainmeter 附带了一个名为“illustro”的默认皮肤套件(见上图左侧)。您可以混合不同套件的皮肤，但它不一定看起来非常有凝聚力，所以通常您希望坚持使用特定的套件。
*   布局:一个布局定义了你的皮肤在桌面上的位置。按照您喜欢的方式配置桌面后，您可以将其保存为布局并在以后重新加载。这样，你可以有一个极简主义的主题，只有一个小侧边栏，在你工作的时候有需要知道的信息，和一个更大的主题，有两个侧边栏，更多的小部件，和一个任务栏，当你可以分心的时候。

Rainmeter 附带了一个名为 illustro 的简单皮肤套件，因此我们将在许多示例中使用它。如果你不是 illustro 的粉丝，你可以在开始之前下载几个皮肤套件。

### 找到并下载适合您风格的完美皮肤套件

illustro 套件是一个很好的起点，但还有很多令人惊叹的套件可供尝试。你可以从我们的 [特色桌面](http://lifehacker.com/featureddesktop#_ga=1.91286362.1347662518.1465819317) 系列开始，读者可以在这里分享他们最喜欢的定制工作区。你也可以看看 [雨量计论坛](https://forum.rainmeter.net/viewforum.php?f=27) ， [雨量计设计者小组](https://rainmeter.deviantart.com) ，或者 [雨量计子论坛](https://www.reddit.com/r/Rainmeter/) 来寻找一个庞大的粉丝群体来制作自己的皮肤。我偏爱 [Enigma](http://enigma.kaelri.com/downloads/) (我们也会用它来举例子)，还有 [Omnimo UI](http://omnimo.info/) 这是一个极其强大的皮肤集合，使用了 Windows 10 的扁平、多彩的设计方案。

一旦你找到了一些你喜欢的皮肤，有两种方法可以安装它们。一些皮肤套件带有。rmskin 文件。有了这些，你只需双击文件，然后在弹出的窗口中点击安装。您也可以选择在安装完成后立即应用新布局。

其他皮肤必须手动安装。这些通常以. zip 或。rar 存档，不包含 an。rmskin 文件。为此，请遵循以下步骤:

1.  下载。包含您想要的皮肤的 zip 文件。
2.  将文件夹的内容提取到计算机上的\Documents\Rainmeter\Skins。
3.  当它完成提取后，右键单击系统托盘中的雨量计图标。
4.  单击全部刷新。

现在，你将有新的皮肤可在雨量计。一些自定义皮肤套件包括预建的布局，所以你只需点击几个按钮就可以得到一个全新的桌面。其他的需要一点调整。我们将使用 illustro 和 Enigma 来回顾两者的基础知识。

### 按照您想要的方式添加和排列您的皮肤

当你第一次加载 Rainmeter 时，你应该会在你的屏幕上看到一些皮肤。你可以点击并拖动它们，将它们排列在一起，如果它们包含链接(比如 RSS 皮肤)，你可以点击里面的信息。您还可以通过几次点击来添加新的皮肤。例如，下面是如何从 illustro 套件添加回收站外观:

1.  右键单击任何打开的皮肤。
2.  转到 illustro >回收站。
3.  点击【回收站. ini】

如果你想删除一个皮肤，右击它并点击“卸载皮肤”您还会注意到，当您右键单击一个皮肤时，每个皮肤都有自己的“设置”菜单。在这里，你可以调整一些方便的设置。以下是一些最有帮助的:

*   **位置:**在这里，你可以设置皮肤出现的位置。您可以让一些外观显示在其他外观的上面，或者选择它们显示在哪个显示器上。
*   **透明度:**这可以让你自定义透过皮肤能看到多少。请注意，许多皮肤套件已经包含了一些半透明的元素，但是如果您想更多地透视您的桌面，您可以在这里进行调整。
*   **鼠标悬停时隐藏:**这将在光标悬停时隐藏皮肤。如果你想在你的工作上保持一个皮肤，但是不想让它妨碍你的工作，这是很方便的。
*   可拖动:这可以让你移动你的皮肤。一旦你对它们的位置感到满意，关闭它来锁定你想要的皮肤。
*   **点击通过:**启用此选项后，您将无法点击皮肤。相反，你会点击它下面的任何东西。这类似于鼠标悬停时的隐藏，除了你仍然可以看到你的皮肤。
*   **贴齐边缘:**当你在排列几个皮肤时，这有助于确保它们都在一条完美的线上。因为没有比差一个像素的皮肤更糟糕的了。

对于大多数用户来说，在配置布局时，可拖动和对齐边缘选项将是最有用的。之后，您可能想要关闭可拖动功能，这样就不会不小心移动任何东西。

### 配置您的皮肤，实现最大程度的定制

一些皮肤开箱即用:时钟显示时间，回收站显示你有多少项目在垃圾桶里。其他的，比如 RSS 皮肤或 Disk 皮肤，需要一些配置来知道要监视哪些磁盘或提要。对于某些套件，您需要仔细阅读配置文件，而其他套件则有更简单的选项面板。下面以 illustro 套件和 [英格玛套件](http://enigma.kaelri.com/downloads/) 为例，介绍如何编辑这两者。

#### 通过配置文件编辑皮肤

illustro 套件只能使用每个皮肤的配置文件进行编辑。例如，默认情况下，磁盘皮肤(在第一次安装 Rainmeter 时应该是活动的)只显示 C:和 D:驱动器。如果你更喜欢显示器，比如说，E:而不是 D:，你需要编辑皮肤。这意味着编辑它的配置文件。为此，请按照下列步骤操作:

1.  右键单击磁盘皮肤，点击“编辑皮肤”这将在记事本中打开“2 Disks.ini”配置文件。
2.  按 Ctrl+F 并搜索`D:`
3.  用`E:`替换`D:`的每个实例
4.  保存。ini 文件并退出记事本。
5.  右键单击磁盘外观，然后单击“刷新外观”

这是一个非常简单的编辑，但是它让您知道即使您不是程序员，也可以对皮肤进行非常小的调整。一般来说，只要花几分钟浏览一下配置文件，您就会知道什么是可编辑部分，以及每个部分的作用。我建议在最初几次编辑时备份原始的配置文件(例如，复制一份并在名称中添加`.bak`),这样如果你搞砸了什么，你可以随时将原始值粘贴回来。

如果你想潜得更深，你可以在这里 查看 [雨量计文档。你会发现大量的指南解释 Rainmeter 如何工作，如何编写你自己的皮肤，以及如何调整你找到的皮肤。你也应该](https://docs.rainmeter.net/manual/) [去看看雨量计论坛](https://forum.rainmeter.net/) 去寻找能给你指明正确方向的有用用户。使用预制的雨量计皮肤，你不需要做这些，但是如果你决定要自己制作，这个社区会很有帮助。

#### 通过套件的选项编辑皮肤

一些套件， [，像英格玛](http://enigma.kaelri.com/downloads/) ，包含选项窗口，让你定制它们而不需要通过配置文件。要调整这些设置，请按照下列步骤操作:

1.  右击打开的英格玛皮肤。
2.  前往英格玛>选项
3.  点击 Options.ini

现在您将看到一个显示 Enigma 版本信息的皮肤。在旁边，有一个图标栏。单击齿轮图标，调整要监控的磁盘驱动器或存储笔记的位置。点按音乐图标以更改播放音乐的应用程序。你可以在这里为所有的 Enigma 套件的皮肤改变大量的选项。这比编辑配置文件容易得多，大多数最好的套件都有这样的选项面板。

### 保存并在更有用的布局之间切换

有这么多真棒雨量计皮肤，你可以创建一个完美的工作和娱乐皮肤集合。如果您想要在需要某些工具时在它们之间切换，您可以使用 Rainmeter 的布局工具来保存不同的工作空间并在不同的工作空间之间切换。要访问布局功能，请按照下列步骤操作:

1.  右键单击任何打开的外观。
2.  转到雨量计，然后单击管理。
3.  单击布局选项卡。

在这里，您可以用新名称保存当前布局。例如，你可以用几个工具创建一个布局来帮助你在工作时监控你的电子邮件和时间。然后，当你想玩的时候，你可以用一些 [令人敬畏的质量效果主题皮肤](http://www.deviantart.com/art/Mass-Effect-Skin-173867458) 创建一个单独的布局。当您想要在现有布局之间切换时，可以通过以下步骤更轻松地完成:

1.  右键单击任何打开的外观。
2.  前往雨量计>布局
3.  单击要应用的布局。

一些皮肤套件也包含了现成的布局，所以当你第一次下载一个新的套件来检查它们的时候，检查一下布局管理器。

* * *

一开始 Rainmeter 可能会非常令人困惑，但是一旦你掌握了基本知识，你应该能够通过一点点的修改来创建一个非常时髦的、信息丰富的桌面。当然，如果你深入研究配置文件、自定义皮肤和其他好东西，你可能需要更多的指导，所以如果你有任何问题，请前往 [雨量计文档](http://rainmeter.net/RainCMS/?q=Documentation) 。