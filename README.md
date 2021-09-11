# EcsRxUnitySlnMergeExample

Example of using the following tools together:

Visual Studio

EcsRx (and SystemsRx)

Unity

EcsRx Unity

SlnMerge



## Notes

Example projects are empty.  I may fill in the examples at a later date if desired.

SystemsRx is not copied to Unity becasue it is referenced as NuGet package by EcsRx.  If you want to include in the build, Fork the project on GitHub, and break that link.

SlnMerge throws everthing into the root.  The project nesting options will help, but you'll have to do it manually every time you add a dependency with an asmdef.  It would be better if the MergeTargetSolution setting had a Folder argument.
