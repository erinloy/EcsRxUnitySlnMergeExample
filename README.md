# EcsRxUnitySlnMergeExample

Example of using the following tools together:

Visual Studio

EcsRx (and SystemsRx)

Unity

EcsRx Unity

SlnMerge


## Based on these instructions

https://discord.com/channels/488609938399297536/488611200901578752/838476035996778497

## Notes

Example projects are empty.  I may fill in the examples at a later date if desired.  The (not implemented) main point is that they can use EcsRx/SystemsRx libraries outside of Unity, and that class libaries and (EcsRx/SystemsRx) Plugins can also be shared with Unity and Non-Unity code.

I used .NET Standard 2.0 as the common/shared runtime.  .NET 4.x (6) can also be used if needed.  To change what gets copied to Unity, alter the ProejctCode.Unity build to target the runtime of choice.  I used .NET 5 here to ensure that .NET Standard libaries are included in the build.  There are other ways to do this if needed. 

SystemsRx is not copied to Unity becasue it is referenced as NuGet package by EcsRx.  If you want to include in the build, Fork the project on GitHub, and break that link.

SlnMerge throws everthing into the root.  The project nesting options will help, but you'll have to do it manually every time you add a dependency with an asmdef.  It would be better if the Folder argument had a wildcard option.
