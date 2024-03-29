---
title: 动词
---

动词的选用原则，请参见 [使用 STE 许可词汇]({% link _style-guide-en/word-choice/use-ste-words.md %}) 和 [选用专业术语](../word-choice/select-technical-terms.md)。

使用动词时，应注意以下几点：

1. toc
{: toc}

# 优先使用一般现在时

通常，一般现在时是最简单、最易于理解的时态。在技术写作中，优先使用一般现在时。不能使用一般现在时的情况下，可以使用一般过去时和未来时。

|  允许使用  |  禁止使用  |
|:---:|:---:|
|  一般现在时<br />一般过去时<br />未来时  |  现在完成时<br />过去完成时<br />现在进行时<br />过去进行时<br />其他复杂的时态  |

{% capture case-id -%}{% increment counter %}{%- endcapture %}

> 本例中，可以使用一般现在时，不需要使用未来时。

{%- capture original-{{ case-id }} -%}
When you open the latch, the panel **will slide** forward.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
When you open the latch, the panel **slides** forward.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

> 本例中，使用一般现在时会改变句子的含义。所以，必须使用未来时。

{%- capture original-{{ case-id }} -%}
Cancel a broker deployment only if you are sure that the broker **never responds to** the deployment request.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
Cancel a broker deployment only if you are sure that the broker **will never respond to** the deployment request.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

# 优先使用主动语态

语态分为两种：主动语态和被动语态。在主动语态中，句子的主语是动作的实施者。在被动语态中，句子的主语是动作的承受者。通常，主动语态比被动语态能够表达得更清晰、更简洁。

{%- capture example-{{ case-id }} -%}
主动语态：  
the manufacturer **supplies** the safety procedures.

被动语态：  
the safety procedures **are supplied** by the manufacturer.
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

**在操作步骤中，必须使用主动语态。在描述性内容中，尽可能使用主动语态。**

通常，大部分描述性内容都可以使用主动语态。但在有些情况下，必须使用被动语态才能表达得更好、更正确地。

可以使用被动语态的情况如下：

- 动作的实施者是系统。
- 你需要强调动作的承受者。
- 不想让用户感觉或错以为你在责备他，比如错误提示信息。
- 使用被动语态能让内容更清晰。
- 某些特定的信息类型，比如术语定义。

> 本例中是一个操作步骤，必须使用主动语态。

{%- capture original-{{ case-id }} -%}
The test can **be continued** by the operator.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
**Continue** the test.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

> 本例中的描述性句子，是可以用主动语态表达的，所以不能使用被动语态。

{%- capture original-{{ case-id }} -%}
These values **are used** by the computer **to calculate** the energy consumption.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
The computer **calculate** the energy consumption from these values.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

> 本例中，动作的实施者是系统，使用被动语态更合适。

{%- capture example-{{ case-id }} -%}
**The file is saved** when you press Enter.
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

> 本例中是一条错误提示信息，使用被动语态才不会让用户感觉你在责备他。

{%- capture example-{{ case-id }} -%}
`Error: An incorrect value was entered.`{: style="background: transparent;"}
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

# 使用合适的语气

根据信息类型选择合适的语气：

- 对于操作说明或要求（比如操作步骤），使用祈使语气。
- 对于说明性信息（比如概念讲解或功能说明），使用陈述语气。

在技术写作中，不要使用虚拟语气。

> 本例中是一个操作说明，应该使用祈使语气。

{%- capture original-{{ case-id }} -%}
The test can be continued.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
**Continue** the test.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

> 本例中是一个功能说明，应该使用陈述语气。

{%- capture example-{{ case-id }} -%}
The product provides a powerful way to store information.
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

> 本例中使用了虚拟语气，应该改为陈述语气或祈使语气。

{%- capture original-{{ case-id }} -%}
If you were to save the file ...
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
If you save the file ...
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

# 只能将过去分词用作形容词

动词的过去分词一般用在被动语态中，但技术写作中不提倡使用被动语态。尽管如此，过去分词仍然可以被用作形容词。

