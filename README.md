# TableLayoutPanel with highlighted header

This is WinForms highlighted header control based on TableLayoutPanel

![Demonstrative image](img_01.png "Demonstrative image")


## Problem

There are a lot of panels for grouping the controls in WinForms. The best one of them is _TableLayoutPanel_. Unfortunately, this panel does not show the header.

## Solution

It can be solved by _GroupBox_ and _TableLayoutPanel_. This solution is easy, but I prefer to make inherited panel from _TableLayoutPanel_.

## How It Works

The _HeaderTableLayoutPanel_ implements the _IsHighlightText_ property and overrides the few properties like _Text_, _DisplayRectangle_ and _SizeFromClientSize_. Also, the _HeaderTableLayoutPanel_ overrides the _OnPaint_ and _OnFontChanged_ methods.



