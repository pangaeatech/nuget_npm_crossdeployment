# nuget_npm_crossdeployment

This example project demonstrates how to create a "Library" in C#, unit test it using GitHub Actions and package the same types and logic to both NuGet and NPM.    This example project contains a set of interfaces, concrete impementations of those interface and static utility classes.  All of these are compiled into a single DLL for usage by other C# applications.  They are also compiled into an NPM package for use by other JavaScript/TypeScript applications.  

The NPM package contains the following: 
* A `library.wasm` file containing the compiled logic
* An `index.js` file containing `export default async function getLibrary(url)` which returns a promise which resolves to the library object
* An `index.d.ts` file which provides all the type information for the library object returned by `getLibrary(url)`