将过去分词用作形容词时，一般有两种形式：

- 放在名词的前面
- 放在 "to be" 或 "to become" 的后面

在这两种形式中，过去分词的作用是描述事物的状态，和被动语态无关。

只有 ASD-STE100 词汇表中的过去分词是可以使用的。有些动词虽然不是许可动词，但它们的过去分词是许可形容词，可以使用。比如 "specified"、"permitted" 和 "damaged"。

一些不规则动词的过去分词（比如 "be" 的过去分词 "been"）不可能成为形容词，所以它们没有包含在 ASD-STE100 词汇表中，不能使用。

> 本例中，"disconnected" 用在名词前面，是一个形容词。

{%- capture example-{{ case-id }} -%}
Connect the **disconnected** wires.
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

> 本例中，"disconnected" 用在 "to be" 的后面，表示接线的状态，是一个形容词。

{%- capture example-{{ case-id }} -%}
The wires **are disconnected**.
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

> 虽然 "damage" 不是许可动词，但 "damaged" 是许可形容词，可以使用。

{%- capture example-{{ case-id }} -%}
Make sure that the mating surfaces **are not damaged**.
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

# 不要将助动词或情态动词和过去分词一起使用

不要将助动词 "to have" 和过去分词一起使用。否则，它们很可能形成不正确的时态，比如现在完成时。

不要将助动词或情态动词和过去分词一起使用。否则，它们很可能变成被动语态或结构复杂的句子。

> 本例中，"to have" 和过去分词一起使用，形成了现在完成时，属于禁止使用的时态。范例中的句子改用了一般过去时，是允许使用的时态。

{%- capture original-{{ case-id }} -%}
The operator **has adjusted** the linkage.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
Tge operator **adjusted** the linkage.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

> 本例中，情态动词 "must" 和 过去分词 "adjusted" 一起使用，形成了被动语态。范例中的句子改用了主动语态。

{%- capture original-{{ case-id }} -%}
The temperature **must be adjusted**.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
**Adjust** the temperature.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

# 不要使用动词的 "-ing" 形式

动词的 "-ing" 形式（以 "-ing" 结尾的单词）不仅容易使句子结构变复杂，还容易产生歧义。所以一般情况下，不要使用动词的 "-ing" 形式。

但动词的 "-ing" 形式在以下两种情况下是可以使用的：

- 专业术语中含有以 "-ing" 结尾的单词
- 以 "-ing" 结尾的单词属于 ASD-STE100 词汇表中的许可词汇

> "Be" 和 "Doing" 一起使用，形成了现在进行时，属于禁止使用的时态。

{%- capture original-{{ case-id }} -%}
When you **are doing** this procedure, obey all the safety precautions.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
When you **do** this procedure, obey all the safety precautions.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}

> 本例中，以 "-ing" 结尾的单词属于专业术语，可以使用。

{%- capture example-{{ case-id }} -%}
Cleaning  
Packaging  
Shipping  
Troubleshooting
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

> 本例中，专业术语中包含以 "-ing" 结尾的单词，可以使用。

{%- capture example-{{ case-id }} -%}
Air-conditioning system  
degreasing agent  
polishing disc  
welding torch
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

> 本例中，以 "-ing" 结尾的单词属于 ASD-STE100 词汇表中的许可词汇，可以使用。

{%- capture example-{{ case-id }} -%}
lighting  
opening
missing  
remaining
{%- endcapture %}

{% include templateComponents/manualCase-single.html %}

# 使用动词描述动作

描述动作时，使用动词，不要使用名词。使用名词描述动作会使表达太含蓄，不如使用动词那样简单直白。

{%- capture original-{{ case-id }} -%}
The ohmmeter gives an **indication** of 450 ohms.
{%- endcapture -%}

{%- capture rewrited-{{ case-id }} -%}
The ohmmeter **shows** 450 ohms.
{%- endcapture -%}

{% include templateComponents/manualCase.html %}
