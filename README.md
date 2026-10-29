# C# Labs

A collection of seven independent C# learning projects targeting .NET Framework 4.7.2. Most are console exercises; `mycalc` is a Windows Forms calculator.

## Projects

| Directory | Project type | Exercise |
| --- | --- | --- |
| [`cash bank/`](<cash bank/>) | Console | Menu-driven banking simulation |
| [`Cash Bank Updated/`](<Cash Bank Updated/>) | Console | Expanded banking and customer workflow |
| [`fact calculator/`](<fact calculator/>) | Console | Factorial calculation |
| [`learning c#/`](<learning c#/>) | Console | Basic vector calculation exercise |
| [`vectoral multiplication/`](<vectoral multiplication/>) | Console | Three-dimensional vector cross product |
| [`Yazı yazma hızı/`](<Yazı yazma hızı/>) | Console | Turkish typing-speed exercise |
| [`mycalc/Calculator/`](<mycalc/Calculator/>) | Windows Forms | Desktop calculator interface |

## Build

The projects use the older .NET Framework project format. Build them on Windows with Visual Studio 2022 or MSBuild and the .NET Framework 4.7.2 targeting pack.

For example:

```powershell
MSBuild.exe "fact calculator\fact calculator.csproj" /t:Build /p:Configuration=Debug
```

Open [`mycalc/Calculator/Calculator.sln`](mycalc/Calculator/Calculator.sln) in Visual Studio to work with the Windows Forms calculator.

## Validation status

All seven projects compile with Visual Studio 2022 MSBuild in the current refresh environment. A few historical console exercises still emit compiler warnings for unreachable code or a self-assignment; these warnings were left visible rather than changing the original exercise behavior without dedicated tests.

Generated `bin/`, `obj/`, and user-specific IDE files are excluded from version control. Build outputs should be recreated locally from source.
