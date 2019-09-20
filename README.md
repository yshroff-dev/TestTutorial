### @activities 1

### @explicitHints 1

## Introduction

### Introduction step @unplugged

![Lesson 2](/static/china-tutorials/agentdig.gif)

# Welcome to Moon Base OMG2 OMG2 OMG2

**Unit 3. Lesson 2** - Mineral Samples!

## Activity 1 

### Step 1

**Activity 1 - Agent Dig 1**: Select the OMG OMG ``||user:on chat command||`` block and rename it to **dig1**.

#### ~ tutorialhint 

```blocks
user.onChat("dig1", function () {
	
})
```

### Step 2

Program your Agent to destroy **1** block **down** and move **1** block **down** by using an ``||agent:agent destroy down||`` and ``||agent:agent move down||``. 

#### ~ tutorialhint 

```blocks
user.onChat("dig1", function () {
    agent.destroy(SixDirection.Down)
    agent.move(SixDirection.Down, 1)
})
```

Hint: Make sure you select **down** from the drop-down menu. 

### Step 3

Make sure that your Agent repeats this action **10** times. Use a ``||loops:repeat||`` block.

#### ~ tutorialhint 

```blocks
user.onChat("dig1", function () {
    for (let i = 0; i < 10; i++) {
        agent.destroy(SixDirection.Down)
        agent.move(SixDirection.Down, 1)
    }
})
```

### Step 4

Add more commands inside your ``||user:on chat command||`` block to program your Agent to **collect all the items** with the help of ``||agent:agent collect all||`` block. After that, program your Agent to return to the surface. Use ``||agent:agent move||`` **up** by **10** blocks. 

#### ~ tutorialhint 

```blocks
user.onChat("dig1", function () {
    for (let i = 0; i < 10; i++) {
        agent.destroy(SixDirection.Down)
        agent.move(SixDirection.Down, 1)
    }
    agent.collectAll()
    agent.move(SixDirection.Up, 10)
})
```
Hint: Make sure the ``||agent:agent collect all||``and ``||agent:agent move up||`` blocks are **not** inside the a ``||loops:repeat||`` block. The Agent needs to move 10 blocks up to return to the surface. 

### Step 5

Go to the Minecraft world and type your command. Once completed, right-click on your Agent to see the inventory. Remove **Moon rocks** and keep only **rare minerals**. Place rare minerals in the yellow minerals box. You will be teleported to the next Activity. 

#### ~ tutorialhint 

Hint: You can always reset the Activity by clicking a reset button inside the NPC Guide. You can open the box by right-clicking on it. Once you are done, you will be teleported to the next Activity. 

## Activity 2

### Step 1

**Activity 2 - Agent Dig 2**: Select a new ``||user:on chat command||`` block and rename it to **dig2**. 

#### ~ tutorialhint 

```blocks
user.onChat("dig2", function () {
	
})
```

### Step 2

Program your Agent to dig a **2** block wide hole. Get your Agent to destroy **1** block **down**, move **1** block **down** and destroy **1** block **forward** from the same location. Use ``||agent:agent destroy down||``, ``||agent:agent move down||`` and ``||agent:agent destroy forward||`` blocks.

#### ~ tutorialhint 

```blocks
user.onChat("dig2", function () {
    agent.destroy(SixDirection.Down)
    agent.move(SixDirection.Down, 1)
    agent.destroy(SixDirection.Forward)
})
```

### Step 3

Now program your Agent to dig this hole **20** blocks **deep**. Program your Agent to repeat the actions **20** times. 

#### ~ tutorialhint 

```blocks
user.onChat("dig2", function () {
    for (let i = 0; i < 20; i++) {
        agent.destroy(SixDirection.Down)
        agent.move(SixDirection.Down, 1)
        agent.destroy(SixDirection.Forward)
    }
})
```

### Step 4

Program your Agent to collect only **diamonds** with the help of ``||agent:agent collect item||`` block and return to the surface with the help of ``||agent:agent move up||`` block.

#### ~ tutorialhint 

```blocks
user.onChat("dig2", function () {
    for (let i = 0; i < 20; i++) {
        agent.destroy(SixDirection.Down)
        agent.move(SixDirection.Down, 1)
        agent.destroy(SixDirection.Forward)
    }
    agent.collect(blocks.item(Item.Diamond))
    agent.move(SixDirection.Up, 20)
})
```
Hint: Don't forget to select a **diamond** egg from the drop-down menu. The Agent needs to move 20 blocks up to return to the surface. 

### Step 5

Go to the Minecraft world and type your command. Check your Agent's inventory and place **diamonds** to the yellow Moon minerals box. You will be teleported to the next Activity. 

