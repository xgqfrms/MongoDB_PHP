#MongoDB and PHP(中文翻译) xgqfms 2015-02-01
## Chapter 1     Why MongoDB?
导致第一次dot-com(网络公司)崩溃的问题之一就是这巨大的开发费用,尤其是服务软件.一组新的并且切实可行的开源工具从第一次dot-com的灰烬中出现,并且变成下一代Internet的基础.在2001年的夏天,一种新的首字母缩略词出现了;LAMP-Linux,Apache,MySQL和PHP-变成一代开发者全体选择的平台.正是那样,PHP和MySQL联姻了(毕竟，它们彼此依靠).它们似乎是被设计的彼此永远在一起．

The Problem of Objects and Relational Data Structures
  这里只有一个问题.PHP一开始是作为一种模板语言-自然地,渐渐地接受对象. PHP 过去用于复杂的应用程序并且php一贯的改进为了满足这些不断增长的需求.实际上在模板文件中写原始的SQL查询语句的操作很快,因为不能接受的(有人说这从来不接受).随着这个问题越来越复杂,为了解决PHP使用对象(或数组)和MySQL(和其他关系型数据库)使用表,行,列 带来的不断地增长的问题,工具被写了出来.
 这不是一个针对PHP的问题.几十年来,人们已经建造了工具和库文件,为了自动化翻译对象到关系数据结构的处理过程.最流行的集合是名叫ORMs(对象关系制图人).ORMs被建造是为了解决SQL的问题.它们的销售定位于: 使用ORM,因为它屏蔽所有数据存储肮脏的细节.,因此所有你以前需要触摸的现在是你的友好地PHP对象.虽然工具出现做了一个合理的工作在保证更好实现上,它们从来没有真正的完美的工作.首先,你总是需要去记忆在这些对象后面的一个关系数据库,就表格,行和列而言.其次,这些ORMs 伴随着高昂的代价.它们增加了很多复杂性和应用程序的开销且仅保留了SQLs特征的子集.随着它们的发展,它很快变成了这样的一个事实,学习ORM是一件比首先学习SQL更加耗费时间的事.
有充足的理由这样说,虽然ORMs 在很大的程度上解决了SQL的问题,它却伴随着ORMs自身的问题.
The Problem with ORMs
The objective of an ORM may be simple, but the solution never is.
一个ORM的目标也许是简单的,但是在这个解决方案从来不会.
ORMs Are Hairy and Complex(既危险有复杂)
Propel 和 Doctrine 是PHP上两个最流行的ORMs. Propel 遵从一个活跃的记录模型.Doctrine遵从hibernate.这两个项目都相当大,有上万行代码构成.Doctrine 也提供自己的类似SQL的查询语言,叫做DQL,所以为了使用Doctrine你需要同时知道SQL和DQL. 

ORMs Aren’t Performant(???)
ORMs 的核心目标是方便开发人员.一个ORM的核心目标是给与开发者方便,当他们创建
把数据库的表,行和列翻译成你的语言对象.

ORMs Neutered SQL

CRUD(创建,查询,更新,删除)
Complicated Architecture


PHP Is Mostly CRUD



MongoDB, Optimized for Operation


MongoDB Is a Document Database


Document == Array


MongoDB Is Optimized for CRUD Operations

Optimal Interface for Developers

Optimal Performance

Optimal Simplicity

The Value of Consistency

CHAPTER 2 
PHP, MongoDB, and You
 
Installing the Driver on Linux or MacOS X

Checking for the Driver
Installing the Driver

Upgrading the Driver

Installing the Driver on Windows

Connecting to a Database

Connecting to a MongoDB Database Server

Selecting a Database

The Basics (CRUD Operations)

Creating/Selecting a Collection

Creating a Document

Primary Keys and ObjectIds

Reading a Document

Updating a Document

Saving a Document

Deleting a Document

The MongoDB Shell

mongo

Using the Shell



Administrative Commands

Working with Sets

Querying Sets

Finding (Querying) Data in MongoDB

Pagination with the Cursor

Ranges

Working with Arrays

Conditionals

Working with Multiple Documents

Working with Indexes

Setting Indexes

Index Order

About Indexes

Compound Indexes

Indexing Arrays

Indexes and Memory

Database References

References Are Not Foreign Keys

When to Use References or Reference versus Embed

How to Create References

How to Access DBRefs


Dates and Times


                                                                   CHAPTER 3
Advanced MongoDB

Regular Expressions

Aggregation Commands

findAndModify

GridFS

Replication

Sharding

Gotchas

                                                                  CHAPTER 4
PHP Libraries and Tools

Object Document Mappers (ODM)

Tools


Frameworks



                                                                   CHAPTER 5
Conclusion


About the Author







