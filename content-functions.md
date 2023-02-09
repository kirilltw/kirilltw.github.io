---
layout: default
title: Content Functions
permalink: /content-functions/
---

[Homepage](./index.md) > {{ page.title }}

# Content Functions

> Originally written and published on 23 July 2021<br>
> This is an adaptation of the article at <https://documentation.divio.com/introduction/> with added clarifications to better contextualize the material.

A lot of people try to create good documentation. Many of them fail. Usually, it is not because they do not try hard enough, but because they are not doing it the right way. This system is a way to make your documentation better by doing it the right way. **The right way is the easier way** - easier to write, and easier to maintain.

The "secret" path to better documentation is structuring the content around the four different *content functions*:

* **Tutorials**
* **How-to guides**
* **Technical reference**
* **Explanation**

Hardware and software documentation is dependent on all four content functions and should be structured around them. At the same time, these content functions should be kept **separate and distinct from each other**.

To draw an analogy from our everyday life, let's imagine you want to cook something. You go to the kitchen and then find out:

* **Bad scenario**: Your cook book, pans and plates, ingredients, dish washing liquid are placed in the same container or bucket just because it is the stuff for cooking and eating. To start cooking, you need to sort out all these things and eventually find that your cook book has vinegar spills, some of your ingredients went bad, etc.
* **Good scenario**: Your cook book is on a bookshelf, pans and plates are in the kitchen cabinets, ingredients are stored in proper places, etc. You effortlessly find everything you need at known places in good condition and start cooking.

Table *Content Functions*

| | Tutorials | How-to guides | Reference | Explanation |
| --- | --- | --- | --- | --- |
| Reader's goal | Learn by doing | Complete a specific task | Look up info / data | Study theory |
| Content's goal | Allow a newcomer to get started | Show how to solve a specific problem | Describe the machinery | Provide background knowledge |
| Mode of writing | Lesson | Procedure, series of steps | Dry description | Discursive explanation |
| Usual formatting | Numbered list | Numbered list | Table, bulleted / numbered list | Text and illustrations |
| HW doc analogy | ? | Programming procedure | Register / Process Description | Peripheral Overview |
| HW doc example (TRM) | ? | In a TRM, see Sections *Programming Procedure* | In a TRM, see Sections *Registers* | In a TRM, see Sections *Introduction*
| SW doc analogy | Getting started guide | SW installation / configuration procedure | API reference, SW process | Introduction to an API reference |
| SW doc example (ESP-IDF) | [ESP-IDF Getting Started](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html) | [Install pre-commit Hook for ESP-IDF Project](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/contribute/install-pre-commit-hook.html) | [API reference](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/storage/nvs_flash.html#api-reference) for *Non-volatile storage library*, [Flash Encryption Process](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/security/flash-encryption.html#flash-encryption-process) for *Flash Encryption* | [Introduction](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/storage/nvs_flash.html#non-volatile-storage-library) for *Non-volatile storage library* |

Sometimes, a document fulfills only **one content function**. It is more characteristic to online writing with its multitude of interlinked pages. A famous advocate of this approach is Mark Baker with his [Every Page is Page One](https://everypageispageone.com/the-book/) approach.

However, more often a single document **combines different content functions**. For example, it is pretty often that Espressif's documentation combines:

* **Explanation** and **reference**
  TRM: Section *Functional Description*
* **Explanation** and **how-to guides**
  TRM: Section *Programming Procedure*
* **Explanation**, **how-to guides**, and **reference**
  ESP-IDF: [*I2C Driver*](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/peripherals/i2c.html)

From the perspective of a writer, **each content function requires a distinct mode of writing** (see the table above). Resiprocally, the **readers pursue different goals** while reading these four kinds of content.

![Overview of Content Functions](https://documentation.divio.com/_images/overview.png "Overview of Content Functions")

This division makes it obvious to both author and reader what content, and what kind of content, goes where. It tells the author **how to write**, and **what to write**, and **where to write** it. It allows the author to arrange the information quickly and efficiently in a way that makes sense, because **each of these kinds of content has only one job**.

With regards to arranging the information, there is another content function of **orientation**. It includes:

1. Inter-document navigation, such as a pathfinder topic.
   As an example, see [I am new to Sphinx!](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/contribute/documenting-code.html#ok-but-i-am-new-to-sphinx)
2.  Intra-document navigation, such as introduction to a document or a jump list
As an example, see [Installation Step by Step](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html#installation-step-by-step)

In fact, it’s extremely hard to maintain good documentation that does not implicitly or explicitly recognize the quadrants of this scheme. The demands of each kind are different from those of the others, so any attempt at documentation that fails to maintain this structure suffers, as it’s pulled in different directions at once.

Once you understand the structure, it becomes a very useful tool for analyzing existing documentation, and understanding what needs to be done to improve it.

For more information on the content functions, see the original articles

* [documentation.divio.com > Tutorials](https://documentation.divio.com/tutorials/#)
* [documentation.divio.com > How-to guides](https://documentation.divio.com/how-to-guides/)
* [documentation.divio.com > Reference guides](https://documentation.divio.com/reference/)
* [documentation.divio.com > Explanation](https://documentation.divio.com/explanation/)
