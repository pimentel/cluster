# 'cluster' package with some modifications

This package was imported from CRAN (version 1.15.3). I've modified the
function `clusGap` to accept the argument `do_parallel` to perform the gap
statistic uniform sampling in parallel using the `parallel` package.

- Harold Pimentel <haroldpimentel@gmail.com>, January 12, 2015

-------

# ORIGINAL README :

  This directory contains code, help and examples for CLUS, an S-PLUS
  package for clustering, as described in ``Clustering in an
  Object-Oriented Environment'' by Anja Struyf, Mia Hubert, and Peter
  J. Rousseeuw (Journal of Statistical Software, volume 1).

------------------------------------------------------------------------

See http://www.stat.ucla.edu/journals/jss/ for the original version.

The current port is based on material now on
	http://www.agoras.ua.ac.be/

KH <Kurt.Hornik@ci.tuwien.ac.at> 1998/05/21

---------

For historical reasons,
we keep R/README-Splus which has no relevance to the R package.

---------------------

TODO {see ./DONE-MM for things done}

 3) daisy() for the case of mixed variables should allow
    a weight vector (of length p = #vars) for up- or downweighing variables.
    daisy() really should accept the other methods mva's dist() does _and_
    it should use dist's C API -- but we have no C API for package code, ARRGH!

 4) Eliminate the many Fortran (g77 -Wall) warnings of the form
    >> mona.f:101: warning: `jma' might be used uninitialized in this function

 6) Mona objects describe a hierarchical clustering; they could also inherit
    from twins, and hence have a pltree() method for plotting the
    hierarchical tree.

 8b) Think about "merging" the plot.agnes and plot.diana methods.

------------------

Martin <maechler@stat.math.ethz.ch>, since 1999

