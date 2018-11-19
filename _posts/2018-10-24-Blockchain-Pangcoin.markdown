---
layout: post
title:  最小的区块链搭建
date:   2018-10-24
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: post13.jpg # Add image post (optional)
tags: [Blockchain]
author: 姜戈# Add name author (optional)
essays: true
---
区块链学习过程中，用Python3代码来做一个最小的区块链搭建。我称它为pangcoin。

跟比特币一样，先定义块，在区块链中，每个块都存储一个时间戳和一个索引。在pangcoin中，需要把两者都存储起来。为了确保整个区块链的完整性，每个块都有一个自动识别散列，每个块的散列将是块索引、时间戳、数据和前块哈希的加密哈希。
```python
#!/usr/bin/env python

# -*- coding: utf-8 -*-

import hashlibas hasher

import datetimeas date

class Block:

    def __init__(self, index, timestamp, data, previous_hash):

        self.index = index#索引

        self.timestamp = timestamp#时间戳

        self.data = data#数据

        self.previous_hash = previous_hash#前块哈希的加密哈希

        self.hash =self.hash_block()#当前块的哈希

    def hash_block(self):

        sha = hasher.sha256()

        sha.update(

        bytes(

                str(self.index) +str(self.timestamp) +str(self.data) +str(

                self.previous_hash),'utf-8'))

    return sha.hexdigest()
```
现在有了块结构，还没有形成区块链，所以需要向实际的链中添加块。如前所述，每个块都需要上一个块的信息。但是按照这个说法就有一个问题，区块链的第一个区块是如何到达那里的呢？不得不说，第一个块，或者说是起源块，它是一个特殊的块，需要手动添加起源块。
```python
def create_genesis_block():

# 起源块

    return Block(0, date.datetime.now(),"Genesis Block","0")
```
定义下一块：
```python
def next_block(last_block):

this_index = last_block.index +1

    this_timestamp = date.datetime.now()

this_data ="Hey! I'm block " +str(this_index)

this_hash = last_block.hash

return Block(this_index, this_timestamp, this_data, this_hash)
```
创建区块链，因为是最小的，pangcoin的数量定义为10个及说明：
```python
def main():

#  添加区块链和起源块

    blockchain = [create_genesis_block()]

previous_block = blockchain[0]

#  起源块后可添加的块数值

    num_of_blocks_to_add =10

    for iin range(0, num_of_blocks_to_add):

block_to_add = next_block(previous_block)

blockchain.append(block_to_add)

previous_block = block_to_add

#  展示说明

        print("Block #{} has been added to the"

              "blockchain!".format(block_to_add.index))

print("Hash: {}\n".format(block_to_add.hash))

if __name__ =="__main__":

main()
```
区块链测试OK

Block #1 has been added to theblockchain!

Hash: ed5c5144149ec443dc9d8717d340ede40043c5fa7c5355d027ac9e7ead069826

Block #2 has been added to theblockchain!

Hash: 4fd0dfba18789234b1c0e187e56ea72bb52562befd2ee85acc02971ed6a99474

Block #3 has been added to theblockchain!

Hash: 7163a83945e2b8b5f6666da51912edc4aa85bbf748f7de76fb892cc6cd4cf6ca

Block #4 has been added to theblockchain!

Hash: 75bc961fa0e2613c5196d9cbe7904f5e705678cdd70f97c02d401b16c27711dd

Block #5 has been added to theblockchain!

Hash: 75d9790faf0d0561853f6617b3716522387f6ffcfc45ed94c917d1a7e5bcaa19

Block #6 has been added to theblockchain!

Hash: 74a3cca336bf483648fd3e64597d18c57614a5f27146cddd91482461db212753

Block #7 has been added to theblockchain!

Hash: 4975bbbca58b8a5bf06209a670b1d61180ffb6a2e2ab5cceec3c0fdd5efe7222

Block #8 has been added to theblockchain!

Hash: 9253440eeae7ddb5803e35b91702cfc72d22107fe82b64842c54a5d6df2c9c19

Block #9 has been added to theblockchain!

Hash: 9d476babbd74cc1622c220045e98c3c0922075e8f77919a70fc1722e86cb70ef

Block #10 has been added to theblockchain!

Hash: 1040825c3715c48a0c650a68d6189d5ab11db3f02b4edae4a19e8dcad8547868

Process finished with exit code 0
