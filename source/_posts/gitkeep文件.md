---
title: .gitkeep 文件
---
 
# 简介

本文主要介绍在**git**中, `.gitkeep`的作用。

## 作用

**git**无法追踪一个**空的文件夹**，当用户需要**追踪(track)**一个空的文件夹的时候，按照惯例，大家会把一个称为`.gitkeep`的文件放在这些文件夹里。

## 例程

就个人而言，一般需要`.gitkeep`地方，是希望完成以下功能:

- 使git忽略一个文件夹下的所有文件，并保留该文件夹

```
# .gitignore

# ignore all files in lib/
lib/*
# except for .gitkeep
!.gitkeep
# ignore TODO file in root directory,not subdir/TODO
/TODO

```

当`.gitignore`采用上面的写法时，git会忽略`lib`文件夹下除了`.gitkeep`外的所有文件。