matlab_bundler
==============

Work Inprogress
==

A dependancy manager for matlab, similar to bundler but for matlab functions instead of gems.

Each project can have a Funtions file which will pull in Matlab functions from the specified location.

The Function syntax may look something like:

    function "suplabel", git "git://github.com/morganp/matlab_suplabel.git", :tag => "v0.1.0"
