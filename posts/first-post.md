---
title: "How Much Does One Character Weigh? Text Encoding and Homoglyph Attacks" 
tags: [UTF-8, bytes, character encoding, homoglyph attacks, ASCII]
---

# How Much Does One Character Weigh? Text Encoding and Homoglyph Attacks

## Introduction

When typing on a computer keyboard, it is natural to view letters, numbers, and emojis as light, abstract symbols on a display screen. However, every character stored on a device possesses a specific physical weight measured in digital storage, specifically bytes. Understanding how computers represent text and allocate memory for different characters is a foundational concept in computer science and digital systems. While simple English text requires minimal space, international characters, accent marks, and emojis require significantly more data. Beyond memory allocation, text encoding mechanics directly impact web security, creating vulnerabilities known as homoglyp attacks. Homoglyph Attacks occur when threat actor register domains, craft email addresses, or design phishing pages using characters from different alphabets or scripts that visually resemble legitimate ones. 

The core topic of this post is text character encoding, specifically focusing on how systems transitioned from early standard systems like ASCII to modern standards like the UTF-8 standard, memory allocation across different character sets, and how visually identical characters can be exploited to deceive users online. This topic matters because character encoding is the underlying framework for all digital communication, data storage, and web navigation. As the internet becomes increasingly global and multilingual, systems must handle diverse character sets without sacrificing efficiency or security.

This blog post will answer three main questions:
1. How does a computer convert human-readable text into binary bytes using encoding standards like ASCII and UTF-8?
2. Why do different characters consume different amounts of memory?
3. How do cybercriminals exploit look-alike characters (homoglyphs) to execute deceptive domain spoofing attacks, and how can these attacks be identified?

## References 
1. Dhingra, S. (2026, July 28). Same look, different code: The technical reality behind homoglyph attacks. Kratikal Blogs. https://kratikal.com/blog/same-look-different-code-homoglyph-attacks/
2. Khalil, M. (2025, November). What is a homoglyph attack? Unicode spoofing in 2026. DeepStrike. https://deepstrike.io/blog/what-is-a-homoglyph-attack
3. Invicti. (n.d.). HTTP spoofing (IDN homograph attacks). Invicti Learn. Retrieved November 8, 2026, from https://www.invicti.com/learn/mitm-https-spoofing-idn-homograph-attack