#### ~ tutorialhint 

```blocks
user.onChat("dig2", function () {
    for (let i = 0; i < 20; i++) {
        agent.destroy(SixDirection.Down)
        agent.move(SixDirection.Down, 1)
        agent.destroy(SixDirection.Forward)
    }
    agent.collect(Item.Diamond)
    agent.move(SixDirection.Up, 20)
})
```

Hint: You can always reset the Activity by clicking a reset button inside the NPC Guide. 

## Activity 3 

### Step 1

**Activity 3 - Agent Dig 3**: Select a new ``||user:on chat command||`` block and rename it to **dig3**.

#### ~ tutorialhint 

```blocks
user.onChat("dig3", function () {
	
})
```

### Step 2

Program your Agent to dig a **4** block **wide** hole. Make the Agent repeat a pattern of breaking and then moving down a layer. 

#### ~ tutorialhint 

```blocks
user.onChat("dig3", function () {
    agent.destroy(SixDirection.Down)
    agent.move(SixDirection.Down, 1)
    agent.destroy(SixDirection.Forward)
    agent.move(SixDirection.Forward, 1)
    agent.destroy(SixDirection.Right)
    agent.move(SixDirection.Right, 1)
    agent.destroy(SixDirection.Back)
    agent.move(SixDirection.Back, 1)
    agent.move(SixDirection.Left, 1)
})
```
Hint: The pattern is ``||agent:agent destroy down||``, ``||agent:agent move down||``, ``||agent:agent destroy forward||``, ``||agent:agent move forward||``, ``||agent:agent destroy right||``, ``||agent:agent move right||``, ``||agent:agent destroy back||``, ``||agent:agent move back||`` and ``||agent:agent move left||`` blocks. 

### Step 3

Now program your Agent to dig the hole **10** block **deep** hole. You can do it using ``||loops:repeat||`` block. 

#### ~ tutorialhint 

```blocks
user.onChat("dig3", function () {
    for (let i = 0; i < 10; i++) {
        agent.destroy(SixDirection.Down)
        agent.move(SixDirection.Down, 1)
        agent.destroy(SixDirection.Forward)
        agent.move(SixDirection.Forward, 1)
        agent.destroy(SixDirection.Right)
        agent.move(SixDirection.Right, 1)
        agent.destroy(SixDirection.Back)
        agent.move(SixDirection.Back, 1)
        agent.move(SixDirection.Left, 1)
    }
})
```

### Step 4

Program your Agent to collect only **diamonds** and **emeralds** from digging, using 2 ``||agent:agent collect item||`` blocks. 

#### ~ tutorialhint 

```blocks
user.onChat("dig3", function () {
    for (let i = 0; i < 10; i++) {
        agent.destroy(SixDirection.Down)
        agent.move(SixDirection.Down, 1)
        agent.destroy(SixDirection.Forward)
        agent.move(SixDirection.Forward, 1)
        agent.destroy(SixDirection.Right)
        agent.move(SixDirection.Right, 1)
        agent.destroy(SixDirection.Back)
        agent.move(SixDirection.Back, 1)
        agent.move(SixDirection.Left, 1)
    }
    agent.collect(Item.Diamond)
    agent.collect(Item.Emerald)
    })
```

Hint: Don't forget to select diamond and emerald eggs from the drop-down menu. 

### Step 5

Program your Agent to return to the surface. Use ``||agent:agent move||`` **up** block. Your Agent needs to move **10** blocks **up**. Once you are done with coding, go to the Minecraft world and type your command to see your Agent dig. 

#### ~ tutorialhint 

```blocks
user.onChat("dig3", function () {
    for (let i = 0; i < 10; i++) {
        agent.destroy(SixDirection.Down)
        agent.move(SixDirection.Down, 1)
        agent.destroy(SixDirection.Forward)
        agent.move(SixDirection.Forward, 1)
        agent.destroy(SixDirection.Right)
        agent.move(SixDirection.Right, 1)
        agent.destroy(SixDirection.Back)
        agent.move(SixDirection.Back, 1)
        agent.move(SixDirection.Left, 1)
    }
    agent.collect(Item.Diamond)
    agent.collect(Item.Emerald)
    agent.move(SixDirection.Up, 10)
})
```

### Step 6 @tutorialCompleted

In the Minecraft world, remove the **minerals** from the Agent's inventory and place them in the yellow Moon minerals box to power up the last transmitter and complete the lesson.  

## Activity 4 

### Step 1

**Activity 4 - Your Activity!**: Program your Agent to dig or collect items for you! Use ``||agent:agent destroy forward||``, ``||agent:agent collect item||`` blocks.

### Finish

**Well done! You have completed the lesson.**


```package
nether
```