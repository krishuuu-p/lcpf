# LCPF README

Welcome to the README of LeetCode problem fetcher VSCode extension! This extension helps you fetch leetcode problems on your local machine and test them against the given testcases as well as those of your own! Moreover you can also choose to add testcases from a local text file. 

All this while writing no driver code! Yes, the driver code will be automatically generated according to the problem that you are working on. But since the variety of problems is vast and given that this project was developed against a tight deadline, I was not able to tackle every case. Barring the problems consisting of a parameter with pointer datatype, in which case you will be explicitly prompted to write the driver code on your own, the generated driver code should work fine.

## Key Assumptions
Some assumptions were made in order to efficiently tackle variety of problems available on LeetCode:

1. The vector input will be given in one line and one line only i.e the parameter of vector datatype will not contain any new line character within it.

2. In case when parameter is of type 'vector<vector<>>' the user is expected to enclose all the inner vectors within square brackets ([]) with opening square bracket one line prior to first inner vector and closing square bracket on the next line of the last inner vector. (see Known Issues section)

3. Input is given in the same order as parameters passed in the function. (see Known Issues section)

## Supported Languages
1. C++
2. Python

## Features

### Demo Video
[Watch the Demo Video Here: ](https://drive.google.com/file/d/1NM2i0FIthgAaMbyN50YCxxs5KAXHclSQ/view?usp=drive_link)

1. Automatically generated driver code.
2. Running code against example as well as user defined testcases.
3. Displays expected output vs received output for each testcase.
3. Proper error messages if testcase fails.
4. Fetching and running code against testcase from local text files.
5. Custom configurations for supported languages in settings.
6. Saves fetched testcases in files according user preferences in settings.

## Extension Settings

* `lcpf.general.saveTestCases`: Whether or not to save fetched testcases to a file.
* `lcpf.general.saveLocation`: Location where you want to save your files.
* `lcpf.general.templateFileLocationCpp`: Path of the C++ template file for leetcode problems.
* `lcpf.general.templateFileLocationPython`: Path of the python template file for leetcode problems.
* `lcpf.language.cpp.Args`: Additional Compilation flags for C++ files.
* `lcpf.language.cpp.Command`:Command used to compile .cpp files. Example 'g++', 'g++-10', 'clang++', etc.
* `lcpf.language.python.Args`: Compilation flags for Python files.
* `lcpf.language.python.Command`: Command used to run python files. Example 'py', 'python3', 'pypy3', etc."

## Known Issues

1. Handling of data-type vector<vector<>> : I am aware of the fact that this datatype can be tackled without the assumptions made and I am working on it.

2. User giving datatypes not in the same order as the parameters in the function : This can also be tackled using a simple hashing and this issue will be fixed soon.

3. Restoring state of webview if the editor is closed or changed.

## Release Notes

### 1.0.0

Initial release of LeetCode Problem Fetcher.

---
#   l c p f  
 