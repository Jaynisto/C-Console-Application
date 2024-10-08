# C# Console Application In A Specified Folder.

## Overview

- My *TestProject App* is a simple C# console application that demonstrates basic features of the .NET platform.

- Make sure you have Visual Studio Code installed so that you can use it's integrated Terminal, and make sure you have .net Software Development Kit (SDK) installed on your machine.

## Steps

- On the Visual Studio Code *File* menu, select *Open Folder*.

- In the Open Folder Dialog make sure you open the one that has your project files.

- On the Visual Studio Code *Terminal* menu, select *New Terminal*.

- Notice the command prompt in the Terminal panel will display the folder's path for the current folder.

```bash
C:\Users\someuser\Desktop>
```

- At the Terminal command prompt, to create a new console application in a specified folder, enter the following command:

```bash
dotnet new console -o ./CsharpProjects/TestProject
```
- This .NET CLI command uses a .NET program template to create a new C# console application project in the specified folder location. The command creates the CsharpProjects and TestProject folders for you, and uses TestProject as the name of your .csproj file



# Update, build, and run your application

- In the Visual Studio Code EXPLORER view, right-click the *TestProject* folder, and then select Open in *integrated Terminal*.

- Verify that the command prompt in the Terminal panel displays the following folder path:

```bash
C:\Users\someuser\Desktop\CsharpProjects\TestProject>
```

- The first time you edit a .cs file, Visual Studio Code may prompt you to add the missing assets to build and debug your app. If you see the prompt, you can select Yes.

- For example you can write on your .cs file :

```bash
Console.WriteLine("Hello, C#!");
```

- On the *File* Manu, select *Save*.

- You always need to save your code changes to the file. Code changes that you've made in the Editor won't be recognized by the code compiler until the code is saved.

- To compile a build of your application, enter the following command at the Terminal command prompt:

```bash
dotnet build
```
- The dotnet build command builds the project and its dependencies into a set of binaries. The binaries include the project's code in Intermediate Language (IL) files with a .dll extension. Depending on the project type and settings, other files may also be included. If you're curious, you can find the TestProject.dll file in the EXPLORER panel at a folder location that's similar to the following path:

```bash
C:\Users\someuser\Desktop\CsharpProjects\TestProject\bin\Debug\net7.0\
```

- To run your application, enter the following command at the Terminal command prompt:

```bash
dotnet run
```

- The dotnet run command runs source code without any explicit compile or launch commands. The command depends on the dotnet build command to build the code.

- Your output will be :

```bash
Hello, C#!
```