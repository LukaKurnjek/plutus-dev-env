# Plutus Pioneer Program v4 contracts translated to Aiken 

This branch contains a translation of the Plinth on-chain code examples from the 
4th Plutus Pioneer program. They are re-writen in the Aiken smart contract language. 

**Installation instructions:**
* First you will need to install the tooling manager *aikup*. Instructions can be found at the [official page](https://aiken-lang.org/installation-instructions).
* Once installed you can simply run the `aikup` command with no arguments and it will install the *aiken* CLI which is used to build and compile projects. 
* Aiken comes with a built-in language server. The aiken docs provide [configuration instructions](https://aiken-lang.org/installation-instructions#language-server). 
* Aiken can be integrated with the Zed, VSCode, Vim/Neovim and Emacs editors. Instructions can be found at the following [aiken docs](https://aiken-lang.org/installation-instructions#editor-integrations).  

**Creating and building a project:**
* To create a project you can use the command `aiken new --help` that will provide instructions for input parameters. The created project 
  will contain the *aiken.toml* file that contains the metadata about the projects, as well as dependencies required by it. 
* If you want to see that all dependencies get download successfully you can use the `aiken check` command. 
* To build an existing aiken project `cd` into that project folder and run `aiken build`. This command generates a [CIP-0057 Plutus blueprint](https://cips.cardano.org/cip/CIP-0057) 
  as *plutus.json* at the root of your project. The blueprint describes the on-chain contract and its binary interface. In particular, it contains 
  the generated on-chain code that will be executed by the ledger, and a hash of the validator(s) that can be used to construct addresses. 

**Notes:**
* To get a list of all available aiken actions for the CLI simply run the `aiken` command without arguments. 
* The language server protocol (LSP) doesn't work if filename uses camel case (eg. ❌ `myValidator.ak` ✅ `my-validator.ak`) 


