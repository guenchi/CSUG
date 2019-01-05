# csug

Chez Scheme 用户手册 翻译

翻译活动经费由@guenchi出资赞助： 1000字/100元

源文档：https://cisco.github.io/ChezScheme/csug9.5/csug.html

# *Chez Scheme Version 9.5 User's Guide* 中文版

原文地址：http://cisco.github.io/ChezScheme/csug9.5

## 翻译任务清单

注：想认领章节翻译的同学可以到Issues中提一个任务领取的Issuse，提的时候最好能同时给一个预估的翻译截止时间。

| 章节                                          | 认领人 | 完成情况 | 开始时间 |
| --------------------------------------------- | ----- | ------ | ------- |
| Preface                                       ||||
| Chapter 1. Introduction                       | flowingfirefly | 完成 section1.1 之前的部分| 2019-01-04 |
| Chapter 2. Using Chez Scheme                  ||||
| Chapter 3. Debugging                          ||||
| Chapter 4. Foreign Interface                  ||||
| Chapter 5. Binding Forms                      ||||
| Chapter 6. Control Structures                 ||||
| Chapter 7. Operations on Objects              | xashes | Section 7.4 | Dec 31, 2018 |
| Chapter 8. Numeric Operations                 ||||
| Chapter 9. Input/Output Operations            ||||
| Chapter 10. Libraries and Top-level Programs  ||||
| Chapter 11. Syntactic Extension and Modules   ||||
| Chapter 12. System Operations                 ||||
| Chapter 13. Storage Management                ||||
| Chapter 14. Expression Editor                 ||||
| Chapter 15. Thread System                     ||||
| Chapter 16. Compatibility Features            ||||

<!--
## 目录

- Preface
- Chapter 1. Introduction
  - Section 1.1. Chez Scheme Syntax
  - Section 1.2. Notational Conventions
  - Section 1.3. Parameters
  - Section 1.4. More Information
- Chapter 2. Using Chez Scheme
  - Section 2.1. Interacting with Chez Scheme
  - Section 2.2. Expression Editor
  - Section 2.3. The Interaction Environment
  - Section 2.4. Using Libraries and Top-Level Programs
  - Section 2.5. Scheme Shell Scripts
  - Section 2.6. Optimization
  - Section 2.7. Customization
  - Section 2.8. Building and Distributing Applications
  - Section 2.9. Command-Line Options
- Chapter 3. Debugging
  - Section 3.1. Tracing
  - Section 3.2. The Interactive Debugger
  - Section 3.3. The Interactive Inspector
  - Section 3.4. The Object Inspector
  - Section 3.5. Locating objects
  - Section 3.6. Nested object size and composition
- Chapter 4. Foreign Interface
  - Section 4.1. Subprocess Communication
  - Section 4.2. Calling out of Scheme
  - Section 4.3. Calling into Scheme
  - Section 4.4. Continuations and Foreign Calls
  - Section 4.5. Foreign Data
  - Section 4.6. Providing Access to Foreign Procedures
  - Section 4.7. Using Other Foreign Languages
  - Section 4.8. C Library Routines
  - Section 4.9. Example: Socket Operations
- Chapter 5. Binding Forms
  - Section 5.1. Definitions
  - Section 5.2. Multiple-value Definitions
  - Section 5.3. Recursive Bindings
  - Section 5.4. Fluid Bindings
  - Section 5.5. Top-Level Bindings
- Chapter 6. Control Structures
  - Section 6.1. Conditionals
  - Section 6.2. Mapping and Folding
  - Section 6.3. Continuations
  - Section 6.4. Engines
- Chapter 7. Operations on Objects
  - Section 7.1. Missing R6RS Type Predicates
  - Section 7.2. Pairs and Lists
  - Section 7.3. Characters
  - Section 7.4. Strings
  - Section 7.5. Vectors
  - Section 7.6. Fixnum-Only Vectors
  - Section 7.7. Bytevectors
  - Section 7.8. Boxes
  - Section 7.9. Symbols
  - Section 7.10. Void
  - Section 7.11. Sorting
  - Section 7.12. Hashtables
  - Section 7.13. Record Types
  - Section 7.14. Record Equality and Hashing
  - Section 7.15. Legacy Record Types
  - Section 7.16. Procedures
