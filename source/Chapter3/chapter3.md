
 3中枢论元的标注细则
====================

3.1总述
-------

中枢论元由核心述谓概念充当。标注时，用依存弧将root指向中枢论元，而并不标注中枢论元的具体语义角色。对于中枢论元的标注，简单总结，就是找出一个语义事件的核心述谓概念。

然而，中枢论元与述谓概念之间的关系并非简单的一一对应。有些语义事件，没有典型的核心述谓概念；有些语义事件，包含多个述谓概念。对于这两种情况，我们需要分开讨论。

从中枢论元的角度来看，在汉语句子里，谓词性成分和体词性成分都可以充当中枢论元，谓词性成分又可细分为两种类型：动词充当中枢论元的情况以及形容词充当中枢论元的情况。（详见3.2节与3.3.1节）

从述谓概念的角度来看，一个语义事件往往不止一个述谓概念，有的述谓概念是核心述谓概念，是root（详见3.3.2节）；而有些述谓概念不是核心述谓概念，比如有些形式动词、情态动词（详见3.4节）；有的述谓概念转位做指称概念（详见5.2节）；有的述谓概念激起的语义事件是一个更大语义事件的组成部分，即降级关系（详见5.3节），有的述谓概念组合形成语义事件链（详见5.4节）；；不同的述谓概念之间又组合形成特殊的结构类型，比如连谓、兼语等结构（详见3.5节）。每一种类型，都需要标注细则。

语义依存图标注体系需要对句子中的每一个成分进行分析，这个过程是对语义关系的解析与重组。关键步骤就是对语义事件中出现的谓词进行分析，确定谁是中枢论元；然后就是句子中间的其他成分进行分析，将有语义关系的词对用依存弧连接起来。

3.2体词性成分充当中枢论元
-------------------------

体词性成分包括体词和体词短语，从词类划分角度来说，包括名词、数词、量词以及人称代词。体词是与谓词相对的概念。体词性成分充当中枢论元，主要用来判断或说明事物的种类数量、时间性质、特点用途等。一般来说，体词性成分不能充当谓语，只有以下情况才可以：

1.  只能是肯定句，不能是否定句；

2.  只能是短句，不能是长句；

3.  一般只能是口语句式，不能是书面语句式；

4.  限于说明时间、天气、籍贯、年龄、容貌、数量等的口语短句。

从以上四种限制条件来看，体词性成分充当中枢论元时，主要包括三种类型：

1.  时间词作谓语；

2.  名词性偏正结构作谓语；

3.  数量词和数量名结构作谓语。

对于名词谓语句，root直接指向体词性成分的中心词。

例如：这孩子圆圆的脸蛋。（root，脸蛋）

分析：该句中，"脸蛋"是中心词，故将root指向它，而"孩子"，"圆圆"，"。"这三个成分与脸蛋有语义关系，所以用依存弧标示出来，其他成分之间的语义关系也要标注出来。

