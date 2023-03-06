1. What is NPM?
NPM is one of the popular package manager/software registery for managing development and sharing utilities/packages. One more popular package manager is yarn.

React app is powered by a lot of helper packages for bundling, optimizing, minifying which can be installed and tracked through npm.

Simple Analaogy for better understanding : maven : java :: npm : javscript(react)

Get npm -> npm init -> created package.json file

2. What is Parcel/Webpack? Why do we need it?
Parcel and Wepack are popular Web application bundlers. Bundler comes with many powerful features to simplify the development of complex web applications with multiple dependecies that is production-ready and easily loadable in the browser.

3. What is .parcel-cache
In the current version of parcel (Parcel v2), the information about the project when it is built is stored in .parcel-cache (.cache in parcel v1). So, when the parcel tries to rebuild the project again, it doesn't have to re-parse or repeat the whole process. This helps in building the project faster.

You might notice this while building the project. For the first time, it might take longer (2s in my case) and for subsequent builds the time got reduced (200ms)

4. What is npx ?
execute using npm with entry file name
npx is a npm package runner that is used to execute the command without installing the package (just use on the go). When you run a package using npx, it searches for the package in the local and global registry, and then it runs the package. If the package is not already installed, npx downloads the package files and installs the package, but it will only cache the files instead of saving it.

Examples :

npx parcel index.html -> npx searches for parcel package in your environment and if not found, downloads it and then runs the command. (with index.html as entry point. you can remove index.html and put it in the source of package.json as well)

npx create-react-app my-app -> npx seraches for create-react-app package in your environment, if not found, downlaods it and then creates my-app using create-react-app in the current project directory.


5. What is difference between dependencies vs devDependencies


