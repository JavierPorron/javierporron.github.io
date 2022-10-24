---
layout: post
title:  Roadmap on Blockchain as a Computer Engineer - Chapter 1
author: Javier Porrón
date:   2022-10-24 00
image:  resiz.jpg
tags:   Blockchain Bitcoin Roadmap Computer Engineer Hash Consensus
---
Here we go, in this 'Chapter 1' we are going to talk about some basic concepts about what is Blockchain and how it works in general concepts. 
I think is not necessary to talk about what could be the benefecits of work as a Blockchain Engineer, Blockchain Developer... The most of you would arrived here because already know that, but, if you didn't I invite you just to take a look on the demand with the past of the years and the salaries. I think it would motivate you to continue with this course week a week.
So! let's start!
 
#### What is Blockchain?
Blockchain as its proper name indicates, it is a chain of blocks, where the blocks contains  data. This chain forms a distributed database or ledger shared among different nodes of a computer network.
This idea was originally propossed in 1991 by Stuart Haber and W. Scott Stornetta where they described something about a blockchain criptographycally secure for a timestamp system. This system couldnt be manipulated.So, in 1992 this scients with the help of Dave Bayer introduced [Merkle trees](https://en.wikipedia.org/wiki/Merkle_tree) to the concept, a kind of data structure where every node of a tree that are not a leaf are labeled by a Hash that comes from the concatenation of the labels of their child nodes. Finally, this technology started working on 'The New York Times' publishing week by week since 1995 hashes of certifieds documents , been 'The New York Times' the first 'Blockchain'.

To be right, the concept of 'Blockchain' as the way that we know was not introduced until 2008 where a person or a group of people with the name of Satoshi Nakamoto improving the design of the technology as we know now a days, calling it Bitcoin. The identity of Satsho Nakamoto is a mistery yet.

#### How it Works?
As we said in the last section, Blockchain is a distributed database that works with blocks where it stores de data. But, **where comes the term of 'chain'?** 

Every block is connected each other as a chain using a **Hash**.

A **Hash** is like a kind of fingerprint that identifies the previous block. This hash is calculated with a criptographic function (called hash), a mathematic algorithim that transform a set of data in to a string of characters with a fixed length, what ever were the length of the input data, the length always will be the same. This causes if the input data change, the result of the function will change as well.

Each block contains the hash of the previous one, forming a kind of chain.
The hash comes from the data stored in the block. When a block is filled completly, is calculated the hash from all the data of the block and this hash is added to the next block. In this way, if one of the previos blocks change, the hash change with it and the chain breaks.

Let's take a clouser look on this.

A block, it's composed mainly of 3 things:
* **The previous Hash:** Hash of the previos block. 
* **The data stored**
* **The Hash of the block:** using the hash function and using as well the data of this block as the input of the function, the fingerprint of the block is obtained.

This process creates the chain. 

<br>

**Blockchain technology is one of the most secure technologies in the world.** But to it incorporates some other mechanisms. 

Imagine the following scenario:
![](../img/Otros.png)
In this scenario, we have 3 blocks that compose a chain. The hash of the previous block is stored in the next block.

Now, imagine that one maliciuos attacker tries to modify the second block to his benefit. The hash of the second block would change and will not match with the hash stored in the next block, so the chain will breaks.

![](../img/Otros2.png)

This scenario, from part of the malicious attacker could be fixed recalculating all the following hashes of the blockchain, something relatively easy for today's computers. To avoid this, blockchain have **consensus mechanisms**, that makes harder to a malicious attacker recalculate all the following hashes on a blockchain. (We will talk deeply about this in the following posts)

Blockchain network its a P2P network, where all the nodes of the network has an exact replica of the database.
In this way, if someone modifies a block in the blockchain that he stores, the other networks will know that the blockchain has been violated and they will reject that block.


<small><a href="https://www.freepik.com/free-vector/server-room-artificial-intelligence-big-data-processing-online-banking-operations_3629652.htm#query=blockchain&position=37&from_view=author">Image by fullvector</a> on Freepik </small>


