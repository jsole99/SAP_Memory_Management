# SAP Memory Management
SAP Learning material to understand Memory Management

# AUTHOR: Jeffery Sole
# Date: 05/12/23
# Description: Kochasoft Memory Types & Memory Management Learning Package

# Table of Contents
[Introduction to Memory Management](#Introduction)

# Introduction

SAP Memory Management has several types of memory which can be allocated differently. This allocation is determined by the systems OS type, work process type, as well as the systems configuration.

As memory is one of the main contributors to SAP system issues, it is important to understand each type of memory area, how they are used, and what can go wrong internally if not monitored carefully. We will break down each memory area and how they can be used to SAP's advantage.

These are the following memory areas SAP has:

| Memory Type | Physical Assignment | Lifetime | Address Stability  | User-Specific |
|---|---|---|---|---|
| SAP Shared Memory (SHM) | All work processes | ABAP Instance | No | No |
| Extended Segments Memory (ES) | All work processes | ABAP Transactions | Yes | - |
| Extended Memory (EM) | All work processes | ABAP Transactions | Yes | Yes |
| Global Extended Memory (EG) | All work processes | ABAP instance | Yes | No |
| PRIV Memory (HEAP) | Process-specific | ABAP transactions | Yes | Yes |
| PROC Memory | Process-specific | ABAP instance | Yes | No |