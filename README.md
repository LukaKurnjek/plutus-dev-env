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
  will contain the *aiken.toml* file that contains the metadata about the project, as well as dependencies required by it. 
* If you want to see that all dependencies get download successfully you can use the `aiken check` command. 
* To build an existing aiken project `cd` into that project folder and run `aiken build`. This command generates a [CIP-0057 Plutus blueprint](https://cips.cardano.org/cip/CIP-0057) 
  as *plutus.json* at the root of your project. The blueprint describes the on-chain contract and its binary interface. In particular, it contains 
  the generated on-chain code that will be executed by the ledger, and a hash of the validator(s) that can be used to construct addresses. 

**Notes:**
* The *plutus.json* file in this repository includes compiled code for all validators from the *validators* folder that was 
  compiled with Aiken v1.0.29-alpha. If re-building the project with a newer version of Aiken the compiled code may change. 
  That does not impact the functionality of the code but can improve its performance. 
* To get a list of all available aiken actions for the CLI simply run the `aiken` command without arguments. 
* The language server protocol (LSP) doesn't work if filename uses camel case (eg. ❌ `myValidator.ak` ✅ `my-validator.ak`) 

**Learning resources:**
* The get a basic understanding of the Aiken programming language you can check out the *Language tour* at the official documentation, that 
  starts with [Primitive types](https://aiken-lang.org/language-tour/primitive-types). Further chapters can be accessed on the left-side menu. 
* The [Awsome Aiken](https://github.com/aiken-lang/awesome-aiken) repository provides links to Aiken libraries, DApps, tutorials and video lessons.
* You can also check out the [Aiken for Amateurs](https://piefayth.github.io/blog/pages/aiken1/) tutorial, that is currently not include in Awsome Aiken. 
* If you are starting with your Cardano journey you might want to check out the [What I wish I knew](https://aiken-lang.org/fundamentals/what-i-wish-i-knew) 
  page that provides tips and secret knowledge and the [EUTXO chrash course](https://aiken-lang.org/fundamentals/eutxo) page that explains the EUTXO accounting model. 
* Also the PPP4 lectures [Hashing and Digital Singatures](https://youtu.be/f-WKPWbk9Jg) and [The EUTXO model](https://youtu.be/ulYDNaEKf4g) provide some 
  begginer friednly explanations. 
  