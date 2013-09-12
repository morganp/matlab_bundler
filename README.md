matlab_bundler
==============

Work Inprogress
==

A dependancy manager for matlab, similar to bundler but for matlab functions instead of gems.

Each project can have a Funtions file which will pull in Matlab functions from the specified location.

The Function syntax may look something like:

    function "suplabel", git "git://github.com/morganp/matlab_suplabel.git", :tag => "v0.1.0"

It is built around a standardised layout for released code : 

    ├── function
    ├── lib
    ├── package
    │   └── +demo_pkg
    ├── test
    └── testharness

Standard functions can be placed in the functions folder. package is expected to hold functions and object contained with in a Matlab Package.

For Simulink distributions 'lib' can hold a simulink library, 'testharness' will be the test harness required to instantiate the library componets with data source and sinks.

test, should contain a matlab executable script which runs pass/fail tests on the function, packaged functions or objects or simulates and verifies output from the testharness.   

Examples
==

[suplabel]: https://github.com/morganp/matlab_suplabel
[padarray]: https://github.com/morganp/matlab_padarray