- Chapter 8. Numeric Operations
  - Section 8.1. Numeric Type Predicates
  - Section 8.2. Fixnum Operations
  - Section 8.3. Flonum Operations
  - Section 8.4. Inexact Complex Operations
  - Section 8.5. Bitwise and Logical Operators
  - Section 8.6. Random Number Generation
  - Section 8.7. Miscellaneous Numeric Operations
- Chapter 9. Input/Output Operations
  - Section 9.1. Generic Ports
  - Section 9.2. File Options
  - Section 9.3. Transcoders
  - Section 9.4. Port Operations
  - Section 9.5. String Ports
  - Section 9.6. File Ports
  - Section 9.7. Custom Ports
  - Section 9.8. Input Operations
  - Section 9.9. Output Operations
  - Section 9.10. Input/Output Operations
  - Section 9.11. Non-Unicode Bytevector/String Conversions
  - Section 9.12. Pretty Printing
  - Section 9.13. Formatted Output
  - Section 9.14. Input/Output Control Operations
  - Section 9.15. Fasl Output
  - Section 9.16. File System Interface
  - Section 9.17. Generic Port Examples
- Chapter 10. Libraries and Top-level Programs
  - Section 10.1. Built-in Libraries
  - Section 10.2. Running Top-level Programs
  - Section 10.3. Library and Top-level Program Forms
  - Section 10.4. Standalone import and export forms
  - Section 10.5. Library Parameters
  - Section 10.6. Library Inspection
- Chapter 11. Syntactic Extension and Modules
  - Section 11.1. Fluid Keyword Bindings
  - Section 11.2. Syntax-Rules Transformers
  - Section 11.3. Syntax-Case Transformers
  - Section 11.4. Compile-time Values and Properties
  - Section 11.5. Modules
  - Section 11.6. Standalone import and export forms
  - Section 11.7. Built-in Modules
  - Section 11.8. Meta Definitions
  - Section 11.9. Conditional expansion
  - Section 11.10. Aliases
  - Section 11.11. Annotations
- Chapter 12. System Operations
  - Section 12.1. Exceptions
  - Section 12.2. Interrupts
  - Section 12.3. Environments
  - Section 12.4. Compilation, Evaluation, and Loading
  - Section 12.5. Source Directories and Files
  - Section 12.6. Compiler Controls
  - Section 12.7. Profiling
  - Section 12.8. Waiter Customization
  - Section 12.9. Transcript Files
  - Section 12.10. Times and Dates
  - Section 12.11. Timing and Statistics
  - Section 12.12. Cost Centers
  - Section 12.13. Parameters
  - Section 12.14. Virtual registers
  - Section 12.15. Environmental Queries and Settings
  - Section 12.16. Subset Modes
- Chapter 13. Storage Management
  - Section 13.1. Garbage Collection
  - Section 13.2. Weak Pairs, Ephemeron Pairs, and Guardians
  - Section 13.3. Locking Objects
- Chapter 14. Expression Editor
  - Section 14.1. Expression Editor Parameters
  - Section 14.2. Key Binding
  - Section 14.3. Editing Commands
  - Section 14.4. Creating New Editing Commands
- Chapter 15. Thread System
  - Section 15.1. Thread Creation
  - Section 15.2. Mutexes
  - Section 15.3. Conditions
  - Section 15.4. Locks
  - Section 15.5. Locked increment and decrement
  - Section 15.6. Thread Parameters
  - Section 15.7. Buffered I/O
  - Section 15.8. Example: Bounded Queues
- Chapter 16. Compatibility Features
  - Section 16.1. Hash Tables
  - Section 16.2. Extend-Syntax Macros
  - Section 16.3. Structures
  - Section 16.4. Compatibility File
- Bibliography
- Summary of Forms
- Index
-->
