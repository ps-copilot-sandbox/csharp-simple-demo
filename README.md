# Simple Copilot demo for C# and .NET through Visual Studio IDE

![Cover image](./images/csharp-cover.jpg)

This contains a simple demo for Copilot for **C#** and **.NET** through **Visual Studio IDE.** This is going to be useful for customers who are interested in using Copilot for C# and .NET and want to use Copilot to generate code through Visual Studio IDE.

Note that Copilot extension for Visual Studio IDE is **only available for Windows**. If you are using Mac, you can use Copilot through VS Code.

## 🎯 Goal

Welcome to GitHub Copilot! In this example, we'll show you how to use Copilot to write a simple .NET application.

## ✍️ Programming Languages

- C#

## 💻 IDE

- [Visual Studio IDE](https://visualstudio.microsoft.com/downloads/) for Windows

## 🗒️ Guide

This guide will walk you through the steps to get started with Copilot in Visual Studio IDE.

### Prerequisites

Make sure that you meet the following requirements.

- [Visual Studio IDE](https://visualstudio.microsoft.com/downloads/) for Windows
- [Copilot Extension for Visual Studio IDE](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot). 

[See this documentation on how to install Copilot extension for Visual Studio IDE](../CopilotExtensionVS)

### Step 1: Launch Visual Studio IDE

Make sure that you followed all prerequisites and installed Visual Studio IDE and Copilot extension for Visual Studio IDE.

Search for **Visual Studio** after clicking Windows button.

![Search Visual Studio IDE](./Demos/images/0_SearchVS.jpg)

Then, your Visual Studio IDE will be launching.

![Launch Visual Studio IDE](./Demos/images/1_VSLaunching.jpg)

### Step 2: Create a new project

Once Visual Studio IDE is launched, you will see the following screen. Although you can use an existig project, let's try to create a new project by selecting **Create a new project**.

![Create a new project](./Demos/images/2_CreateProject.jpg)

Then, you will see different options. Select **Console App (.NET Framework)** and click **Next**.

![Select Console App (.NET Framework)](./Demos/images/3_ConsoleApp.jpg)

Then, you will see the following screen. Enter **HelloCopilot** as the project name and click **Create**.

![Enter project name](./Demos/images/4_ProjectName.jpg)

You will see a progress bar while Visual Studio IDE is creating a new project.

![Creating a new project](./Demos/images/5_CreateProject.jpg)

### Step 3: Check Copilot is enabled

Let's make sure that Copilot is enabled. On bottom, you should see **Auth Status: OK** under **Output** window. Make sure to select **GitHub Copilot** from the dropdown.

![Check Copilot is enabled](./Demos/images/6_VSCodeStatus.jpg)

And you should also see a Copilot icon above the **Output** window.

![Copilot icon](./Demos/images/7_CopilotLogo.jpg)

### Step 4: Write a simple code

Let's start writing some simple code first. Inside your **Main** method, create a following comment after `//`

```csharp
// Print out Hello, Copilot 3,000 time with incrementing index
```

![Write a simple code](./Demos/images/8_FirstCode.jpg)

As soon as you enter next line, you should see that Copilot is suggesting you to write a code. 

![Copilot suggestion](./Demos/images/9_CopilotSuggestion.jpg)

Select the first suggestion by hitting **Tab** button.

![Select Copilot suggestion](./Demos/images/10_Complete.jpg)

By the way, since this is a Console App, it will be a good idea to add the following line at the end of your **Main** method.

```csharp
Console.ReadLine();
```

This can helps to keep the console window open after the program is finished.

![Add Console.ReadLine()](./Demos/images/11_AddReadline.jpg)

Your file should look like this.

![Final code](./Demos/images/12_Readline.jpg)

That is it for writing a very simple code using Copilot. We can run this code by clicking **Start** button on top, but let's actually write a function.

### Step 5: Write a function

We will add a function above the **Main** method. Let's add a following comment as a block comment.

```csharp
/*
 * Function to sum all the numbers in a list of integers
 */
```

![Write a function](./Demos/images/13_AddFunction.jpg)

Again, when you enter, it should show you a suggestion. Yours might look different frome mine, though.

![Function suggestion](./Demos/images/14_FunctionSuggestion.jpg)

Hit **Tab** button to select the first suggestion. Your code might look like this.

![Function code](./Demos/images/15_CompleteCode.jpg)

Let's proceed to add codes to run that within main function. In the Main method, start clicking anywhere and click **Enter** button to see suggestions made by Copilot.

![Main method](./Demos/images/16_CreateList.jpg)

You can keep hit **Enter** and **Tab** buttons to take suggestions, but make sure that you can stop once you are happy with the result or fix if needed.

![Print](./Demos/images/17_Print.jpg)

### Step 6: Run the code

Now, let's run the code. Click **Start** button on top.

![Run the code](./Demos/images/18_Start.jpg)

If there is a drop down, click **Start** again.

![Run the code](./Demos/images/19_Start.jpg)

Then, you will a console window with the following output.

![Run the code](./Demos/images/20_ConfirmResult.jpg)

### Step 7: Add more complicated function

Let's add little more complicated function. Add a following comment as a block comment.

```csharp
/*
 * Function to randomly assign 4 digit codes to N x M matrix representing lockers
 */
```

![Add more complicated function](./Demos/images/21_AddMatrix.jpg)

Going back to Main function again, start hitting **Enter** and **Tab** buttons to take suggestions.

![Add main](./Demos/images/22_AddMain.jpg)

Sometime, you might need to enter more details result to correct.

![Complete](./Demos/images/23_Completed.jpg)

Sometimes, you might encounter an error like this.

![Error](./Demos/images/24_PossibleError.jpg)

Although you may not get an exactly same result, this example has a problem with index because it was using `i` as an index for both `for` loops. Let's fix that by changing the second `for` loop to use `j` instead of `i`.

![Fix](./Demos/images/25_FixError.jpg)

Remember. Copilot is not perfect, and it can make some dumb mistakes. You might need to fix the code to make it work. You are the main pilot, and Copilot is your assistance.

Your final result when you run the code again might look like this.

![Final result](./Demos/images/26_FinalResult.jpg)

That is it! Congratulation on finishing your first exercise with Copilot. You can try to write more complicated code and see how Copilot can help you.

## 🤝 Contributing
Contributions are warmly welcomed! ✨

To contribute to a public exercise, please refer to our contribution guidelines [here](https://github.com/ps-copilot-sandbox/.github/blob/main/.github/CONTRIBUTING.md).

To create a net new exercise, please use [this repository template](https://github.com/ps-copilot-sandbox/copilot-exercise-template).
