# ninetails
![Private Status Badge](https://img.shields.io/badge/status-private_beta-blue) ![Test Passing Badge](https://img.shields.io/badge/test-passing-orange)

ninetails is a tool for reverse engineering browser javascript code. It can fully deobfuscate the most secure `javascript-obfuscator` configuration and unpack browserify, webpack, and rollup bundles.

* Removes Debug Protection and Self Defending code.
* Removes dead code branches.
* Restores flattened control flow.
* Unpack constants from shuffled string arrays.
* Idenfities multiple types of anti-tampers.
* Simplifies expressions, properties and objects.
* Restores disabled console output.
* Rename cryptic scope variables 
* Monitors enviroment changes and function calls in a sandbox and recreats a script as a last ditch effort.

## Installation
```bash
cd ninetails # Go into the ninetails directory
npm install # Install required packages
npm run build # Build ninetails
npm install . -g # Install ninetails globally
```

## Usage
```bash
ninetails obfuscated.js -o deobfuscated.js # Deobfuscate a file

ninetails bundle.js --unpack -o modules # Unpack a webpack or browserify bundle
```

## Contact
Feel free to DM me on Discord about anything at `shrekent#2783`.