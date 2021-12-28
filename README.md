# LspCpp

## Dependencies
`LspCpp` depends on the boost and rapidjson,utfcpp,uri and threadpool

## Build

### Linux / Mac
1. On linux ,install boost
   ```shell
      $ sudo apt-get install libboost-dev 
   ``` 
   On Mac,install boost on Mac
   ```shell
      $ brew install boost
   ``` 

2. [Restore the submodules][4].
   ```shell
     $ git submodule init
     $ git submodule update
   ``` 
3. Building with ``CMake``
-----------------------
	$ mkdir _build
	$ cd _build
	$ cmake ..
	$ make -j4

### Windows

  1. [Restore the submodules][4].
     ```shell
      git submodule init
      git submodule update
     ``` 
  2. Open cmd or powershell and generate visual studio project  with ``CMake``.
  -----------------------
    mkdir _build
	cd _build
	cmake -DUri_BUILD_TESTS=OFF  ..

  3. "cmake -help" is useful if you are not familiar with cmake.
  
  4. Build it with Visual Studio.
 
## Reference
 Some code from :[cquery][1]

## Projects using LspCpp:
* [JCIDE](https://www.javacardos.com/tools)
* [LPG-language-server](https://github.com/kuafuwang/LPG-language-server)
## License
   MIT
   
##  Example:
[It's here](https://github.com/kuafuwang/LspCpp/tree/master/examples)


[1]: https://github.com/cquery-project/cquery "cquery:"
[2]: https://www.javacardos.com/tools "JcKit:"
[3]: https://docs.microsoft.com/en-us/nuget/consume-packages/package-restore "Package Restore"
[4]: https://git-scm.com/book/en/v2/Git-Tools-Submodules "Git-Tools-Submodules"
