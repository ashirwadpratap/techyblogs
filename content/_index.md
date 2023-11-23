# How to fix error "__dirname is not described in ES module scope" in Node


## What is the error message " __dirname isn't defined in ES module scope " in Node?


The blunders message "__dirname is not defined in ES module scope" means that you are attempting to apply the __dirnamevariable in an ES module, but the __dirname variable isn't always available in ES modules with the aid of  default.


## Why is the __dirname variable no longer available in ES modules with the aid of default?


The __dirname variable is a CommonJS global variable that returns the listing call of the modern script. ES modules are a more recent module layout that is designed to be more modular and reusable. ES modules no longer have the right of entry to CommonJS international variables by way of default.


## How to fix the error message "__dirname isn't described in ES module scope"


There are two approaches to repair the mistake message "__dirname isn't described in ES module scope":


- Use the import.Meta.Url property to get the URL of the current module. You can then use the direction. Dirname() technique to get the directory call of the cutting-edge module.


- For instance, the following code shows the way to get the listing name of the modern module using the import.Meta.Urlproperty and the route. Dirname() approach:


- JavaScript
- import path from 'path';


- const __dirname = direction.Dirname(import.Meta.Url);


- Use a 3rd-party bundle to get the __dirnamevariable. There are a few 0.33-party programs that offer the __dirnamevariable for ES modules. One famous package deal is referred to as not unusual-es.


### To use the commonplace-es bundle, you can set up it the usage of the subsequent command:


- npm deploy commonplace-es


- Once the package deal is established, you can import it into your code and use the getGlobals() characteristic to get the __dirnamevariable.


- For example, the subsequent code indicates how to get the __dirnamevariable using the not unusual-es bundle:


- JavaScript
- import  getGlobals  from 'common-es';


- const __dirname getGlobals().__dirname;


- To fix error “_ _dirname is not defined in Es module scope “ in node


1. Use CommonJS Modules:
The easiest manner to resolve this mistake is to change from the use of ES modules to CommonJS modules through changing the report extension from ".Mjs" to ".Cjs" or ".Js". CommonJS modules have an entry to the __dirname and __filename variables.


For example, if you have a report named "myModule.Mjs," trade it to "myModule.Cjs" or "myModule.Js."


2. Use import.Meta.Url:
If you need to retain the use of ES modules, you could use the import.Meta.Url property to get the current module's URL, which you can then parse to extract the listing path. Here's an example:


### import { fileURLToPath } from 'url';
### import { dirname } from 'path';


### const __filename = fileURLToPath(import.meta.url);
### const __dirname = dirname(__filename);


// Now, you can use __dirname in your code.




## Which method should you use?


Which technique you use to fix the error message "__dirname is not defined in ES module scope" relies upon your precise desires. If you are only using the __dirname variable in some places in your code, then you may use the import. Meta.Urlproperty and the route.Dirname() technique.
If you use the __dirname variable in many places in your code, or in case you want to apply an improved answer, then you can use a 3rd-celebration bundle like commonplace-es.


## Conclusion


The error message "__dirname is not described in ES module scope" is a commonplace error which could arise while switching from CommonJS modules to ES modules. There are two approaches to fix this mistake: using the import.Meta.Url assets and the direction.Dirname() method, or using a 3rd-birthday celebration package deal like not unusual-es.


## Additional notes


If you are using a module bundler like Webpack, you may also use the __dirname variable in ES modules via configuring Webpack to remedy CommonJS modules.


If you're using TypeScript, you could additionally use the __dirname variable in ES modules by permitting the resolveJsonModule compiler option.