标注结果用依存图结构表示如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\{J3\@KW1I83ZAHO9\`C@\~AR%P.png](../media/image010.gif){width="3.5833333333333335in"
height="0.9555555555555556in"}

图 7体词性成分做中枢论元示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\%I1PE16LUO\[D2QIO\@9MWM0C.png](../media/image011.png){width="3.65625in"
height="1.0208333333333333in"}

图 8体词性成分做中枢论元示例2

正是因为体词性成分充当中枢论元有诸多限制条件，所以形成的多是单一语义事件，易于标注。但是，有一种情况需要特殊注意，那就是"的"字短语充当中枢论元的情况。"的"字短语是由助词"的"附着在实词或短语后面组成，指称人或事物，属于名词性短语。"的"字短语一般作主语、宾语，但是也能出现在名词谓语句中。

例如：这本书\|\|新买的。（root，买）

分析：在这个句子里，
"买的（V+的）"构成的是一个具有指称概念的名词短语，复指主语"这本书"。在对"的"字短语进行标注时，我们将"的"字作为结构中心，其他成分按照实际语义关系进行标注。这样处理的原因在于，"的"字结构中的"的"与普通的助词"的"的语义内涵不同，需要特殊标注出来。

标注结果用依存图结构形式表示如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\5EP6Q0PRVINPXE\[OJ\$CI\$78.png](../media/image12.gif){width="3.09375in"
height="0.8930555555555556in"}

图 9体词性成分做中枢论元示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\TJW\]J86AO\`A\$08KT3\`AC%M5.png](media/image13.png){width="3.0625in"
height="0.9631944444444445in"}

图 10体词性成分做中枢论元示例4

3.3谓词性成分充当中枢论元
-------------------------

谓词性成分包括谓词和谓词短语，从词类划分的角度来说，包括动词、形容词和代替动词、形容词的代词。谓词是与体词相对的概念。谓词性成分充当中枢论元，主要指动词谓语句和形容词谓语句这两种情况。

### 3.3.1形容词充当中枢论元 

形容词充当中枢论元的情况在句法上体现出来的主要是形容词谓语句，用来描写人或物的形状、性质、特征等，以形容词为核心。当形容词充当中枢论元的时候，一般也不会出现复杂的长难句，所以在实际标注时，直接将root指向该形容词。

例如：宝塔很高。（root，高）

标注结果依存图结构表示如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\]041%\_PA\@ALRU)\~Z\@ZU\[%2H.png](media/image14.png){width="2.21875in"
height="0.8125in"}

图 11形容词充当中枢论元示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\_}WF\]\$8\~L7KZDDH\@W0EDHVW.png](media/image15.png){width="2.14375in"
height="0.6458333333333334in"}

图 12形容词充当中枢论元示例2

简单来说，形容词充当中枢论元并构成简单语义事件的情况如上介绍所示。然而，形容词与动词的组合也会构成复杂语义事件，这个时候，需要判断不同述谓概念之间的语义联系。一般来说。如果句中出现多个形容词并列充当述谓概念时，将第一个形容词标注为中枢论元root，其余形容词标注按照语义关系与root形容词进行连接即可。

例如：她时而开心，时而忧愁，性格阴晴不定。（root，开心）

分析：这个句子中出现了三个形容词："开心、忧愁、阴晴不定"，相当于三个语义事件。"开心"和"忧愁"是并列关系，而"阴晴不定"是对前两种关系的总结。我们将root指向第一个形容词"开心"。

标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\1\~7G@)ANQB\@99\~3XQ\~TFML4.png](media/image16.png){width="5.768055555555556in"
height="0.8659722222222223in"}

图 13形容词充当中枢论元示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\MDL)J3)6E7\~ONIKKABLY0\[C.png](media/image17.png){width="5.767361111111111in"
height="0.8020833333333334in"}

图 14形容词充当中枢论元示例4

### 3.3.2动词充当中枢论元

动词充当中枢论元选择中枢论元最复杂的一类情况。从句法上说，不仅涉及到单句，还涉及到复句、紧缩句等；从语义上说，不仅涉及到单一事件，还涉及到事链。主要用来叙述人或物的动作行为、发展变化等。下面我们分情况讨论事件中动词充当中枢论元的情况。

1.  **语义事件中只有一个动词的情况。**

当语义事件中只有一个动词时，将root指向这个动词。一般来讲，这个动词多是动作行为动词。

> 例如：公司处分了旷工者。（root，处分）

分析：该事件只有一个动词"处分"，所以将root指向"处分"，其余标注成分按照语义关系进行标注，标注结果用依存图形式表示如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\NF2Y7N(N4F\[6\[)@%JF0\@OZR.png](media/image18.png){width="3.78125in"
height="0.9993055555555556in"}

图 15动词充当中枢论元示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\%4\$\[O\]T9\_\_)QAER)L1(\]ETS.png](media/image19.png){width="3.8020833333333335in"
height="0.9138888888888889in"}

图 16动词充当中枢论元示例2

2.  **语义事件中有多个动词的情况。**

当语义事件中出现多个动词时，默认情况是将核心述谓概念作为中枢概念root的，但真实语言情况复杂多变，我们需要注意复杂的语言现象中找出核心的述谓概念。比如以下情况。

1.  现在着手进行一些小的调查。（root，着手）

2.  它们正在进行研究。（root，研究）

例1中有两个动词------"着手"和"进行"，进行的语义较虚，所以把root指向"着手"；同理，例2将root指向研究，尽管从语言学上讲，研究已经"名词化"了，但是相对于进行来说，它依然是这一语义事件的核心述谓概念。以例1为例，标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\3F}A\_J2\]HJ7\_6%{1@\]VJ9}H.png](media/image20.png){width="4.364583333333333in"
height="1.1777777777777778in"}

图 17动词充当中枢论元示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\{GJ(888UKV%\$P6SI1\$I{GQ3.png](media/image21.png){width="4.5in"
height="1.1694444444444445in"}

图 18动词充当中枢论元示例4

3.  他一边写作业，一边听歌。（root，写）

例3从句法上讲，是一个并列复句，从语义上讲，是一个事链。两个动词"写"和"听"对于这个事链的贡献值是一样的。所以，我们默认将root指向第一个述谓概念。标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\)RC\[XVTJ0\[N\@Q6(UP\]H{RXB.png](media/image22.png){width="4.78125in"
height="0.9777777777777777in"}

图 19动词充当中枢论元示例5

> ![C:\\Users\\cheng\\Documents\\Tencent
> Files\\1501808365\\FileRecv\\MobileFile\\Image\\H2I50VG5WC\]RYSX07){%)XU.png](media/image23.png){width="4.435416666666667in"
> height="0.8854166666666666in"}

图 20动词充当中枢论元示例6

4.  我希望他来。（root，希望）

5.  他来不来还不知道。（root，知道）

例4和例5都涉及到了主谓短语充当某一句法成分的情况。例4是主谓短语做宾语，例5是主谓短语做主语句。这时候，两个动词在语义事件上的地位是不平等的，即这个主谓短语是做了核心动词的一个论元，具体来说，就是"他来"是希望的一个客事角色。所以我们将root指向句子主干中的述谓概念，主谓短语中的述谓概念做降级关系处理。以例4为例，标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\~JH(VS}45CQJ\_\`L0C@)NOR6.png](media/image24.png){width="2.5625in"
height="0.5395833333333333in"}

图 21动词充当中枢论元示例7

> ![C:\\Users\\cheng\\Documents\\Tencent
> Files\\1501808365\\FileRecv\\MobileFile\\Image\\S351(\@V\]0B){U\[2FCUHJ\_6A.png](media/image25.png){width="2.9895833333333335in"
> height="0.6131944444444445in"}

图 22动词充当中枢论元示例8

6.  他看着剪下来的地图。（root，看）

例6中也有两个动词，"看"和"剪"。但是动词"剪"在这里并不是一个述谓概念，而是转位做了指称概念，充当一个修饰成分，所以root指向"看"，而"剪"被标注为反关系。标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\[\$RBU3J9L\]ET1L7CDOVXF\[1.png](media/image26.png){width="4.104166666666667in"
height="1.1333333333333333in"}

图 23动词充当中枢论元示例9

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\16{B0WUL6\[5PPM9{4%2XC6J.png](media/image27.png){width="4.479166666666667in"
height="1.25in"}

图 24动词充当中枢论元示例10

更详细的标注细则，在后文中皆有叙述。

3.  **语义事件中既有动词也有形容词的情况。**

主要有两种情况：

如果句子是形容词和动词联合构成复杂语义事件时，我们将root指向第一个述谓概念。对比下面两个例句：

1.  他从小就很聪明，非常喜欢买书、读书。（root，聪明）

2.  孙中山长得像他的母亲，性格比较安静。（root，长）

例1中有四个述谓概念，分别是"聪明、喜欢、买、读书"，我们默认将root指向第一个述谓概念------形容词"聪明"。例（2）有两个述谓概念，分别是"长、安静"，我们默认将root指向第一个述谓概念------动词"长"。

也就是说，当语义事件中，同时出现形容词和动词并构成复杂语义事件时，谁是中枢论元不是按照词类确定的，主要看谁的位置在前。

3.4特殊谓词的标注细则
---------------------

上文已经提及，单一语义事件中也会出现多个动词的情况。在选定了中枢论元root后，如何对于剩余动词进行合理的标注，是一个亟待解决的问题。《现代汉语》将动词分为七种意义类别，分别是动作行为动词、心理活动动词、存在变化消失类、判断动词、能愿动词、趋向动词以及形式动词。动作行为动词一般表示主体的动作行为，经常做语义事件的中枢论元。在此，我们再举出几个例子：

1.  他送给我一本新词典。（root，送）

2.  一个游击队员突然说。（root，说）

3.  门关得严严的。（root，关）

4.  那件事原来是他搞的。（root，搞）

上述例（1）（2）（3），"送、说、关"等都是动作行为动词，我们将root指向这些动词。例（4）的"搞"虽然意义比较虚，我们还是将root指向它。

但是，我们再看几个例子：

5.  外商到中西部地区进行投资。

6.  他拿出一本书来。

7.  这可能会改变我们的生活。

这三个例子都是单一语义事件，但是都包含了不止一个动词，例（5）有形式动词"进行"，例（6）涉及到趋向动词"出来"，例（7）包括了能愿动词"可能"和"会"。结合语义我们得知，每一个语义事件的核心述谓概念都不是这些辅助性的动词，而是那些具有明显动作行为的动词。试比较下面两组句子：

a)外商到中西部地区投资。 b) \*外商到中西部进行

他拿一本书。 \*他出一本书来。

这改变我们的生活。 \*这可能会我们的生活。

a组和b组句子是例（5）到例（7）的变体，a组句子是将所有的心理活动动词、能愿动词去掉后的句子，我们发现，虽然句子的一些"情态义"消失了，但是句子的"命题义"并不受影响；b组句子是将动作行为动词去掉后的结果，我们发现，这些句子不能完整的表达一个清晰的语义事件。所以，我们将root指向那些动作行为动词。

接下来的问题是，对于表达一些"情态义"的述谓概念，我们如何标注。接下来，分别叙述判断动词、形式动词、趋向动词、心理活动动词以及能愿动词的标注细则。

### 3.4.1判断动词

判断动词"是"表示肯定，表示事物等于什么或属于什么；表示事物的特征、质料、情况等，也可以表示事物的存在。对于判断动词，我们需要注意一种特殊情况，即判断动词"是"与副词"是"之间的语义差别。

**1)判断动词"是"的标注情况。**

"是"字最常见的用法是放在两个名词（词或短语）中间，前面的名词是句子的主语。一般来说，判断动词出现在单一语义事件中，表达的含义简单清晰，"是"就是该语句的中枢论元，用依存弧将root指向"是"即可。例如：

1.  他是最好的老师。（root，是）

2.  这不是新书。（root，是）

这两个例句一肯一否，都是"是"作为判断动词的用法。"是"作为判断词，是一种特殊的动词，判断词加名词构成一个"合成谓语"。所以，"是"的客体角色是相对固定的，粗粒度标签是系事角色，细粒度标签为类事角色，而主体角色需要根据相应的语言情况进行标注。具体分析例2------"这"是一个范围角色，"书"是系事角色（类事角色），"新"是一个修饰角色，"不"是否定修饰。标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\7R{Y\]KHCNUBG59INS4\[K\@1U.png](media/image28.png){width="3.4895833333333335in"
height="0.6555555555555556in"}

图 25判断动词示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\LL9LV0\[\_YVHLNE\`JKBSJ4LL.png](media/image29.png){width="3.3541666666666665in"
height="0.7222222222222222in"}

图 26判断动词示例2

**2)副词"是"的标注情况。**

副词"是"常常用在谓语动词、形容词前，表示肯定的情况。这些情况中的"是"从语句语调的角度来看，需要重读，相当于"确实"的意思，不能省略。但是，"是"不重读的时候，可以省略，只表示一般的肯定，可以与句末语气词"的"配合构成"是......的"结构。不论重读还是轻读，副词"是"表示的都是语气上的含义。所以一般来说，我们将它的粗粒度标签标注为依附标记mDEPD，细粒度标注为情态标记mMod，依附在中枢论元上。例如：

1.  今天是很冷。（root，冷）

2.  他的家底老肖是知道的。（root，知道）

这两个例句分别是重读的"是"和轻读的"是"，都标注为依附标记。注意例（2）与"的"字短语的区别。

3.  他是卖菜的。（root，是）

例（2）与例（3）形式上都是"是......的"的结构，但是二者表达含义不同。例（2）是副词"是"，需要标注为依附标记，而例（3）是判断动词"是"，需要标注为中枢论元root。以例2为例，"老肖"是知道的主体角色（粗粒度为施事角色额，细粒度为感事角色），"他的家底"是"知道"的客体角色（粗细标签皆为当事角色），而"是"和"的"是依附标记。所以标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\BS72J\]}1OJK3\@AJ\]Q%\]X453.png](media/image30.png){width="4.041666666666667in"
height="1.1263888888888889in"}

图 27判断动词示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\`4{}H%5Y{YD02}YPX\@MX3RB.png](media/image31.png){width="4.010416666666667in"
height="1.1520833333333333in"}

图 28判断动词示例4

**3)其他"是"的标注情况。**

有时候，"是"在语句中出现的时候，形式上看起来似乎像是判断动词或者是副词，而实际上，它们是连词"不是、而是、还是、就是"等。这种情况，我们要将它们的粗粒度标签标注为关系标记mRELA，细粒度标签标注为连词标记mConj,依附在每一个语义事件的核心述谓概念上。例如：

1.  他在休息的时候，不是看书，就是看报。（root，看1[^3]）

2.  草地并不是金色的，而是绿色的。（root，是1）

例1中的"不是，就是"是表示选择关系的连词，我们将它们的粗粒度标签标注为关系标记mRELA，细粒度标签标注为连词标记mConj。例2中的"不是、而是"虽然从形式上看是连词，但是实际上是判断动词，真正的连词是"而"。第一个"是"是root，第二个"是"是表示选择关系的另一个事件，应该标注为eSelt（粗细粒度标签相同），依附在第一个"是"上。例2的标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\}E2\`FB\@J0BQ0\$TME4AB(ASW.png](media/image32.png){width="5.385416666666667in"
height="0.875in"}

图 29判断动词示例5

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\EGP3YO@(AN%4WR4X54CFZQI.png](media/image33.png){width="5.208333333333333in"
height="0.9381944444444444in"}

图 30判断动词示例6

**综上，"是"有三种标注情况：**

1.  判断动词"是"应该标注为中枢论元root；

2.  副词"是"标注为依附标记mDEPD（细粒度为mMod）

3.  由"是"构成的连词"不是、而是、就是"等标注为连词标记mConj。

### 3.4.2形式动词

形式动词一般是指"进行、加以、给以、给予、予以"等语义虚化的动词，它们是本身不具有实在意义而只能用动名词或以动名词为中心语的偏正短语作宾语的动词。从句法上说，"进行"的功能之一是将动词宾语名词化；而从语义上将，真正表示该语义事件动作行为的是形式动词后面的动词，而且后面动词的受事常常在前面。例如：对优秀员工进行表扬。实际的语义是"表扬优秀员工"。核心述谓概念是"表扬"而非"进行"，所以我们将root指向动词"表扬"，形式动词标注为依附标记mDEPD，细粒度标签为虚化标记mVain，依存于中枢论元上。例如：

1.  他们正在进行研究。（root，研究）

2.  此类活动必须予以制止。（root，制止）

分析：以句1为例，中枢论元是"研究"，"他们"是研究的主体，"正在"表示的是时间，而"进行"的作用是将研究名词化。所以，标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\@6E\`(3\]ZZWZA}WJ23%MLX58.png](media/image34.png){width="3.28125in"
height="0.9090277777777778in"}

图 31形式动词示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\7{\${HY)(DOCQ9\_\_QUZBK6Z8.png](media/image35.png){width="3.4375in"
height="0.9305555555555556in"}

图 32形式动词示例2

但是，有时候，这些形式动词可以"独当一面"，在语义事件中表达完整的动作，这个时候，我们把它们标注为root。例如：

1.  考试进行了三个小时。（root，进行）

2.  一切都在按计划进行。（root，进行）

分析：以句1为例，该句只有一个谓词，即进行，所以它被标注为中枢论元，考试是当事角色，三个小时是时间角色。所以，标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\8KQUCEHSL{R6\_CJNB8U\`\_}U.png](media/image36.png){width="3.7291666666666665in"
height="1.0152777777777777in"}

图 33形式动词示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\7JBR2VN{FS\`\`\~KVZCAYMIWT.png](media/image37.png){width="3.6770833333333335in"
height="1.0166666666666666in"}

图 34形式动词示例4

注意区分一种情况，"开始继续"类动词。这几个动词有实际意义，同时也有虚化的倾向，但是又没有虚化到像形式动词一样，可以省略或者被其他意义很虚的词替代的地步。所以，我们仍然将root指向它们。

例如：从明天开始干。（root，开始）

分析："开始"和"干"都是动词，似乎都可以充当中枢论元，但是我们规定将root指向了"开始"，而"干"是"开始"的一个后继动作，所以标注为后继事件关系。标注结果用依存图结构表示如下：

> ![C:\\Users\\cheng\\Documents\\Tencent
> Files\\1501808365\\FileRecv\\MobileFile\\Image\\(PF\_\]2JGG{JD{\_7DA2L\$\[\_4.png](media/image38.png){width="3.1458333333333335in"
> height="0.79375in"}

图 35形式动词示例5

> ![C:\\Users\\cheng\\Documents\\Tencent
> Files\\1501808365\\FileRecv\\MobileFile\\Image\\69HB}CLVYG\~84CCA4KN2P0T.png](media/image39.png){width="3.2708333333333335in"
> height="0.8125in"}

图 36形式动词示例

> **综上，形式动词有两种标注情况：**

1.  形式动词与其他动词结合，意义虚化时，标注为依附标记mDDEPD，细粒度标签为虚化标记mVain，依存于中枢论元；

2.  形式动词单独出现，表达完整的语义，标注为root。

### 3.4.3趋向动词

趋向动词表示移动的趋向，可以单独作谓语或者谓语中心，但是经常用在别的动词或者形容词的后边表示趋向，作趋向补语。趋向动词是一个封闭的词类，有单音节的，也有多音节的，多音节的趋向动词可以合用，也可以连用。所有的趋向动词如下表所示：

表格 6趋向动词总表

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\X{I)W3\_LQ5\~Z\]\_NB9)UOER3.png](media/image40.png){width="4.520833333333333in"
height="1.2513888888888889in"}

根据不同的用法，趋向动词也有不同的标注方法。

**1）单独作谓语或者谓语中心的情况。**

趋向动词单独作谓语或谓语中心的时候，我们将root指向这个趋向动词。

例如：月亮下去了，太阳还没有出来。（root，下去）

分析：本句中的"下去"和"出来"都是趋向动词，我们将root指向第一个趋向动词"下去"，而"出来"是前一句的一个后继事件，依附在"下去"上，标注为后继事件关系eSucc。标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\_P1K\$LY{H\`1\$UY8WET63)8U.png](media/image41.png){width="4.416666666666667in"
height="1.0576388888888888in"}

图 37趋向动词示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\_P1K\$LY{H\`1\$UY8WET63)8U.png](media/image41.png){width="4.510416666666667in"
height="1.086111111111111in"}

图 38趋向动词示例2

**2）作趋向补语的情况。**

相比于趋向动词单独作谓语或者谓语中心的情况，趋向动词依附于别的谓词后面表示趋向补语，是更常见的情况。这种情况，按照粗粒度标注标签，统一标注为mDEPD，按照细粒度标注标签，根据不同的语义倾向，可以细分为趋向标记mDir，时间标记mTime等。且看如下一些例子：

1.  企业产权转让的收入，要集中\<起来\>再投资。（root，集中）

2.  没有任何资料显示他们破坏\<过\>这些资料。（root，显示）

3.  拿\<出来\>一本书 VS拿\<出\>一本书\<来\>（root，拿）

例1中的"起来"是趋向标记mDir，例2中的"过"是时间标记mTime。都依附于之前的动词做趋向补语，粗粒度标签为mDEPD。前文讲过，趋向补语可以分开使用，例3中当"出来"合用时，依存弧指向"拿"，当"出来"分开用时，将"出"指向"拿"，"来"指向"出"，粗粒度标签标注为依附标记mDEPD，细粒度标签分别标注为趋向标记mDir和离合标记mSepa。有时候趋向动词做补语时意义非常虚化，例如口语中常说的"说起来、谈起来、想起来"等，我们也都将粗粒度标签标注为mDEPD，细粒度标注为虚化标记mVain。以句3为例，标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\JATY3\~Q8\@W3OK)12OK6\[FV8.png](media/image42.png){width="3.625in"
height="1.03125in"}

图 39趋向动词示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\VAB\$T4LJHPH\_RMJU4BJELIF.png](media/image43.png){width="3.6770833333333335in"
height="1.1388888888888888in"}

图 40趋向动词示例4

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\(MK\`WPP\`Y(%X631RN\$I(QWH.png](media/image44.png){width="3.78125in"
height="0.925in"}

图 41趋向动词示例5

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\77Y)I%8BI61}8\[DZ76J8%Q9.png](media/image45.png){width="3.21875in"
height="0.8395833333333333in"}

图 42趋向动词示例6

**综上，趋向动词有两种标注情况：**

1.  单独作谓语或者谓语中心时，标注为中枢论元root；

2.  跟在谓词后作趋向补语时，标注为依附标记mDepd，细粒度标签根据实际语义情况，可以是时间标记mTime、趋向标记mDir等。

### 3.4.4心理活动动词

心理活动动词是表示心理活动的动词，其中一些又有一定感情色彩，例如"爱、怕、恨、喜欢、羡慕、讨厌、敬佩、希望"等。心理活动动词与一般的动作行为动词相比，除了能受程度副词修饰之外，还有带宾语能力的不同。汉语中根据动词带宾语能力的不同，将只能带名词性宾语的动词称为"名宾动词"，把既能带名词性宾语，又能带为谓词性宾语的动词称为"名谓宾动词"。心理活动动词就是一种名谓宾动词。也正是因为这种可以带谓词性宾语的能力，使得心理活动动词常常会出现在兼语结构中。

实际上，如何对心理活动动词进行标注并不困难，直接将root指向它们即可，而且它们的主体角色一般都是感事角色Aft（粗粒度标注为施事角色AGT），复杂的是对心理活动动词后的其他成分的标注。有三种情况：

**1）心理活动动词带名词性宾语的情况。**

这种情况就是"主语+谓语+宾语（SVO）"的简单句，当谓语是心理活动动词是，主语一般是感事角色Aft，宾语是客事角色Cont，表达的是主体对于某一种事物的主观态度。

例如：台湾人平时都喜欢哪一类的音乐？（root，喜欢）

分析：本句中，"喜欢"是中枢论元root，而"台湾人"是"喜欢"的主体感事角色Aft，"音乐"是"喜欢"的客事Cont，需要提出的是，疑问代词"哪"依附在类上，表示的是类别的范围，所以标注为范围角色。标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\)O6V\_BXFFLZ\@F{V\[FYC5CM6.png](media/image46.png){width="5.2125in"
height="0.9791666666666666in"}

图 43心理活动动词示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\`CDI\_AN\`)HW@)\]}HOKZLC0X.png](media/image47.png){width="5.052083333333333in"
height="0.9305555555555556in"}

图 44心理活动动词示例2

**2）心理活动动词带谓词性宾语的情况。**

谓词性宾语往往是一个动宾结构的短语，整句的结构是"主语+谓语+动宾短语"，这时候一个语义事件中出现了多个谓词，其中，动宾短语整体是降级作了心理活动动词的宾语，所以标注时要将这种结构关系表示出来。

例如：我喜欢写作业。（root，喜欢）

分析：本句中，"喜欢"是中枢论元root，而"我"是喜欢的主体感事角色Aft，动宾短语"写作业"是"喜欢"的客事角色，又因为是降级关系，所以依存弧由"写"指向"喜欢"，标签为dCont，表示降级客事关系，而"作业"是"写"的客事角色Cont。标注写过如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\VEDMZ\$Q2O0}\[8}Z5\$F@%%\$2.png](media/image48.png){width="3.4375in"
height="0.8479166666666667in"}

图 45心理活动动词示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\@)L\@M{MA@\~50D\$Y0C\$PEHU6.png](media/image49.png){width="3.5833333333333335in"
height="0.9729166666666667in"}

图 46心理活动动词示例4

**3）心理活动动词出现在兼语结构中的情况。**

兼语结构有多种类型，心理活动动词是其中的一种情况。构成的句法结构是"主语N1+谓语V1+主语/宾语N2+谓语V2"。N2既是V1的宾语，又是V2的主语，我们可以理解为兼语，那么出现了多父亲节点的特殊现象；也可以理解为主谓短语做宾语，那么就出现了嵌套事件关系。标注的时候，我们要将这些语言知识表达出来。

例如：我喜欢她聪明。（root，喜欢）

分析：本句中，"喜欢"是中枢论元root，而"我"是喜欢""的主体角色，"喜欢"的客事是一个主谓短语"她聪明"，所以标注为dCont，依存弧由"喜欢"指向"聪明"，同时，"她"是"喜欢"的客事Cont，"她"又是"聪明"的主体当事角色Exp。完整的标注结构如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\6V0JEN\[MGAC8OXF\]%M32)XP.png](media/image50.png){width="4.09375in"
height="0.9270833333333334in"}

图 47心理活动动词示例5

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\ST454\[96RZ\`%FPX4\_3(VU5G.png](media/image51.png){width="3.8958333333333335in"
height="0.9479166666666666in"}

图 48心理活动动词示例6

综上，对于心理活动动词的标注很简单，直接将中枢论元root指向它即可，对于心理活动动词后的待标成分，需要重点分析。

### 3.4.5能愿动词

能愿动词又叫助动词，能用在动词、形容词前边表示客观的可能性、必要性和人的主观意愿，主要作用是评议动词、形容词。表可能的能愿动词有：能、能够、会、可能、可以、可等；表必要的能愿动词有：要、应、应该、应当等；表意愿的能愿动词有：肯、敢、要、愿、愿意等。要注意区别一种情况：有部分能愿动词除了能够用在动作行为动词之前做状语外，还可兼类作一般动词，例如"会说英文"VS"会英文"，前者中的"会"是能愿动词，表示可能性，整个短语的语义中心在"说"上面，而"会"只表示一种情态上的意义；后者中的"会"是一般动词，表示能力，能够。对于这种形式上易混淆的情况，我们分别进行说明。

能愿动词出现在动词、形容词前，一般做状语，整个语义事件的中枢论元是后面的谓词而非能愿动词，所以，我们将root指向后面的核心述谓概念，而将能愿动词指向核心述谓概念，粗粒度标签标注为依附标记mDEPD，细粒度标注标签为情态标记mMod。例如：

1.  他很快就要退休了。（root，退休）

2.  你敢不敢答应我。（root，答应）

分析：以句1为例，root为"退休"，"要"依附在"退休"上，标注为mDepd，表示这是一个依附性成分。标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\8SY%6Z6RU4G1(XUAQZCFU2Y.png](media/image52.png){width="4.083333333333333in"
height="1.0958333333333334in"}

图 49能愿动词示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\16\[49(5\`P\[\`2S9\[P\_YWI\`ZX.png](media/image53.png){width="3.9993055555555554in"
height="1.09375in"}

图 50能愿动词示例2

对于兼类的能愿动词作一般的动作行为动词时，我们根据实际语义关系，按照一般动词的情况进行标注即可。例如：

1.  我要一杯茶。（root，要）

2.  他会英文、法文、希腊文等三种外文。（root，会）

分析：本句中的"要"在这里是一个一般性的动作行为动词，标注为中枢论元root，"我"是主体角色，"茶"是客体角色。对应的标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\()WI\~R2DJ2IV(\[\@LJ2Q332M.png](media/image54.png){width="3.5729166666666665in"
height="0.9423611111111111in"}

图 51能愿动词示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\{F71\@A3EDRFTEX{ZM2\$\@7BC.png](media/image55.png){width="3.65625in"
height="0.9027777777777778in"}

图 52能愿动词示例4

综上，对于能愿动词，由于它们在语义事件中主要表达的是主体的一种主观态度，所以，我们不把root指向它们，而是将它们标注为依附标记。

3.5谓词特殊结构的标注细则
-------------------------

除了需要对特殊的动词进行必要的标注说明外，谓词也会构成一些特殊结构，这些特殊结构也需要规范化的细则。我们从两方面来说：

首先从谓词的内部结构看。汉语是一种缺乏形态变化的孤立语，但是有些动词会出现一些形态上的变化，主要是重叠以及离合。

其次从谓词的外部组合看。不同的谓词可以构成并列结构、兼语结构、连谓结构、中补结构。

对于上述各种特殊结构，接下来，我们逐一进行说明。

### 3.5.1重叠式

有些动词可以重叠，表示短暂、轻微的含义。

单音节动词的重叠式为"AA式"，例如："想想"、"说说"等。变体形式为"A一A式"或者"A了A式"。在实际待标语句中，由于分词结果，AA式重叠常常被分成一个词语，可以单独作一个述谓概念，而"A一A式"以及"A了A式"，在分词时常常被分成三个待标成分。标注时，我们把第一个A作为核心，依存弧指向第二个A，标注为语义依附标记mDEPD，细粒度标注标签为重复标记mRept，表示第二个A和第一个A实际是一个词，中间的插入成分粗粒度标签标注为依附标记mDEPD，细粒度标签标注为时间标记mTime（了）或者频次标记mFreq（一），也是依附在第一个A上。标注范式如下图：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\4\~ZXI89416RB\~I14%2J\`\_SY.png](media/image56.png){width="2.40625in"
height="0.71875in"}

图 53重叠式范式1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\%\]\$XIQJD43C0J97)L)AFD7H.png](media/image57.png){width="2.40625in"
height="0.65625in"}

图 54重叠式范式2

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\98\]\~O4MMPX9LDHM%P\@G}TPF.png](media/image58.png){width="2.3541666666666665in"
height="0.65625in"}

图 55重叠式范式3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\MM)RHV\`AT\]XMF15}\[J8{3}R.png](media/image59.png){width="2.3229166666666665in"
height="0.6666666666666666in"}

图 56重叠式范式4

例如：他说了说他的想法。（root，说1）

分析：本句中root指向第一个"说"，而"他"和"他的想法"分别是"说"的主客体角色。标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\~TINL1%W\@X6D\$M04U\]KW\$2G.png](media/image60.png){width="3.5104166666666665in"
height="0.9506944444444444in"}

图 57重叠式示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\(S5WTPMH@{OA)NS4)5(IFXC.png](media/image61.png){width="4.135416666666667in"
height="1.1194444444444445in"}

图 58重叠式示例2

双音节动词的重叠式为"ABAB式"，例如："研究研究"、"打扫打扫"等。分词的结果通常是AB/AB，，我们把第一个AB作为核心，第二个AB依附在其上，粗粒度标签标注为依附标记mDEPD，细粒度标注标签为重复标记mRept，表示这是一个重复性的话语。标注范式如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\$QSI3J\@DQ\@WA\~W1\]BT\`8B\$J.png](media/image62.png){width="2.0208333333333335in"
height="0.6666666666666666in"}

图 59重叠式范式5

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\9JFKV8\]\$VHZ)5SQ{PBVYB(P.png](media/image63.png){width="1.8541666666666667in"
height="0.6875in"}

图 60重叠式范式6

例如：我研究研究这个课题。（root，研究1）

分析：本句中，"研究1"是句子的中枢论元，"我"和"这个课题"分别是研究的主客体角色。标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\$)\~HF}D4BUW502YMKF(CD)N.png](media/image64.png){width="3.665277777777778in"
height="1.0277777777777777in"}

图 61重叠式示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\5{N3\_CXI{YP1L\]{9RVLJPIR.png](media/image65.png){width="3.6979166666666665in"
height="1.01875in"}

图 62重叠式示例4

在部分口语语料中，会遇到这样的情况。动宾短语加上语气，形成一个祈使句，并重复使用，表示一种呼喊或者命令。

例如：开会了，开会了！（root，开会1）

分析：我们同样把第二个"开会"作为第一个"开会"的重复成分，标注为标注重复标记mRept，粗粒度标签为依附标记mDEPD。结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\%30)M}2AJ7O4\$W8\$9\_1\_(ZO.png](media/image66.png){width="3.7291666666666665in"
height="0.79375in"}

图 63重叠式示例5

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\1\@ZU2J40KY\~%YF5\_\[7PD0L7.png](media/image67.png){width="4.072916666666667in"
height="0.7833333333333333in"}

图 64重叠式示例6

综上：动词的重叠式标注，无论是单音节重叠，还是双音节重叠，或者是口语中国句子的重叠，我们都将第二个重叠成分作为第一个成分的重复标记，粗粒度标注标签为mDEDP，细粒度标注标签mRept，依存弧由第一个成分指向第二个成分。

### 3.5.2离合式

离合词在语法研究上一直都是重点，比如"毕业、见面、游泳、散步"等，合用时是一个词，分开时是一个动宾短语，所以有人认为是短语，有人认为是词，还有人认为离则为短语，合则为词。正是由于离合词的可离可合的特点，在标注时也有不同的情况。

当离合词合用的时候，依据分词结果，是一个待标成分，不存在标注存疑的情况。

当离合词分开使用的时候，中间可以添加其他成分，例如"洗澡"、"洗个澡"、"洗个热水澡"等动宾短语，从语义上说，一般宾语是动词的客事角色，但是，在标注的时候，我们不将动词支配的宾语标注为该动词的离合标记mSepa。这是因为，离合标记连接的两个成分一定是动宾短语，而如果我们标注为普通动宾短语的话，就难以抽取出离合短语应有的结构特征。但是将细粒度标签升级为粗粒度标签的时候，要将离合标记升级成为客事角色CONT。这样的处理策略，既能在粗粒度标签体系下体现离合短语动宾结构的特征，又能在细粒度标签体系下对离合短语进行特殊化处理，彰显出汉语离合短语的特殊性。如果我们可以将离合词AB的形式表示为"A......B"的话，那么标注范式为：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\`CD{151UDH9V7ZBV8I}7T(Q.png](media/image68.png){width="2.59375in"
height="0.7604166666666666in"}

图 65离合式范式1

![C:\\Users\\cheng\\AppData\\Local\\Temp\\WeChat
Files\\5f675bca4844a4f117d6b6163a42b16.png](media/image69.png){width="2.4270833333333335in"
height="0.6784722222222223in"}

图 66离合式范式2

例如下面两个例句：

1.  我想洗个热水澡。（root，想）

2.  我想洗澡。（root，想）

分析：句1是离合词分开使用的情况，句2是离合词合用的情况。对于句1来说，"洗个热水澡"是"想"的降级客事角色dCont，中间添加的成分按照实际语义关系进行标注，比如"个"是"洗"的依附成分，"热水"是"澡"的修饰成分；而句2中"洗澡"合用，是"想"的客事角色。句1的标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\%5937\~2NQNM(LWSN8HQK\[ZB.png](media/image70.png){width="3.8541666666666665in"
height="1.0930555555555554in"}

图 67离合式示例1

![C:\\Users\\cheng\\AppData\\Local\\Temp\\WeChat
Files\\f524535d0df065337984b22e2a87142.png](media/image71.png){width="3.9583333333333335in"
height="1.09375in"}

图 68离合式示例2

句2的标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\[K\@T\~60C\[9\[S\@C7\${G\`9QL5.png](media/image72.png){width="3.1041666666666665in"
height="0.78125in"}

图 69离合式示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\2\~YA6CB8SREEGV{O1\~Y\$HBR.png](media/image73.png){width="3.0833333333333335in"
height="0.8958333333333334in"}

图 70离合式示例4

注意，离合式动宾短语的重叠形式是AAB，例如：洗洗澡，散散步。综合重叠式和并列式的标注细则，那么标注范式是：

![C:\\Users\\cheng\\AppData\\Local\\Temp\\WeChat
Files\\6688559d2de14ed8d6747310e9d904e.png](media/image74.png){width="1.5729166666666667in"
height="0.7680555555555556in"}

图 71离合式范式1

![C:\\Users\\cheng\\AppData\\Local\\Temp\\WeChat
Files\\d14f0e16a7a9d98f0c7f7bc5ad244d1.png](media/image75.png){width="1.7395833333333333in"
height="0.7548611111111111in"}

图 72离合式范式2

综上，动词的离合式，粗粒度标签标注为客事角色CONT，细粒度标签标注为离合标记mSepa。

### 3.5.3并列式

两个或两个以上意义相关、层次相同、句法功能相同、由并列连词连接起来的语法结构成为"并列结构"。很多词类都可以并列出现，而且可以出现在各种句法位置上，表达各种语义关系或充当各种语义角色。并列的各项之间可以互换位置，它们在逻辑上不互相依赖。例如，名词的并列可以作主体角色、客体角色，形容词的并列可以作修饰角色等。在这里，我们以动词的并列为例，对于并列式结构进行一个标准化的标注制订。

根据并列结构的定义，我们可以总结出几个关键性的成分：并列成分ABC等（至少两个），连词（以"和"为代表）、标点符号（以"、"为代表）。所以，并列结构可以表示为按照并列成分的多少以及种类分为以下三种情况：

**1.A、B**

**2.A和B**

**3.A、B和C。**

事实上，很多标注规范都对并列结构进行了详细的描述，标注的方法不尽相同，主要有以下几种形式:

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\EPS\[L\~0\@OEWNQ\[XN(C(7NTF.png](media/image76.png){width="1.8854166666666667in"
height="0.375in"}

图 73并列式举例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\WMQ}B\~AK89\[(XO3237RANH5.png](media/image77.png){width="1.96875in"
height="0.6979166666666666in"}

图 74并列式举例2

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\O{\[)G2G9W4\[T}VOY5GP\~GYB.png](media/image78.png){width="1.9479166666666667in"
height="0.75in"}

图 75并列式举例3

由图可见，争议点主要在于并列的成分中，谁是核心成分、标点依附于谁，连词又依附于谁的问题上。针对这些问题，**我们规定：**

1.  **并列式中的第一个成分为核心成分，其他并列成分依次依附于前一个并列成分，粗粒度标签标注为并列事件关系eCOO，细粒度标签为eCoo；**

2.  **标点依附于前一个成分，粗粒度标签为mPUNC，细粒度标签为mPunc；**

3.  **连词依附于后一个成分，粗粒度标签为mRELA，细粒度标签为mConj。**

> 所以上述三种情况的标注范式分别为：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\$I4ND6TTEUV\]O\_FT2RSVAYB.png](media/image79.png){width="2.2083333333333335in"
height="0.6145833333333334in"}

图 76并列式范式1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\D905\$JHYP{K\~\_VQP\`O1PWNV.png](media/image80.png){width="2.1666666666666665in"
height="0.6458333333333334in"}

图 77并列式范式2

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\9{\_8U)QVS64C\`NBL2X2J%(O.png](media/image81.png){width="2.09375in"
height="0.65625in"}

图 78并列式范式3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\I4WQ3LAI\[FIZM\_20%IK8\[M4.png](media/image82.png){width="2.0416666666666665in"
height="0.625in"}

图 79并列式范式4

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\RO5ERM(Y\[%2NU\@0NWR\]FX7T.png](media/image83.png){width="4.020833333333333in"
height="0.84375in"}

图 80并列式范式5

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\OVGV\_NSAZ4ZO)ZGANJF%64C.png](media/image84.png){width="3.90625in"
height="0.7916666666666666in"}

图 81并列式范式6

例如：他一个人吃饭、喝水以及睡觉。（root，吃饭）

分析：这个句子属于并列式的第三种类型，其中，"吃饭"是核心，标注为root，"喝水"依附在"吃饭"上，"睡觉"依附在"喝水"上，"顿号"依附在"吃饭"上，"以及"依附在"睡觉"上。不能忘记的是，"吃饭"、"喝水"以及"睡觉"的主体角色都是"他"，即"他"是一个多父亲节点的节点，实际上，并列结构常常会出现交叉弧现象。另外还有一个标注难点："他"和"一个人"的关系------"一个人"是对"他"的复指，相当于同位关系，所以细粒度标签标注为等同关系eEqu，而粗粒度标签标注为并列关系eCOO。所以标注结果如下所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\PFGW\~\~\@EW43(AK\[\[58VCDOP.png](media/image85.png){width="3.9895833333333335in"
height="1.0590277777777777in"}

图 82并列式示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\P7(XN012GRU\[9IDOR800QAD.png](media/image86.png){width="4.229166666666667in"
height="1.0833333333333333in"}

图 83并列式示例2

注意：并列相可以是词、短语也可以是句子。虽然严格来说。并列式短语与并列事件关系不是一回事，但是为节约语义标签，我们将它们都标注为eCoo，关于并列事件关系的标注，详见5.4小节。

### 3.5.4兼语式

兼语式是这样一种结构：由前一动词到的宾语兼做后一谓语的主语，即动宾短语的宾语和主谓短语的主语套叠，形成一个有宾语兼主语双重身份的"兼语"。有兼语的短语叫做兼语短语，由兼语短语充当谓语或独立成句的句子叫做兼语句。根据兼语前一动词的语义，常见的兼语句有以下几种：

表格 7兼语式类型表

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\TC4D5KD\~1NX\`(\[O\_LK2O6X1.png](media/image87.png){width="4.958333333333333in"
height="4.134027777777778in"}

我们用"N1+V1+N2+V2"来表示兼语句句式特征。对于兼语句的标注，主要有两个方面的特征一定要标注出来：

1.  **N2与V1和V2的语义关系**。兼语式的特征之一就是N2节点出现了多父亲节节点的现象。

2.  **V1和V2之间的语义关系。**这两个述谓概念也会构成一定的语义联系，需要标注出来。

前文在讲述心理活动动词是，对于爱恨事兼语的标注有了解释，由于"爱恨式"的N1有很强的主观施动性，所以我们把"N2+V2"结构视为V1的降级客事角色，而N1的语义角色也相对固定，细粒度标签为感事角色Aft，粗粒度标签为施事角色AGT，而其他待标成分之间的语义关系需要结合语境。具体例子可参照心理活动动词示例。标注范式为：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\53\@Z\$KE\_T\`2\_99PK8QA801H.png](media/image88.png){width="3.1979166666666665in"
height="0.7604166666666666in"}

图 84兼语式范式1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\59Y(IOGS)3(FX{0\[V}FEOTI.png](media/image89.png){width="3.4479166666666665in"
height="0.84375in"}

图 85兼语式范式2

对于使令式的兼语，一般来说，由于使令式的动词都具有主观施动性，所以N2是V1的受事角色PAT（细粒度标签也是受事角色），N2是V2的主体角色，而V2是V1的一种结果，所以我们标注为结果事件关系eEFFT，细粒度标签为eRes，其他待标成分之间的语义关系需要结合语境。标注范式为：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\{PVTUC8\]\_V\`3{22V(7K(S29.png](media/image90.png){width="3.375in"
height="0.78125in"}

图 86兼语式范式3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\3\`U(ZHW4DU%0GGZ%)8V\_A3R.png](media/image91.png){width="3.4583333333333335in"
height="0.7604166666666666in"}

图 87兼语式范式4

例如：微笑使你年轻。（root，使）

分析：微笑是使的当事角色，你是使的受事角色，同时也是年轻的当事角色。所以标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\433(XSQ6\~PEBB8{JE\${(\_9T.png](media/image92.png){width="3.0520833333333335in"
height="0.7027777777777777in"}

图 88兼语式示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\R3VKP\[@)\$(IYA@{G)E6%V\~U.png](media/image93.png){width="3.2916666666666665in"
height="0.6798611111111111in"}

图 89兼语式示例2

对于选定式和"有"字式的兼语，一般来说，由于这类兼语的前一动词多是对客观情况的描述、动作性不强，所以我们标注为后继事件关系eSUCC，细粒度标签标注为eSucc，其他待标成分需要结合具体语境，所以标注范式为：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\0{}XQHW)9J54ZP\[0ZH5{9U2.png](media/image94.png){width="3.53125in"
height="0.7486111111111111in"}

图 90兼语式范式5

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\7PA\`XI(YRSWL7Z{\_AE8P5D1.png](media/image95.png){width="3.625in"
height="0.7715277777777778in"}

图 91兼语式范式6

例如下面两个例句分别是选定式和"有"字式：

1\. 大家选他当班长。（root，选）

2\. 他有个妹妹很能干。（root，有）

分析：以句1为例，"大家"是"选"的施事角色，"他"是"当"的当事角色，"班长"是"当"的成事角色。所以，标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\11HOCO%\`F%\@KNJRNL%\_\_N%A.png](media/image96.png){width="3.8229166666666665in"
height="0.7527777777777778in"}

图 92兼语式示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\1UF0MKK\[SLB\~\_2U(NMA2\]Z3.png](media/image97.png){width="3.7291666666666665in"
height="0.7986111111111112in"}

图 93兼语式示例4

**综上，对于兼语式，根据V1和V2的关系，一共出现了三种标注情况：**

1.  爱恨式。依存弧由V1指向V2，是降级客事关系，粗粒度标签为dCONT，细粒度标签为dCont；

2.  使令式。依存弧由V1指向V2，是结果事件关系，粗粒度标签为eEFFT，细粒度标签为eRes；

3.  选定式和"有"字式。依存弧由V1指向V2，是后继事件辊系，粗粒度标签标注为eSUCC，细粒度标签标注为eSucc。

对比上述三种标注类型，我们发现，依存弧的指向是一致的，只是语义关系不同，这与V1表达的语义有很大的关系。除了上述四种基本的类型之外，还有一些其他类型的兼语句分类标准，但是上述三种标注方式基本能包含所有的兼语句类型，例如，"协助类、陪伴类"等的兼语可以按照第三种标注方式标注。所以，此处对于其他语义类型的兼语句式就不做细说。

### 3.5.5连谓式

连谓式是这样一种结构：由多项谓词性成分连用、谓词性成分之间没有语音停顿，也不用任何关联词语的短语叫做连谓短语，由连谓短语充当谓语或者独立成句的句子叫做连谓句。对于连谓句的语义依存图标注，必须要标注说明的是：

1.  主语与不同谓词之间的关系；

2.  不同谓词之间的关系。

连谓句可以表示多种语义关系，例如：

1.他低着头不动。------前一动作是后一动作的方式。

2.金山取了笔记本走了。------表示动作发生的先后顺序。

3.他看书看累了。------前后两个动作表示因果关系。

等等。

但是连谓式内部的几个谓词不管内部语义如何，排列顺序大部分都是按照时间先后。后一动作是前一动作的继续，粗粒度标签标注为后继事件关系eSUCC，细粒度标签标注为eSucc。如果将连谓式的结构表示为"N1+V1+V2"的话，同时我们要注意，一般情况下，这两个谓词都与主体角色N1有关，这两个词之间的语义依存关系也需要表示出来，而语义标签信息需要结合具体语境。所以标注范式如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\Z3FT4\_%\`2\$B)%\]%L\[\]XS\@9U.png](media/image98.png){width="2.4791666666666665in"
height="0.8020833333333334in"}

图 94连谓式范式1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\S20K3V\]Z(PKMC}3\_D}FFKCE.png](media/image99.png){width="2.4791666666666665in"
height="0.78125in"}

图 95连谓式范式2

> 例如：金山取了笔记本走了。（root，取）

分析：本句两个动作分别是"取"和"走"。"走"是"取"的后继事件关系，同时"取"和"走"的主体角色都是"金山"。所以标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\3FMJ%EPTCB)6W%N)(\`59OR7.png](media/image100.png){width="3.571527777777778in"
height="0.8090277777777778in"}

图 96连谓式示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\P)\`5U{RZL%KMXST\_)\_3\_(\_B.png](media/image101.png){width="3.6145833333333335in"
height="0.8236111111111111in"}

图 97连谓式示例2

注意，有时候，N1可能不是后一动作的发出者，而是后一动作造成结果的直接体验者。（详见3.5.6中补式）。

例如：他看书看累了。（root，看1）

分析：本句中有三个谓词性成分："看1"，"看2"以及"累"。其中"累"是"看2"的结果，"累"也是主体他的状态。所以，标注结果如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\{X253A7H4VJJ6FBD1N%8U)I.png](media/image102.png){width="3.6458333333333335in"
height="0.8194444444444444in"}

图 98连谓式示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\)KFVB\~4)\`6%\`2(CYYYX\`S\`N.png](media/image103.png){width="3.40625in"
height="0.78125in"}

图 99连谓式示例4

有一种复杂的情况，即兼语连谓兼用句。我们可以将兼语连谓句用"N1+V1+N2+V2"表示，由于兼语连谓句中的V1多是陪伴协助类的动作，所以将V1和V2的关系标注为后继事件关系eSUCC（细粒度标签为eSucc），其他词对之间的语义关系结合具体语境进行标注。所以标注范式为：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\X42YSKP04\_Y)WP\$UOQ\]P3\`N.png](media/image104.png){width="3.4895833333333335in"
height="0.8541666666666666in"}

图 100兼语连谓式范式1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\Z4OO\$}C9PR\[PI4B0)JH)\[6S.png](media/image105.png){width="3.375in"
height="0.8854166666666666in"}

图 101兼语连谓式范式4

例如：我陪他上楼。（root，陪）

分析：这个句子涵盖了三个语义事件，分别是："我上楼"，"他上楼"，"我陪他"，标注的时候要将这些情况标注出来。标注结果用依存图展示如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\`)H\`KC}Z08T\]\~}\$NL\~4}IOF.png](media/image106.png){width="3.0416666666666665in"
height="0.7486111111111111in"}

图 102兼语连谓式示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\]E\~6DE\[I\@LSBW\]DTTW6TBC6.png](media/image107.png){width="3.4166666666666665in"
height="0.7888888888888889in"}

图 103兼语连谓式示例2

其实通常来说，连谓式结构有语义上的轻重，很多连谓式是前轻后重型的，例如：坐车回家\|赶着做活，结构内部的语义重心在后面的"回家"和"做活"上；也有前重后轻型的，例如：买菜去\|说着玩儿，结构内部的语义重心在前面的动词"买"和"说"上；还有一部分连谓结构无法分出语义上的前后差别，例如：躺着不动\|喝酒喝醉了，这样的连谓式很难说清楚前后哪一个动词才是结构内部的重心。所以也是鉴于此，标注时默认的情况是将连谓结构的第一个动词作为结构中心。

### 3.5.6中补式

中补式是这样一种结构：由补充关系的两个成分组成，前面被补充的成分是中心语，由谓词充当，后头补充成分是补语，可以由谓词充当，例如"打\<伤\>"、"打\<死\>"；也可以由数量短语、介词短语充当，例如"踢了\<三下\>"、"学\<到天黑\>"；也可以由副词充当，例如"好\<极\>了"等，又叫动结式。对于中补式的标注，关键点在于补语跟句子中的哪一个待标成分具有语义上的关系。关键点在于补充成分是否跟主语或者宾语发生语义关系。

试比较以下例句：

1.  他打\<伤\>了导演。（root，打）

2.  他作业写得\<好\>极了。（root，写）

3.  他又踢了\<三次\>足球。（root，踢）

句1和句2的补语，从语义关系上讲，不仅与谓语中心有语义关系，而且与周边角色发生语义关系。句1"伤"的是"导演"，句2"好"的主体是"作业"而非"他"，但是句3中的补语是只与谓语中心语义关系。所以，以此为标准，可以将中补式的标注方式分成两种情况：

**1.补充成分与谓语中心和主客体角色发生语义关系。**

关于补充成分和谓语中心的关系，我们将依存弧由谓语中心指向补语，粗粒度标签标注为结果事件关系eEFFT，细粒度标签标注为eRes。同时这个补充成分作为一个新产生的动作结果，也是语义事件中某个参与者的某种状态，所以，它又依存于该参与者，与主客体角色发生语义关系。用"N1+V+VC+N2"组合来表示这种结构，VC表示补语，其中N2的位置不定，可以出现在中补结构之后，也可以由介词"把"引出，放在谓语中心之前，也可以是N2的一个附属成分。当参与者N2位置提前的时候，就会出现依存弧交叉的情况。要注意VC依附于哪一个成分上。所以标注范式如下图所示：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\FX58H\~C\@9TJ{NTFU3F5\~{MP.png](media/image108.png){width="2.7291666666666665in"
height="0.6770833333333334in"}

图 104中补式范式1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\\@ZQ27L1LJH\[)D84QNT1H4)A.png](media/image109.png){width="2.65625in"
height="0.6979166666666666in"}

图 105中补式范式2

例如：他把导演哭哭了。（root，哭1）

分析：本句中，第一个"哭"是谓语中心，"他"是这个"哭1"的施事角色；"哭2"是"哭1"的结果，同时"哭2"的动作发出这是"导演"。这个句子解构出来的两个语义事件是："他哭"和"导演哭"。所以，标注结果显示如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\XU}MW3G8\]TCN4IM3(2%G0KP.png](media/image110.png){width="4.145833333333333in"
height="0.9048611111111111in"}

图 106中补式示例1

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\Q\_KKJF01AQOTV3@\`4(6C4XP.png](media/image111.png){width="4.072916666666667in"
height="0.9451388888888889in"}

图 107中补式示例2

再例如：他作业写得好极了。（root，写）

分析：本句有两层中补式。第一层是"写"的结果补语\<好\>，第二层是"好"的程度补语\<极\>。该语义事件的中枢论元root是"写"，"写"的结果是"好"，"好"的程度是"极"，"他"是"写"的施事，"作业"是"好"的当事。也就是说，这个句子解构出来的两个语义事件是："他写作业"和"作业好极了"。标注结果用依存图显示如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\ZEVQ\$NQJT\[EEQAY1T3DP3GQ.png](media/image112.png){width="4.260416666666667in"
height="0.7680555555555556in"}

图 108中补式示例3

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\6K\$\$2IC}BL8\~\[XEEMK\@EJK7.png](media/image113.png){width="4.333333333333333in"
height="0.7458333333333333in"}

图 109中补式示例4

**2 补充成分只与谓语中心发生语义关系。**

当补语由数量短语或者介词短语充当的时候，补语成分往往充当某一种语义角色。例如"踢了＜两脚＞"、"走＜到天涯海角＞"、"学＜到深夜＞"，分别表示的是谓语中心的数量关系、位置关系、时间关系，所以我们将它们标注为度量，空间角色以及时间角色。依存弧由谓语中心指向补语成分。

对上述三个短语的标注示例分别如下：

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\%PX4R6\@6\[GZJ611Z%\`\](CAF.png](media/image114.png){width="1.9791666666666667in"
height="0.6597222222222222in"}

图 110中补式示例5

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\6NV01\@E\~\`43QO9O(DXK20GD.png](media/image115.png){width="2.0833333333333335in"
height="0.5833333333333334in"}

图 111中补式示例6

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\RFUV}TDFV\[\@5DI8HL5N51CK.png](media/image116.png){width="2.1145833333333335in"
height="0.6236111111111111in"}

图 112中补式示例7

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\))Z\@CV5TD)\]\$R0\`A{S\@8\`HX.png](media/image117.png){width="2.0416666666666665in"
height="0.5701388888888889in"}

图 113中补式示例8

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\THMY{S\$LZZ6L9(\~U2M\~0NTV.png](media/image118.png){width="1.90625in"
height="0.6284722222222222in"}

图 114中补式示例9

![C:\\Users\\cheng\\Documents\\Tencent
Files\\1501808365\\FileRecv\\MobileFile\\Image\\D43S6E\`OQ\$I3Z\~R17C9FC\@Y.png](media/image119.png){width="2.0520833333333335in"
height="0.6152777777777778in"}

图 115中补式示例10

在具体的语言环境中，也可能会出现其他的语义角色，这三种是比较常见的情况。总的来说，当补语中表达的是明确的数量、时间、空间等关系的时候，我们将它们标注为语义周边角色。

3.6小结
-------

综上就是关于中枢论元的标注细则。主要涉及到两个问题：

1.  如何确定某一语义事件中的中枢论元；

2.  如何处理中枢论元同其他述谓概念之间的关系。

对于第一个问题，我们要找到语义事件中最核心的述谓概念。

对于第二个问题，我们要对每一个述谓概念、每一种结构进行语义分析，然后再确定他们之间的语义关系。

中枢论元是一个语义事件的"纲"，找出它之后，我们就可以以此为切入点，开始对句子中其他成分进行标注了。
