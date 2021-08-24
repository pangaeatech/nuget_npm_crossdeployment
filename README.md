# nuget_npm_crossdeployment

This example project demonstrates how to create a "Library" in C#, unit test it using GitHub Actions and deploy the same types and logic to both NuGet and NPM.    This example project contains a set of interfaces, concrete impementations of those interface and static utility classes.  All of these are compiled into a single DLL which is deployed to NuGet for usage by other C# applications.  The logic is compiled into an NPM packages which is deployed to NPM for use by other JavaScript/TypeScript applications.  The interaces and types are compiled into an NPM package which is deployed to NPM for use when typechecking other TypeScript applications which use the corresponding NPM logic package.

